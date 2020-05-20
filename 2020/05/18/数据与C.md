## 分类
### 整数类型
```
#includ <stdio.h>
int main (){

    int num;//声明变量num
    int num1,num2;//声明变量num1 num2
    num=1;//赋值
    num1 =2;
    num2 =3;
    //先声明在赋值
    //scanf 输入函数
    //为防止溢出 使用scanf_s 安全
    //scanf_s("%d",num,10) 需要限制长度
    int num4;
    scanf_s("%d",num4,10)
    return 0;
}
```
## 进制 (10 代表向前进一位)
//二进制 0 1 10
//八进制 0 1 2 3 4 5 6 7 10
//十进制 0 1 2 3 4 5 6 7 8 9 10
//十六进制 0 1 2 3 4 5 6 7 8 9 A B C D E F 10
#### 如何在c程序中打印出各进制的值
八进制使用%o取值 十进制使用%d 十六进制使用%x
```
printf("num的8进制：%o,10进制：%d,16进制：%x", num,num,num);
```
+ int 32位
+ short int 16位 short不长于int
输出使用 %hd %ho %hx
+ long int 32位 不短于int
输出使用%ld %lo %lx
+ long long int 64位
%lld %llo %llx
+ unsiged 无符号 意思差不多是没有前面的符号 只有数字 正数
unsiged int
## 字符类型
char 表示字符类型 理论上占8位
使用ascii时足够 但是中文中不行 所以使用万国码 unicode（16位 32位）
```
char name='a';
char name1;
scanf("%c",&name1); 
//char name= "A"; 错误 单引号代表字符 双引号代表字符串
```
## 浮点类型
float 单精度浮点型  32位
double 双精度浮点型 64位
long double 长精度浮点型 不经常用
浮点寄存器无法精确存储
## 布尔类型 bool
bool a =0；
布尔类型只可以表示0或者1 0代表false 1代表true 假或真


