# DAY-7.12



[TOC]



> **本课目标**

- [掌握标识符和关键字]()
- [掌握变量和常量的使用]()
- [了解Java中的数据类型]()
- [掌握数据类型的转换]()

------



## 变量

- 存储数据的空间（装数据的容器）
- 变量命名规则
  - 变量名由字母、数字、下划线_、美元符号$组成
  - 变量名不能以数字开头,不建议使用美元符号开头
  - 变量名不能使用Java关键字
  - 变量名采用小驼峰命名法
  - 变量名要做到见名知意
  - Java是严格区分大小写
- 变量在赋值后可以重新赋值

- 变量的声明
  - 数据类型	变量名；
- 变量赋值
  - 变量名	=	数据；



## 基本数据类型

### 数值型类型

- 整型数据
  - `byte、short、int、long`
- 浮点型数据
  - `float、double`



### 非数值型类型

- 字符`char`	使用单引号`''`括起来的，单引号中只能写一个中文汉字或者一个英文字符
- 布尔类型`boolean`布尔类型的变量中只能存放两个数据`true`、`false`

### 引用数据类型（3个）

- 数组、类、接口

------

### 数据类型的使用

```java
byte num1 = 1;
short num2 = 1;
int num3 = 1;
long num4 = 11342L;
float num5 = 234.2F;
double num6 =23.4 ;
char ch1 = 's';
boolean bool1 = false;
```

### 字符串类型

- ​		字符串类型的数据是引用类型数据



### 练习：输出个人信息



![image-20220713103222625](C:\Users\chenz\AppData\Roaming\Typora\typora-user-images\image-20220713103222625.png)

```java
public class 个人信息输出 {
    public static void main(String[] args) {
        float score = 98.5f;
        String name = "张三";
        char sex = '男';
        System.out.println("Java课考试最高分："+source);
        System.out.println("最高分学员姓名："+name);
        System.out.println("最高分学员性别："+sex);
    }
}
```

### 练习：输出个人简历

![image-20220713104512873](C:\Users\chenz\AppData\Roaming\Typora\typora-user-images\image-20220713104512873.png)

```java
public class 输出个人简历 {
    public static void main(String[] args) {
        String name = "小明";
        int age = 25;
        String exp = "工作了3年了\n做过5个项目\n技术方向是Java";
        String like = "篮球";
        System.out.println("这个同学的姓名是："+name);
        System.out.println("年龄是："+age);
        System.out.println(exp);
        System.out.println("兴趣爱好是："+like);
    }
}
```

## 常量

> 程序运行中，值不能改变的量称之为常量，常量使用`final`关键字

- 常量名全部使用大写字母，多个单词之间使用下划线隔开
- 常量一般在声明的时候就进行赋值
- 常量的值不能被改变
- 语法格式：
  - `final`	数据类型	=	数据；

## Scanner的使用

1. 导入Scanner类

   `import java.util.Scanner;`

2. 创建Scanner对象

   `Scanner input = new Scanner(System.in);`

3. 获得键盘输入的数据

   `int now = input.nextInt();`

#### 例子：

```java
import java.util.Scanner;
public class Scanna的使用 {
    public static void main(String[] args) {
        System.out.println("请输入数值a:");
        Scanner input = new Scanner(System.in);
        int a = input.nextInt();
        System.out.println("a的数值为："+a);
    }
}
```

