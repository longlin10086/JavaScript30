# Type Ahead

本挑战主要练习了：

- 如何完成一个好看的搜索框
- 如何在 JS 中使用正则表达式
- 字符串 replace / join 方法
- Array 的 push 方法

## 待学习知识

### RegExp / replace

```js
  function matchCities(text, c) {
    const reg = new RegExp(text, "gi");
    c = c.filter(city => reg.test(city.city) || reg.test(city.state));
    const HTMLs = c.map(city => {
      let hlCity = city.city.replace(reg, `<span class="hl">${text}</span>`);
      let hlState = city.state.replace(reg, `<span class="hl">${text}</span>`);
      let Population = city.population.replace(/\B(?=(\d{3})+(?!\d))/g, ",");
      return `<li>
            <span class="name">${hlCity}, ${hlState}</span>
            <span class="population">${Population}</span>
        </li>`;
            }
    )
    suggestion.innerHTML = HTMLs.join('\n');
    console.log(HTMLs);
  }
```