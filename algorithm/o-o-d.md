# o o d

```

function Person(name, age) {
    //私有属性和方法
    var sex = '秘密㊙';
    var getSex = function () {
        console.log(sex)
    }

    //公有属性和方法
    this.name = name;
    this.age = age;
    this.descript = '我是共有属性'
    this.getInfo = function () {
        getSex()
        console.log(this.name, this.age)
    }
}
//静态属性和方法
Person.descript = '我喜欢吃火锅...';
Person.work = function () {
    console.log('我是一名前端开发工程师')
}
//给原型对象添加属性和方法
Person.prototype.descript = '我是原型上的属性'
Person.prototype.hobby = ['游泳', '跑步'];
Person.prototype.getHobby = function () {
    console.log(p1.hobby)
}

var p1 = new Person('丽萨',23);

console.log(p1)

console.log(p1.sex) //  私有属性  undefined

console.log(p1.descript) // 我是共有属性

//因为自己有descript属性，所以直接使用自己的属性

console.log(p1.hobby)  // 原型中的属性  ["游泳", "跑步"]

console.log(Person.descript)  //静态属性  我喜欢吃火锅...

Person.work()  //静态方法    我是一名前端开发工程师

p1.getInfo() //  共有方法  秘密㊙ 丽萨  23  

p1.getHobby() //原型中的方法  打印hobby
//自己没有该方法，但是在原型上找到了，所以可以打印出来

// p1.getSex() // 私有属性   报错

// p1.work(); // 静态方法  报错

console.log(Person.sex) // 报错  静态属性


作者：卡布奇诺__
链接：https://juejin.cn/post/6846687603484262414
来源：稀土掘金
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。
```
