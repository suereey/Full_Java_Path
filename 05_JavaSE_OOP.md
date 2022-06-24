# OOP
## Intro
- 面向对象编程的本质：以类的方式组织代码，以对象的组织（封装）数据
## 类与对象的创建
- 创建 method: 修饰符 + 返回类型 + 方法名(){}
```
public String sayHello(){
    return "hello world";
}

public void say(){
    return;
}
```

- 调用方法
```
public class Student {
    public void say(){
        System.out.println("hello");
    }
}

public class Demo02 {
    public static void main(String[] args) {
        Student student = new Student();
        student.say();
    }
}
```
- 对象是一个具体的事物，类是抽象的，而类是抽象的模板
- **类(class)与对象(object)的创建**
```
public class Student {
    //属性 attributes
    String name; //inital: null
    int age; //inital: 0
    //methods
    public void study(){
        System.out.println(this.name + "hello, i'm working");
    }
}

public class Application {
    public static void main(String[] args) {
        //类（抽象）需要实例化. 类实例化后会返回一个自己的对象！
        //student对象就是一个Student类的具体实例
        Student xiaoming = new Student();
        Student xiaohong = new Student();

        xiaoming.name = "xiaoming";
        xiaoming.age = 3;
    }
}
```

## 构造器详解
- 构造器：
    - 和类名相同
    - 没有返回值
- 作用：
    - new本质在调用构造方法
    - 初始化值对象的值

- 定义有参值后，如果想使用无参构造，显示的定义无参构造

```
public Person(){} //使用new关键字，本质是在调用构造器, 用来初始化值

//有参构造：一旦定义了有参构造，无参就必须显示定义
public Person(String name){
    this.name = name;
}

//alt+insert默认帮你生成有参构造器
```
## 创建对象内存分析
![10_Memory](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/10_ClassMethod_Memory.png)

## Summary Class vs. Object
- class是一个模板，抽象； object是一个具体的实例
- 方法：定义与调用
- 对应的引用：
    - 引用类型：基本类型（8）
    - 对象是通过引用来操作的：栈-->堆
- 属性(attributes)：字段field 成员变量
    - 默认初始化
        - 数字： 0， 0.0
        - char：u0000
        - boolean: false
        - 引用:null
        
    修饰符 属性类型 属性名= 属性值

- 对象的创建和使用
    - 必须使用new关键字创造对象，构造器 ```Pet dog = new Pet();```
    - 对象的属性: ```dog.name```
    - 对象的方法: ```dog.sleep()```
- 类
    - 静态的属性 属性
    - 动态的行为 方法
## 封装, 继承, 多态
- encapsulate
    - 提高程序安全性，保护数据
    - 隐藏代码实现的细节
    - 统一接口（get，set）
    - 提高系统的可维护性
    - Example: Private, get/set
    ![11](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/11_PrivateGetSet.png)
- inheritance
    - 子类继承了父类，就继承了父类的all public methods, and all public attribute (like ``` public int money = 10_0000_0000;```)
    - **Super keyword**
    ![12](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/12_Super.png)
- polymorphism

- Summary
![13](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/13_Override.png)
## 抽象类和接口
- abstract class
- interface: 接口都需要有实现类
```
//define interface
public interface UserService{
    void add(String name);
    void delete(String name);
    void update(String name);
    void query(String name);
}

public class UserServicImpl implements UserService{

}
```

## 内部类

# Error and Exception

