# 数组 (Arrays)
## 数组Intro
- 数组: **相同类型**的有序集合 (cannot mix string and numbers)
- Array has index starting from 0
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
- 堆 (heap):
- 栈 (stack): 
``
//1. 定义数组 
int[] array1 = null;

//2. 创建数组
array1 = new int[10];

//3. 给数组元素赋值
array1[0] = 1;
//...
```
## 多维数组
## Arrays 类
## 稀疏数组