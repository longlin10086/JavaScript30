# Array Cardio Day 1

本挑战主要练习了：

- JS 数组的 filter / map / sort / reduce 方法
- 将 NodeList 转化成 数组
- 字符串 子串包含问题 / split 方法

## 待学习知识

### reduce()

```js
    console.log(
            data.reduce((result, currentValue) => {
              if (!result[currentValue]) result[currentValue] = 0;
              result[currentValue]++;
              return result;
            }, {})
    );
```

