# description: 
 Any construct that could possibly be considered a declaration is a declaration.  In this example, the second line of main is interpreted as a function declaration in preference to an object declaration with initialization.

```C++ runnable
#include <iostream>

struct Foo
{
  Foo(int d) : x(d) {}
  int x;
};

int main() 
{ 
  double x = 3.14;

  Foo f( int(x) );

  std::cout << f.x << std::endl;

  return 0;
} 
```

