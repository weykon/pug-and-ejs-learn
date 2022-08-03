# PUG

![Playground](https://pug.vercel.app/)

原名jade （whatever）

缩进敏感
空格敏感

## 流程代码

+ if () else 无大括号

+ for  

```
- var arr = [1,2,3,4,5] 
ul 
 - for(var i=0;i<arr.length;i++) 
 li= arr[i] 
```

+ each val in [1,2,3,4]

```
- var arr = {name:'binge',six:'man'} 
ul 
 each val in arr 
 li= val 
```

标签直接字母 div

标签属性括号内 div(class=['aa'])

## 变量

+ 字母前#和大括号， #id  是id标识
比如  p #{obj.name} 变量下

+ 前置 - ，比如 - var bool = true
直接变量

+ #[] 这样是嵌入pug的代码

样式p(style="color="black";")
或者p(style={color="black",})

(extends, block content) 说是继承，相当上下文拼接

mixin 相当于标识函数体
mixin todo(param)
  // anything

+ todo("ai~") // 调用

try my silly md work ⬇️ hahaha

## ! 和 # ？

|         |      |          |
| ----------|--- | -----:|
| let a = 1  |   | ```<p>1</p>``` |
| p #{a}      | **=>** | ```<p>1</p>``` |
| p !{a}       | |                |

<p>```let a = 1```</p> <p>```p #{a}```</p><p>```p #{a}```</p> | => | <p>```<p>1</p>``` </p> <p>```<p>1</p>```</p>
--- | --- | ---