# Repository_with_Liz_Lee

<br>

draw an ice-cream (*non-rigid) here (though actually don't know what for)


<br>



| Feature              | Example Code                           | Notes                                                                  |
| -------------------- | -------------------------------------- | ---------------------------------------------------------------------- |
| **C++ Philosophy**   | `// C++ = performance + abstraction`   | Combines low-level efficiency with high-level abstractions             |
| **STL Containers**   | `std::vector<int> v = {1,2,3};`        | Dynamic array (resizable), part of the Standard Template Library (STL) |
| **STL Map**          | `std::map<string,int> scores;`         | Key-value store, automatically sorted by key                           |
| **Eigen Matrix**     | `Eigen::MatrixXd M(3,3);`              | Double-precision 3×3 matrix, supports linear algebra operations        |
| **Eigen Vector**     | `Eigen::Vector3d v(1,2,3);`            | 3D vector, useful in geometry and graphics                             |
| **Print to Console** | `std::cout << "Hello";`                | Requires `<iostream>`, prints output to standard stream                |
| **Loop (for)**       | `for(int i=0;i<n;i++) cout<<i;`        | Classic C++ loop for iteration                                         |
| **Function**         | `int add(int a,int b){ return a+b; }`  | Functions can be inline or declared in headers                         |
| **Class (OOP)**      | `class MyClass { ... };`               | Encapsulation, Object-Oriented Programming (OOP)                       |
| **Template**         | `template<typename T> T max(T a,T b);` | Generic programming → write once, reuse with any type                  |
| **Assignments Rule** | `// Use STL + Eigen only`              | Implement your own logic, no non-standard dependencies allowed         |


<br>


| Category              | Syntax Example                                                                       | Explanation                                                                 |
| --------------------- | ------------------------------------------------------------------------------------ | --------------------------------------------------------------------------- |
| **Program Structure** | `cpp<br>#include <iostream><br>using namespace std;<br>int main() { return 0; }<br>` | Every C++ program starts with `main()`. `#include` imports libraries.       |
| **Variables**         | `int x = 5; double pi = 3.14; bool flag = true; char c = 'A';`                       | Basic data types: integers, floating point, boolean, character.             |
| **Strings**           | `std::string name = "Alice";`                                                        | Use `<string>` library. STL `string` supports concatenation and substrings. |
| **Constants**         | `const double g = 9.81;`                                                             | Value cannot change after initialization.                                   |
| **Input / Output**    | `cin >> x; cout << x << endl;`                                                       | `cin` reads input, `cout` prints output. `endl` = newline.                  |
| **If / Else**         | `cpp<br>if (x > 0) cout<<"Positive";<br>else cout<<"Non-positive";<br>`              | Conditional branching.                                                      |
| **Switch**            | `cpp<br>switch(op) { case '+': ... break; default: ...; }<br>`                       | Multi-way branching based on an integer/char value.                         |
| **For Loop**          | `for(int i=0; i<10; i++) cout<<i;`                                                   | Classic iteration loop.                                                     |
| **While Loop**        | `while(x > 0) { x--; }`                                                              | Loop continues as long as condition is true.                                |
| **Do-While Loop**     | `do { x--; } while(x > 0);`                                                          | Executes at least once before checking condition.                           |
| **Arrays**            | `int arr[5] = {1,2,3,4,5};`                                                          | Fixed-size collection of same-type elements.                                |
| **STL Vector**        | `std::vector<int> v = {1,2,3}; v.push_back(4);`                                      | Dynamic array that can grow/shrink.                                         |
| **STL Map**           | `std::map<string,int> scores; scores["Alice"]=90;`                                   | Key-value container (sorted by key).                                        |
| **Functions**         | `cpp<br>int add(int a,int b){return a+b;}<br>`                                       | Functions group reusable logic.                                             |
| **Pass by Reference** | `void square(int &n){ n *= n; }`                                                     | `&` allows modifying caller’s variable directly.                            |
| **Default Arguments** | `int add(int a,int b=5){ return a+b; }`                                              | Parameter `b` defaults to 5 if not provided.                                |
| **Overloading**       | `int add(int a,int b); double add(double a,double b);`                               | Same function name, different parameter types.                              |
| **Classes**           | `cpp<br>class Student {<br>public:<br> string name;<br> void print();<br>};<br>`     | User-defined types with attributes + methods.                               |
| **Constructor**       | `Student(string n) : name(n) {}`                                                     | Special function to initialize class objects.                               |
| **Destructor**        | `~Student(){ cout<<"Destroyed"; }`                                                   | Called automatically when object is destroyed.                              |
| **Access Specifiers** | `public`, `private`, `protected`                                                     | Control access to class members.                                            |
| **Inheritance**       | `class GradStudent : public Student { ... };`                                        | Derive one class from another.                                              |
| **Polymorphism**      | `virtual void speak();`                                                              | Allows overriding in derived classes.                                       |
| **Templates**         | `template<typename T> T max(T a,T b){ return (a>b?a:b); }`                           | Generic programming, reusable for many types.                               |
| **Namespaces**        | `namespace math { int add(int a,int b); }`                                           | Avoids naming conflicts, groups functions logically.                        |
| **Pointers**          | `int* p = &x; cout<<*p;`                                                             | Store memory address of variables, `*` dereferences.                        |
| **References**        | `int& ref = x;`                                                                      | Alternative name (alias) for a variable.                                    |
| **Dynamic Memory**    | `int* p = new int(10); delete p;`                                                    | Manual allocation (`new`) and deallocation (`delete`).                      |
| **Smart Pointers**    | `std::unique_ptr<int> p = make_unique<int>(10);`                                     | RAII memory management (no manual `delete`).                                |
| **Exceptions**        | `cpp<br>try { throw 1; }<br>catch(int e){ cout<<e; }<br>`                            | Structured error handling.                                                  |
| **Preprocessor**      | `#define PI 3.14` or `#include <cmath>`                                              | Preprocessing directives (before compilation).                              |
| **Comments**          | `// single line` or `/* multi-line */`                                               | Non-executable notes inside code.                                           |




<br><br>



