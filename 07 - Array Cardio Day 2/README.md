# Array Cardio Day 2

本挑战主要练习了：

- JS 数组 some / every / find / findIndex / splice 方法

## 待学习知识

### splice 与 slice 区别

```js
comments.splice(index, 1);

const newComments = [
    ...comments.slice(0, index),
    ...comments.slice(index + 1)
];
```