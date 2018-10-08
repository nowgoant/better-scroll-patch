# 基于 better-scroll v1.12.6，打的补丁.

修订如下：

### 2019-10-08 修改

```
 function getNow() {
  var _getnow =
    window.performance && window.performance.now
      ? window.performance.now() +
        (window.performance.timing
          ? window.performance.timing.navigationStart
          : 0)
      : +new Date();
  // console.log('_getnow', _getnow);
  return _getnow;
}
```
