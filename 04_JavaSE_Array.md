# 数组 (Arrays)
## 数组Intro
- 数组: **相同类型**的有序集合 (cannot mix string and numbers). 元素为相同类型, 元素可谓基本类型和引用类型
- Array has index starting from 0
- 数组长度是确定的，一旦被创建，大小不可变 (Error: ArrayIndexOutofBoudns)
- 数组变量属于引用类型 (array[0], and value store in heap)
## 数组使用
- Define array
```
int [] nums; //1. define an array (preferred)
int nums2[]; //define an array

nums = new int[10]; //2. 里面可以存放10个int类型的数字

//3. 给数组元素赋值
nums[0] = 1;
for(int i=1; i< nums.length; i++){
    nums[i] = nums[i-1] * 2;
}
System.out.println(nums[9]);
```
- **Array.length**

## 内存分析
- 堆 (heap) and 栈 (stack): 
```
//1. 定义数组 
int[] array1 = null;

//2. 创建数组
array1 = new int[10];

//3. 给数组元素赋值
array1[0] = 1;
//...
```

![09](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/09_JavaMemory.png)
![08](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/08_JavaMemory.png)

## 三种初始化状态: 静态, 动态, 默认初始化
- 数组长度是确定的，一旦被创建，大小不可变
- 元素为相同类型, 元素可谓基本类型和引用类型
- 数组变量属于引用类型 (array[0], and value store in heap)

```
int[] a = {1,2,3,4,5,6};
//动态初始化, 包含默认初始化 (inital value = 0)
int[] b = new int[10];
b[0] = 10;
```

- Iterate an array
```
int[] arrays = {1,2,3,4,5};

//iteration
for(int i = 0; i < arrays.length; i++){
    System.out.println(arrays[i]);
}

//find max
int max = arrays[0];
for(int i = 0; i< arrays.length;i++){
if (arrays[i] >max){
    max = arrays[i];
    }
}

// iteration
for (int array: arrays){
    System.out.println(array);
}
```
## 多维数组
```
int[][] array  = {{1,2}, {2,3}, {3,4}, {4,5}};
int[][] array = new int[2][4];
```

## Arrays 类
```
import java.util.Arrays; //在这个之后，就可以使用一些自带的function。比如

System.out.println(Arrays.toString(array1)); //print full array

Arrays.sort(array1); //sort array

```
