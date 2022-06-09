# Java Intro

## JDK, JRE, JVM
- JDK: java Development Kit
    - JRE: Java Runtime Environment
        - JVM: Java Virtual Machine
## Hello World in Java: Build a file with name, Hello.java
    ```
    public class Hello{
        public static void main(String[] args){
            System.out.print("Hello World!");
        }
    }
    ```

    ```
    //In Command Prompt:
    javac Hello.java //编译javac java文件会生成一个class文件
    java Hello //run the Hello class in java
    ```