var F = function(){
    // this指向谁，在定义时是不知道的
}
var p = new F;

(1) 新建一个对象
instance = new Object()

(2)设置原型链
instance.__proto__ = F.prototype;

(3) 让F中的this指向instance，执行F的函数体
（4）判断F的返回值类型
如果是值类型，就丢弃它，还是返回instance。
如果是引用类型，就返回这个引用类型的对象，替换掉instance。