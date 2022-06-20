# Method
## 方法的定义和调用
- Example
```
public class Demo01 {
    //main方法
    public static void main(String[] args) {
        int add = add(1,2);
        System.out.println(add);
    }
    //add method
    public static int add(int a, int b){
        return a+b;
    }

}

```
## overload
## 命令行传递参数
## 可变参数
![07](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/07_Methods_parameters.png)
## 递归, rescursion
- 前阶段 -> 边界条件 ->返回阶段
- java栈计算，递归容易导致内存不够，内存崩溃
- Example: calculate x!. Such as 6!
    ```
    public class Demo04 {
        public static void main(String[] args) {
            System.out.println(f(6));
        }
        public static int f(int n){
            if (n==1){
                return 1;
            }else{
                return n*f(n-1);
            }
        }
    }
    ```
