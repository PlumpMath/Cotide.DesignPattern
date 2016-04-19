 
## 设计模式

### 策略模式 （Strategy）

>  定义算法家族，分别封装起来，让它们之间可以互相替换，此模式让算法的变化，不会影响到使用算法的客户。在分析过程中如果需要在不同的时间应用不同的业务规则，就可以考虑使用策略模式处理这种变化的可能性。

#### 优点

* 策略模式提供了对“开闭原则”的完美支持，用户可以在不修改原有系统的基础上选择算法或行为，也可以灵活地增加新的算法或行为。
* 策略模式提供了管理相关的算法族的办法。
* 策略模式提供了可以替换继承关系的办法。
* 使用策略模式可以避免使用多重条件转移语句。
   
#### 缺点 

* 客户端必须知道所有的策略类，并自行决定使用哪一个策略类。
* 策略模式将造成产生很多策略类，可以通过使用享元模式在一定程度上减少对象的数量。
  

#### 适用环境
* 如果在一个系统里面有许多类，它们之间的区别仅在于它们的行为，那么使用策略模式可以动态地让一个对象在许多行为中选择一种行为。
* 一个系统需要动态地在几种算法中选择一种。
* 如果一个对象有很多的行为，如果不用恰当的模式，这些行为就只好使用多重的条件选择语句来实现。
* 不希望客户端知道复杂的、与算法相关的数据结构，在具体策略类中封装算法和相关的数据结构，提高算法的保密性与安全性。



### 装饰模式 （Decorator）

> 动态地给一个对象添加一些额外的职责，换言之客户端并不会觉得对象在装饰前和装饰后有什么不同。装饰模式可以在不需要创造更多子类的情况下，将对象的功能加以扩展,这就是装饰模式的模式动机。

#### 优点:

* 装饰模式与继承关系的目的都是要扩展对象的功能，但是装饰模式可以提供比继承更多的灵活性。
* 可以通过一种动态的方式来扩展一个对象的功能，通过配置文件可以在运行时选择不同的装饰器，从而实现不同的行为。
* 通过使用不同的具体装饰类以及这些装饰类的排列组合，可以创造出很多不同行为的组合。可以使用多个具体装饰类来装饰同一对象，得到功能更为强大的对象。
* 具体构件类与具体装饰类可以独立变化，用户可以根据需要增加新的具体构件类和具体装饰类，在使用时再对其进行组合，原有代码无须改变，符合“开闭原则”
 

#### 缺点:

* 使用装饰模式进行系统设计时将产生很多小对象，这些对象的区别在于它们之间相互连接的方式有所不同，而不是它们的类或者属性值有所不同，同时还将产生很多具体装饰类。这些装饰类和小对象的产生将增加系统的复杂度，加大学习与理解的难度。
* 这种比继承更加灵活机动的特性，也同时意味着装饰模式比继承更加易于出错，排错也很困难，对于多次装饰的对象，调试时寻找错误可能需要逐级排查，较为烦琐。


## 原则

### 单一职责原则

> 单一职责原则 (SRP)，就一个类而言，应该仅有一个引起它变化的原因。


### 开放-封闭原则

> 开放-封闭原则，是说软件实体（类、模块、函数等等）应该可以扩展，但是不可修改。

 
### 依赖倒转原则

> 依赖倒转原则

* 高层模块不应该依赖底层模块，两者都应该依赖抽象。
* 抽象不应该依赖细节，细节应该依赖抽象。

### 里氏代换原则

> 里氏代换原则 (LSP)，子类型必须能够替换掉它们的父类型。


 
## 感激
感谢以下的书籍
* 大话设计模式 
* Head First 设计模式 
* [图说设计模式](http://design-patterns.readthedocs.org/)
