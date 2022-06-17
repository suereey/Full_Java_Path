# Scanner and Loop
## Scanner对象
- 通过Scanner类来获取用户的输入 (```java.util.Scanner```)
- Can use next() or nextLine()
```
import java.util.Scanner;
public class Demo01 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("accept words...");

        if (scanner.hasNext()){
            //接受用户的输入
            String str = scanner.next();
            System.out.println("the words are: " + str);
        }

        /*
        if(scanner.hasNextLine()){
            String str = scanner.nextLine();
            System.out.println("the words are: " + str);
        }
        */

        scanner.close();

    }
}
```

![04Scanner](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/04_Scanner_next.png)

## if statement
## swtich statement

```
switch (expression) {

  case value1:
    // code
    break;
  case value2:
    // code
    break;  
  default:
    // default statements
  }
```

## loop
- while loop
- do...while loop: 即使不满足，也run一次。
```
public class DoWhileDemo {
    public static void main(String[] args) {
        int i= 1;
        int sum = 0;
        do{
            sum = sum + i;
            i ++;
        }while(i < 0);
        System.out.println(sum); //print sum = 1
    }
}

``` 
- for loop
```
public static void main(String[] args) {
    for(int i=1; i<10; i++){
        System.out.println(i);
    }
}
```

``` 
int[] numbers = {1,2,3,4,5}; //定义一个数组
for(int x:numbers){ //遍历数组
  System.out.println(x);
}
```

## break, conitnue, goto