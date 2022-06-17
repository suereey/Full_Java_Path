# Java Basic
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

![04Scanner]()

## 顺序结构

## if statement

## while statement