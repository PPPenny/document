笔记

JS笔记



_.extend(param,param,param)   浅拷贝，后面的赋给第一个，如果重复，后面替换前面

_.findWhere(data,{查询条件});     返回符合条件的对象{}

_.where(data,{查询条件});             返回一个数组对象[{},{}]

_.pick(obj,key1,key2);                    从对象中返回需要的key重组新对象，如果不存在key，则返回{}







ES笔记



object.assign({},...source);

ES6的深拷贝，{} 目标对象

...source 源拷贝对象，把...source里的拷贝到{}对象里面，如果...source里面有属性名相同的，后面的覆盖前面的



=>

右边代码块多于一条语句，就要使用大括号将它们括起来，并且使用return（）返回，返回的是对象则：return({"key1":"value1","key2":"value2"});

不带{}:默认直接返回

（1）函数体内的this对象，就是定义时所在的对象，而不是使用时所在的对象。

（2）不可以当作构造函数，也就是说，不可以使用new命令，否则会抛出一个错误。

（3）不可以使用arguments对象，该对象在函数体内不存在。如果要用，可以用Rest参数代替。

（4）不可以使用yield命令，因此箭头函数不能用作Generator函数。

```
this指向的固定化，并不是因为箭头函数内部有绑定this的机制，实际原因是箭头函数根本没有自己的this，导致内部的this就是外层代码块的this。正是因为它没有this，所以也就不能用作构造函数。
```



router:根据路径找到对应组件，并渲染的过程称为路由

<Link to="/path">  link创建HTML链接元素，点击后不跳转，被link截取跳转，把跳转的路径传给router,实现渲染



字符串拼接:  {'string'+this.var}      string :表示原本的字符串，this.var表示变量

字符模板 ``,中间包含变量则：${var} 表示

 **for...in语句**以任意顺序遍历一个对象的[可枚举属性](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Enumerability_and_ownership_of_properties)。对于每个不同的属性，语句都会被执行。



for in遍历的是数组的索引，而for of遍历的是数组元素值