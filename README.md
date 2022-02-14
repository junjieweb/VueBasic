# vue_basic

## 初识Vue

1. 想让Vue工作，就必须创建一个Vue实例，且要传入一个配置对象；
2. root容器里的代码依然符合html规范，只不过混入了一些特殊的Vue语法；
3. root容器里的代码被称为【Vue模板】；
4. Vue实例和容器是一一对应的；
5. 真实开发中只有一个Vue实例，并且会配合着组件一起使用；
6. {{xxx}}中的xxx要写js表达式，且xxx可以自动读取到data中的所有属性；
7. 一旦data中的数据发生改变，那么页面中用到该数据的地方也会自动更新；

<span style="color:red;">注意区分：js表达式 和 js代码(语句)</span>

1. 表达式：一个表达式会产生一个值，可以放在任何一个需要值的地方：

```javascript
(1). a
(2). a+b
(3). demo(1)
(4). x === y ? 'a' : 'b'
```

2. js代码(语句)

```javascript
(1). if(){}
(2). for(){}
```

## 模板语法

Vue模板语法有2大类：

* 插值语法：
* 功能：用于解析标签体内容。
* 写法：{{xxx}}，xxx是js表达式，且可以直接读取到data中的所有属性。
2.指令语法：
* 功能：用于解析标签（包括：标签属性、标签体内容、绑定事件.....）。
* 举例：v-bind:href="xxx" 或  简写为 :href="xxx"，xxx同样要写js表达式，且可以直接读取到data中的所有属性。
* 备注：Vue中有很多的指令，且形式都是：v-????，此处我们只是拿v-bind举个例子。
