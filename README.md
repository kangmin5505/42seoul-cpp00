# 42seoul-cpp00

## Orthodox Canonical Class Form(OCCF)
In C++98 and C++03 the OCCF had four different methods that the C++ compiler is willing to generate:
- Default constructor
- Copy constructor
- Destructor
- Copy assignment operator
```cpp
class A final {
public:
  A ();
  A (const A &a);
  ~A ();
  A & operator = (const A &a);
};
```

## Namespaces
### Namespaces
A mechanism for expressing that some declarations belong together and that their names shouldn't clash with other names.
### using-declaration
A using-declaration makes a name from a namespace usalbe as if it was declared in the scope in which it appears.
```cpp
using std::cout;
```
### using-directive
A using-directive makes unqualified names from the named namespace accessible from the scope in which we placed the directive.
```cpp
using namespace std;
```
