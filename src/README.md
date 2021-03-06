# 组件示例

组件编写示例。

## config

组件配置。

| 配置项 | 含义 |
| :---: | :--- |
| name | 组件名；必需。 |
| data | 组件的模板的默认数据；可选。|

组件名会经过[name.js](../name.js)转化，用于组件的html元素的id，以及组件模块导出的文件名、全局函数名。

## template

组件的模板部分，使用[ejs](http://ejs.co)（兼容原生html）。

## style

组件的样式部分，使用[scss](https://sass-lang.com)（兼容原生css）。

在打包时会在最外层加封一个组件ID选择器（详见[pre.js](../pre.js)执行过程），很大程度避免了css污染问题。

## init

组件的初始化代码，并导出一个初始化函数。
