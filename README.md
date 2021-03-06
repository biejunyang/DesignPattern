# DesignPattern
Java Desgin Pattern Study
# 1、适配器模式：
  用途：把一个类的接口转换成客户所期望的另一种接口，从而使原本因接口不匹配，不能一起工作的类能在一起工作。
  举例：如生活中的电源适配器，能够将三角插座适配成我们所希望的二脚插座。

  适用场景：
    1、已经存在的类不符合我们的要求，可以用适配器适配成我们所需要的。
    2、创建一个复用类，使得该类与不先关的类或者不可预见的类一起工作，如Spring MVC中的处理适配器(HandlerAdapter)，适配我们编写的不可预见的Controller。

  适配器模式中的角色：
    1、目标角色(Target)：客户所期待的接口，可以是类或者接口，但是在类适配器中只能是接口，因为Java是单继承
    2、需要适配的角色(源角色Adaptee)：需要适配的类
    3、适配器角色(Adapter)：核心类，把原接口转换成目标接口，只能是具体类。
