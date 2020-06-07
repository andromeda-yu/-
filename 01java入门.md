### java的特点
1、面向对象编程   
2、字节码方式运行在虚拟机上   
3、简单、安全、健壮   
4、跨平台   

### java基本数据类型
整数类型 long int short byte   
浮点类型 double float   
布尔类型 boolean   
字符类型 char   

### java输入输出语句
输入：   
```java
import java.util.Scanner;
Scanner scanner = new Scanner(System.in);
String name = scanner.nextLine();
int age = scanner.nextInt();
```
输出：
```java
System.out.print("Hello");
System.out.println("World");
```
格式化输出：
```java
final double PI = 3.1415926;
System.out.printf("PI = %.2f"\n, PI);
System.out.printf("PI = %7.2f\n", PI); //输出小数点后两位，整数部分+小数点+小数部分共7位
```

### 条件判断
```java
double a = 1 - 9/10.0;
System.out.println(a == 0.1); //浮点数的判断不精确
System.out.println(Math.abs(a-0.1)<0.00001); //使用距离判断
String b = "Hello";
System.out.println(b=="Hello"); //判断是否指向同一个引用
System.out.println("Hello".equals(b)); //判断内容是否相同

//switch语句，尽量少使用
switch(option){
case 1:
    System.out.println("case 1");
    break;
case 2:
case 3:
    System.out.println("case 2");
    break;
default:
    System.out.println("default");
}
```

### 数组
```java
int[] ns = {1,2,3,4,5};
System.out.println(Arrays.toString(ns)); //打印数组变量
Arrays.sort(ns); //数组排序
int[][] arr = {{1,2,3}, {4,5}};
System.out.println(Arrays.deepToString(arr)); //打印多维数组
```
