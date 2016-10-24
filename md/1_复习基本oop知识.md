#复习基本OOP技术

[TOC]
##內容概述
###1. “Oriented”的涵意

* ”O-oriented”: 面向对象，世界一切都是由对象构成。软件中以对象的方式来编程
* -Oriented,Based,Driven,-Centered区别
 + -Based :基于需求，有先后的顺序。
 	> eg：软件中先需求分析；然后基于需求分析文档的结果（文件），而进行后续的软件开发活动，所以称为：<font color=blue> Requirement-based software development</font>
 + Driven :引导
    就向北极星引导我们,指出方向而已。也向汽车司机(Driver)只是引导汽车方向,并没有去驱动汽车;而是引擎才是驱动汽车
    > eg:Model-driven(以软件模型作为引导开发)； Use Case-driven（以用户需求做为引导开发）
 + -Centered：中心，框架
 	一切软件开发的活动都围一切软件开发的活动都围绕着架构,就像盛诞节的糖果和礼物都挂在圣诞树上一样。
    > eg:Architecture-centered(圣诞书中心)

**<font color=blue> Test：</font>**
>请问: Service-Oriented Architecture(SOA)是什么涵意呢?
>软件的东西都是面向服务的

###2. 从对象(Object)谈起
* Object（对象）：世界万物所认识的东西
* Object（对象）特点：
 + 静态的： 对象之特征或属性(Attribute)
 + 动态的： 对象之行为(Behavior)
> eg: 鸟儿的特征是:有翅膀、尾巴(静态的);其行为是:唱歌、会飞等等（动态的）。
* 软件之对象(Software Object): <font color=gren> 由数据(Data)</font> 和  <font color=gren> 函数(Function)</font>所组成。

###3. 类的用途:叙述软件对象
* 自然界： 类(Class)是群体(或集合),而对象是类中的一份子。人们常用「是一个」(Is A)来表达对象与类间之关系
>eg:月亮是一个星球;毕加索是一个艺术家;张大千是一个画家..
* 软件中：类就是说明软件中之对象,应含那些数据及那些函数。 用关键字：<font color=blue> **class**</font>
>eg:代码中的定义
> ```java
     1.类的定义：
        class Rose {
            private double price; //date
            private int month;    //date
            public void say(){    //function
        		System.out.println("Color is RED.");
        		}
        }
     2. 对象的产生：
        Rose rose = new Rose();
     3.实际代码中：
        public class JMain {
            public static void main(String[] args) {
            Rose rose = new Rose();
            rose.say();
            }
         }
```

###4. <基类/子类>结构用途(一):表达继承
![](./picture/uml-.png)

###5. <基类/子类>结构用途(二):表达组合
###6. <基类/子类>结构的接口(卡榫函数)
###7. IoC机制与Default函数
###8. 主动型 vs. 被动
###9. 接口与类(别)