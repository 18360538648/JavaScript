# ES^学习笔记

## 1.箭头函数

箭头函数是ES6引入的编写函数的新语法，通过与ES5进行对比，少了function和return申明

```
 // ES5
    var selected = allJobs.filter(function (job) {
      return job.isSelected();
    });
    // ES6
    var selected = allJobs.filter(job => job.isSelected());
    
  //两个参数
    // ES5
    var total = values.reduce(function (a, b) {
      return a + b;
    }, 0);
    // ES6
    var total = values.reduce((a, b) => a + b, 0);
```

## 2.=、==、===、！=、！==

* = ：赋值运算符
* == ：值是否相等(不考虑类型)
* === ：值和类型都要相等
* ！= 不严格的不等判读(只判读值)
* ！== 严格的不等判断(值和类型都要判断)