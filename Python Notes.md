### python 基础
#### IDE
      IDLE,Pycharm,wingide,eclipse
#### 注释
    单行注释 #xxxx

    多行注释
    '''
        多行注释
    '''
#### 行连接符
     使用\作为行链接符号
     a="sdfksdkjfhskd\
     dfs"
     print(a)

#### pyhton对象
     id 标识, type 类型, value 值
     a = 3;
     id(a)
     type(a)

#### 引用
     变量称之为对象的引用
     变量在栈里面
     对象在堆里面
#### 标识符
    与java 类似
    区分大小写 字母或者_开头后续字母数字下划线  避免关键字  避免双下划线（系统使用）
#### 变量赋值
    简单赋值
    a=3
    链式赋值
    a=b=3
    解包赋值
    a,b,c=1,2,3
    利用解包赋值可以进行变量值交换(不需要定义中间变量)
    如:
    a,b=1,2
    a,b=b,a
#### 常量
    python本身不支持常量
    只能通过命名来规范定义：
    用大写加下划线MAX_VALUE=100
#### 运算符
    + - *
    / 浮点数除
    // 整数除
    ** 幂运算
    divmod(x,y)   #返回商和余数
    逻辑运算符 and or not
    等值判断 == is ，注意==会判断实际的value值 is判断是否是同一个对象的地址
    和Java[-128,127]类似 Python 也会对小范围的数字进行缓存[-5,255] 如果进行is 判定的话需要特别注意
```
    >>>a=5
    >>>b=5
    >>>a is b 
    >>>True
    >>>a=800
    >>>b=800
    >>>a is b
    >>>False
 ```
#### 整数
    *进制
    0B 开头二进制
    0o 开头八进制
    0x 开头16进制
    如：0o9是错误的 八进制应该表示为0o11
    *进制转换
    int(5.4)
    python3整数大小无限制
    python2整数位32位

    0xff = 15*16^1 + 15 = 255
#### 浮点数
    float  浮点数类型
    float(2) 2.0
    float("2.1") 2.1
    科学计数法
    3.14 可表示为 314E-2或者314e-2
    round(3.5) 4 四舍五入取整
#### 字符串
    Python 和 Java 一样字符串不可变，但Python木有字符只有字符串和其他语言不一样
    1.1字符串编码
    (默认源代码文件为ascii编码)python 2 建议 定义文件编码： # -*- coding: utf-8 -*-
    在字符串前面添加 u如u'中'
    1.2python 3可以直接使用  
    >>> ord('中') #内置函数ord 查看unicode编码
    20013
    >>> chr(20013) #内置函数chr 对应的unicode转换为字符
    '中'
    2.1 使用 单引号 和双引号 字符串创建
    >>> str= "奥比岛"
    >>> str
    '奥比岛'
    >>> str='奥比岛'
    >>> str
    '奥比岛'

#### 时间
    time ,datetime,timedelta
    time.time() 返回1970-1-1到至今的秒数
    格式化时间time.strftime()
    ```
    strftime(...)
        strftime(format[, tuple]) -> string
    ```
    字符串转化为时间 time.strptime()
    ```
      strptime(...)
        strptime(string, format) -> struct_time
    ```
    时间计算 timedelta
#### 函数
##### 函数定义
    python中函数本质也是对象 可以使用  type函数查看
    使用可以做到类似重命名
    比如说：
    def f1():
        print("f1")
    f2=f1
    f2()
    #java做不了这样啊哈哈哈

##### 函数返回值
    使用return 关键字返回 如果不手动指定则默认返回 None
    等值判断 ==,is。注意==会判断实际的value值 is判断是否是同一个对象的地址
    

#### 集合元素
    tuple,list,dict,set
    #list
    li = [1,2,3] #<class 'list'>
    tp =(1,2,3)  #<class 'tuple'>
    dic = {'a':'1','b':'2'} #<class 'dict'>
    se = {1,2,3} #<class 'set'>
