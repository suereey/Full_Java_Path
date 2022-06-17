# Java Intro

## JDK, JRE, JVM
- JDK: java Development Kit
    - JRE: Java Runtime Environment
        - JVM: Java Virtual Machine
## Hello World in Java
- Build a file with name, Hello.java

    ```
    public class Hello{
        public static void main(String[] args){
            System.out.print("Hello World!");
        }
    }
    ```

- In Command Prompt:

    ```
    javac Hello.java //编译javac java文件会生成一个class文件
    java Hello //run the Hello class in java
    ```

## Java注释
- //单行注释
- /*多行注释*/
- /**文档注释 */ 

## Java Keywords. Example: class, boolean, try... [more](https://www.w3schools.com/java/java_ref_keywords.asp)

## Datatype

```
//整数
int num1 = 10;
byte num2 = 20;
short num3 = 30;
long num4 = 30L; //long 类型后面要加L

//小数:浮点数
float num5 = 50.1F; //float 类型后面要加F
double num6 = 3.141592653589;

//字符
char name = "A";

//字符串, String不是关键字（key word）
//String namea = "ABCD"

boolean flag1 = true;
boolean flag2 = false;

```

![03](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/03_datatypes.png)
![02](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/02_datatypes.png)
