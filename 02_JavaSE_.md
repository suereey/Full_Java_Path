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

![04Scanner](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/04_Scanner_next.png)

## if statement
## Swtich

```
switch (expression) {

  case value1:
    // code
    break;
  
  case value2:
    // code
    break;
  
  ...
  ...
  
  default:
    // default statements
  }
```

## while statement
## DOwhile statement