## breeze-date

这是一个基于原生JavaScript开发的移动端下拉选择插件

## 版本 

1.0.0

## 安装

使用npm下载源文件


```
npm install breeze-selector --save
```

直接使用script引用

```js
<script src="../dist/breeze-selector-1.0.0.min.js"></script>
```

## 使用

```js
<script type="text/javascript">
  let ageRange = [];
  for ( let i = 0; i < 29; i++ ) {
    ageRange.push({
      id: i,
      value: 22 + i,
      label: ( 22 + i ) + '岁'
    });
  }
  var SELECTOR1 = new BreezeSelector({
    target: "selector1",
    type: "date",
    format: 'age',
    currentValue: ['30岁'],
    data: [ageRange]
  });
</script>
```

## 参数
```
```

|        参数       |   类型   | 默认值  |             说明             |
|-------------------|----------|----------|-------------------------------------|
| target              | String    | “picker”       | 目标元素id          |
| currentValue             | Array   | 0      | 当前值 |
| data             | Array   | 0      | 数据[二维数组] |
| ensureCallback       | Function   | 空函数   | 点击确定之后执行回调函数          |

## 演示

[demo](https://breeze55.github.io/breeze-selector/example/index.html)

```
如果你感觉好用，欢迎给我打赏
```
![avatar](https://raw.githubusercontent.com/breeze55/static/master/breeze.png)

## License
[MIT](https://github.com/breeze55/breeze-selector/blob/master/LICENSE)
