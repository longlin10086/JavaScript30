# CSS Variables

本挑战主要练习了：

- CSS 中的 variable 变量使用以及如何通过 JS 更改
- 如何给页面元素 addEventListener
- 如何给 图片 / 元素 增添模糊效果

另外，在本项目中我发现打开 Edge 调试器窗口后 mousemove 的 eventListener 会失效；
并且，Edge 也并不支持对 color input 进行 mousemove 的 eventListener；
addEventListener 中传入的函数尽量不要使用 arrow function，会造成未知问题。

## 待改进内容

### filter 属性

```css
    img {
      background: var(--base);
      padding: var(--spacing);
      filter: blur(var(--blur));
    }
```

### setProperty 方法

```js
    function inputHandler() {
      const suffix = this.dataset.sizing || '';
      document.documentElement.style.setProperty(`--${this.name}`, `${this.value}` + suffix);
    }
```

