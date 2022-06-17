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
- /* 多行注释 */
- /**文档注释 */ 

## Java Keywords. Example: class, boolean, try... [more](https://www.w3schools.com/java/java_ref_keywords.asp)

## Datatype: 8个基本类型 & 扩展
- 8个基本类型
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

- 数据类型扩展

    - 整数拓展
    ```
    整数拓展: 进制 二进制0b, 八进制0, 十进制, 十六进制0x
    int i = 10; //十进制 return 10
    int i2 = 010; //八进制 return 8
    int i3 = 0x10; //十六进制 return 16
    ```

    - 浮点数拓展: float and double
        - **最好不用float比较**.
        - **银行业务怎么表示钱: BigDecimal (数学工具类)**
    ```
    float f = 0.1f; // 0.1
    double d = 1.0/10; //0.1
    System.out.println(f==d); // return false

    float d1 = 231313131313131313f;
    float d2 = d1+1;
    System.out.println(f==d); // return true

    // float: 有限，离散，舍入误差 大约 接近但不等于
    ```

- 字符拓展: 字符强制转换成数字
    ```
    char c1 = "a";
    System.out.println((int)c1);
    ```
- 类型转换 （Java是强类型语言）
    - 自动转换: low -> High (byte, short, char -> int -> long -> float -> double)
    - 强制转换: High -> Low (try not to do this!)
    ```
    int i = 128
    byte b = (byte) i //内存溢出

    System.out.println(i); //return 128
    System.out.println(b); //return -128, 内存溢出

    System.out.println((int)23.7); //return 23 精度问题
    ystem.out.println((int)-45.89f); //return -45 精度问题
    ```
    - **注意点**:
        - 不能对boolean进行转换
        - 不能把对象类型转换成不相干类型
        - 不能把高容量转成低容量时候，强制转换
        - 转换的时候可能存在内存溢出, 或者精度的问题