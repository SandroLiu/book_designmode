# 迪米特法则
英文`Law of Demeter`，缩写`LoD`，也称最少知识原则`Least Konwledge Principle`，缩写`LKP`。

## 定义
一个对象应该对其他对象有最少的了解，通俗地讲，一个类应该对自己需要耦合或调用的类知道得最少。

## 注意

- 只与直接的朋友通信。每个对象都必然会与其他对象有耦合关系，两个对象之间的耦合就成为朋友关系，这种关系的类型有很多，例如组合、聚合、依赖等。

- 朋友类的定义是这样的：出现在成员变量、方法的输入输出参数中的类称为成员朋友类，而出现在方法体内部的类不属于朋友类

- 如果一个方法放在本类中，既不增加类间关系，也对本类不产生负面影响，那就放置在本类中