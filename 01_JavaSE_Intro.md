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

## Java Keywords
- Example: class, boolean, try, catch... [more](https://www.w3schools.com/java/java_ref_keywords.asp)

## Datatype
![03]()
![02]()

```
//整数
int num1 = 10;
byte num2 = 20;
short num3 = 30;
long num4 = 30L; //long 类型后面要加L
```