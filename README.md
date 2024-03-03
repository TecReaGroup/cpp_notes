# cpp_notes

## C++

### comment（注释）

1. 单行注释：// comment
2. 多行注释：/\* comment \*/

### scanf

1. double: 以科学计数法表示，所以相对于long long类型可以接受更大的数，但存在精度损失（常用于阶乘和幂运算数据类型）
2. scanf返回值: “所输入的数据与格式字符串中匹配次数.”返回已成功赋值的数据项数；出错时则返回EOF.（注：EOF(End Of File)是一个预定义的常量，等于-1.）。常用方式（循环读取输入）：

```c++
while(scanf("%d %d",&a, &b) != EOF){
        //pass
    }  
```

![scanf](photos\scanf.png "scanf")

### printf

1. printf .nf: 会对最后一项四舍五入
2. printf %nd: 保留n位数多余用空格补充（右对齐）; 左对齐：%-nd。如果参数过长，以参数长度为准，不会进行截断

![printf](photos\printf.png "printf")

### memset

1. syntax：memset(array, initial_value, sizeof_array)

### sort

1. syntax: sort(array_header_adress, array_tail_adress, compare_function) //a < b reurn true -> order sorting (default); a > b return true -> reverse sorting

### Remeber

1. 循环，迭代末尾注意变量初始化
