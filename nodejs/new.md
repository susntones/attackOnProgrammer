new操作符具体干了什么呢?其实很简单，就干了三件事情。

```javascript
var obj  = {};
obj.__proto__ = Base.prototype;
Base.call(obj);
```

* 第一行，我们创建了一个空对象obj
* 第二行，我们将这个空对象的__proto__成员指向了Base函数对象prototype成员对象
* 第三行，我们将Base函数对象的this指针替换成obj，然后再调用Base函数。