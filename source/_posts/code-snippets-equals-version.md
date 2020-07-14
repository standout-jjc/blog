---
title: TS比较版本号大小算法
toc: true
comments: true
date: 2020-07-14 10:41:12
categories:
  - [code snippets]
tags:
  - [code snippets]
  - TypeScript
---

## 使用递归判断版本号大小 ##

``` typescript
function equalsVersion(curVersion: string, minVersion: string): boolean {
  const curVersionNumber: number[] = curVersion.replace(/[vV]/, '')
    .split('.').map((number: string) => parseInt(number));
  const minVersionNumber: number[] = minVersion.replace(/[vV]/, '')
    .split('.').map((number: string) => parseInt(number));
  const equals: Function = function (curVersion: number[], minVersion: number[], index: number = 0): boolean {
    if (index >= curVersion.length && index >= minVersion.length) {
      return true;
    }
    if ((curVersion[index] || 0) < (minVersion[index] || 0)) {
      return false;
    }
    return equals(curVersion, minVersion, index + 1);
  };
  return equals(curVersionNumber, minVersionNumber);
} 
```

> JEST 测试

```typescript
test('test equalsVersion', function () {
  expect(equalsVersion('v0.1', 'v2.1')).toBeFalsy();
  expect(equalsVersion('v0.1', 'v0.1.1')).toBeFalsy();
  expect(equalsVersion('v0.1', 'v0.1.999999')).toBeFalsy();
  expect(equalsVersion('v0.1', 'v0.1.8.123')).toBeFalsy();

  expect(equalsVersion('v1.1.0', 'v1.0.0')).toBeTruthy();
  expect(equalsVersion('v0.1.0', 'v0.1.0')).toBeTruthy();
  expect(equalsVersion('v0.1', 'v0.1.0')).toBeTruthy();
  expect(equalsVersion('v0.1.0', 'v0.1')).toBeTruthy();
  expect(equalsVersion('V0.1.0', 'V0.1.0')).toBeTruthy();
  expect(equalsVersion('0.1.0', 'V0.1.0')).toBeTruthy();
  expect(equalsVersion('v0.1.0', '0.1.0')).toBeTruthy();
});
```
