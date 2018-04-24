Summary: 头文件与类声明

Author:      Amusi

Date:          2018-04-24

# C vs C++ 关于数据和函数

C: built-in，struct —>数据和函数 —> 变量（variables）

C++: class，struct —> 数据成员（Data members）和成员函数（Member functions）—> 对象（objectes）



# C++ 关于数据和函数

![c++](https://note.youdao.com/yws/res/40232/WEBRESOURCEc233a5c08227f73c171ac52ba2c1e7f3)



# C++ 代码基本形式

1. .h（自定义头文件）
   - Classes
   - Declaration（声明）
2. .cpp
   - \#include<iostream>
   - \#include<complex.h>
     - ex.main()
3. .h（库文件）

# C++ vs C 输出

C++版本

```C++
#include <iostream.h>
// 等价于#include <iostream>
using namespace std;

int main()
{
  int i = 7;
  cout<< <<endl;
}
```

C版本

```c
#include <stdio.h>
// 等价于#include <cstdio>

int main()
{
  int i = 7;
  printf();
}
```

# 防止头文件（Header）重复包含和编译

在complex.h头文件中最前面添加预编译指令: #ifndef .. #define ..，在头文件最后添加#endif

```c++
#ifndef __COMPLEX__
#define __COMPLEX__

...
  
#endif
```

示例:

```c++
#ifndef __COMPLEX__
#define __COMPLEX__

#include <cmath>

// 前置声明（forward declarations）
class ostream;
class complex;

complex& _doapl (complex* this, const, complex& r);

// 类声明（class declarations）
class complex
{
  ...  
};

// 类定义（class definition）
complex::function .. 

#endif
```

# 类的声明

```c++
class complex
{
  public:
  	complex(double r = 0, double i =0): re(r), im(i){}
    complex
  private:
}
```

