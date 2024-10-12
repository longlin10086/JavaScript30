# 01 JavaScript Drum Kit

本挑战主要练习了：

- 利用 JS 添加 / 移除 class 属性；
- 如何响应键盘事件；
- 简单的异步处理（原代码有个小 bug，当我一直按一个按键时会导致 class 无法移除）

## 待改进内容

### QuerySelector

```js
    const audio = document.querySelector(`audio[data-key="${e.keyCode}"]`);
    const key = document.querySelector(`div[data-key="${e.keyCode}"]`);
```