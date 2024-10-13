# JS + CSS Clock

本挑战主要练习了：

- CSS 中的 transform[rotate] / transition 属性
- JS setInterval 方法
- CSS 伪类

## 待改进内容

### box-shadow

```css
    .clock-face:after {
      width: 1em;
      height: 1em;
      left: 50%;
      top: 50%;
      position: absolute;
      display: block;
      content: '';
      background-color: #a8c5d1;
      border-radius: 50%;
      box-shadow:
              0 0 0 2px rgba(0,0,0,0.1),
              0 0 10px rgba(0,0,0,0.2);
      transform: translate(-50%, -50%);
    }
```