# 本次课程你将学到

- 类型注解
- 接口
- 类

### 类型注解

TypeScript里的类型注解是一种轻量级的为函数或变量添加约束的方式。

首先我们创建一个后缀为ts的文件demo.ts

文件中编写以下代码

```typescript
function greeter (person:string){
  return 'hello' + person
}

let myName:string = "xiaoming"

greeter('xiaoming')
```
其中string就是我们的类型注解
不仅仅可以使用string我们还可以

- boolean  布尔值
```js
let isTrue:boolean = true
```
- number   数值
```js
let age:number = 22
```
- string   字符串
```js
let name:string = 'xiaoming'
```
- number[] 数组
```js
let arr: number[] = [1,2,3]
```
- [string,number] 元组
```js
let x:[string,number,boolean]

x = ['hello',5,false]
```
- enum 枚举

```ts
enum Color {Red, Green, Blue}
let c: Color = Color.Green;
```
- Any
```
let name:Any = 'xiaohong'
```
最后我们打开终端在对应文件夹目录下运行

``` javascript
tsc demo.ts
```

在你的目录文件夹中会生成一个demo.js文件


