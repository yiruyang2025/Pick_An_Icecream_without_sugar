# Repository_with_Liz_Lee

<br>

- draw an ice-cream (*non-rigid) here (though actually don't know what for)


<br>



## Python vs C++ Quick Syntax Cheat Sheet

| Concept                | C++ Example                               | Python Example                                                        | Key Difference                                                             |
| ---------------------- | ----------------------------------------- | --------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| **Hello World**        | `std::cout << "Hello";`                   | `print("Hello")`                                                      | Python has built-in `print()`, no headers needed                           |
| **Variable**           | `int x = 5; std::string name = "Bob";`    | `x = 5; name = "Bob"`                                                 | Python is dynamically typed (no explicit types)                            |
| **Data Types**         | `int, double, char, string, bool`         | `int, float, str, bool, list, dict, tuple`                            | Python has richer built-in data types                                      |
| **Array/List**         | `std::vector<int> v = {1,2,3};`           | `nums = [1, 2, 3]`                                                    | C++ vectors need `<vector>`, Python lists are built-in and dynamic         |
| **Map/Dictionary**     | `std::map<string,int> scores;`            | `scores = {"Alice": 90, "Bob": 85}`                                   | Python dict is built-in, syntax is shorter                                 |
| **If Statement**       | `if(x > 0) { cout << "pos"; }`            | `if x > 0:\n    print("pos")`                                         | Python uses **indentation** instead of braces                              |
| **For Loop**           | `for(int i=0;i<5;i++) cout<<i;`           | `for i in range(5): print(i)`                                         | Python loop is more concise, no index type                                 |
| **While Loop**         | `while(x > 0) { x--; }`                   | `while x > 0:\n    x -= 1`                                            | Syntax is simpler, colon + indent instead of braces                        |
| **Function**           | `int add(int a,int b){ return a+b; }`     | `def add(a, b):\n    return a + b`                                    | Python uses `def`, no return type required                                 |
| **Lambda Function**    | `auto sq = [](int x){ return x*x; };`     | `sq = lambda x: x*x`                                                  | One-liner anonymous functions are easier in Python                         |
| **Class**              | `class Dog { string name; };`             | `class Dog:\n    def __init__(self, name):\n        self.name = name` | Python classes are simpler, no header/semicolon                            |
| **Template / Generic** | `template<typename T> T max(T a,T b);`    | `def max_func(a, b): return a if a>b else b`                          | Python is inherently generic (dynamic typing), no template keywords needed |
| **Import Library**     | `#include <cmath>`                        | `import math`                                                         | Python uses `import`, no compilation step needed                           |
| **Exception**          | `try { ... } catch(exception &e) { ... }` | `try:\n    ...\nexcept Exception as e:`                               | Python uses `try/except`, no need for types unless specified               |
| **Main Entry Point**   | `int main(){ ... return 0; }`             | `if __name__ == "__main__": main()`                                   | Python doesn’t require `main()`, but conventionally uses this pattern      |
| **Compilation vs Run** | `g++ file.cpp -o prog && ./prog`          | `python3 script.py`                                                   | Python is interpreted (no compilation step)                                |


<br>

## Full-Stack Development Workflow (Python + React + Node.js)



```
User clicks button (React) →
React sends API request →
Backend (Node.js or Python) processes logic →
Backend queries database →
Backend returns JSON response →
React updates UI
```



<br>

```
+------------------+        +--------------------+        +-------------------+
|   FRONTEND       |        |   BACKEND          |        |   DATABASE        |
| (React + npm)    | <----> | (Node.js OR Python)| <----> | (SQL / NoSQL DB)  |
+------------------+        +--------------------+        +-------------------+
        |                             |                             |
        v                             v                             v
  React Components              REST / GraphQL API              Data Storage
  (UI/UX, HTML, CSS, JS/TS)     (Business Logic, Auth, etc.)    (Postgres, MongoDB...)
        |
        v
   npm (Node Package Manager)
   - installs React libraries
   - runs dev/build scripts
```

<br>

## (Timeline & Roles)

| Component    | Full Name                           | Year Introduced              | Creator(s) / Organization                                 | Motivation (Why Created)                                                                                                              | Role in Workflow (What It Does)                                                                                                                |
| ------------ | ----------------------------------- | ---------------------------- | --------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| **Python**   | Python Programming Language         | 1991                         | Guido van Rossum (Netherlands, CWI)                       | Existing languages like C/Java were too complex; wanted a **simple, readable, general-purpose language**.                             | Backend option: APIs, business logic, AI/ML, data science, web frameworks (Flask, Django, FastAPI).                                            |
| **Database** | Database Management System (DBMS)   | 1960s (concept), 1970s (SQL) | IBM (IMS, then Edgar F. Codd for relational model at IBM) | Applications needed to **store data persistently and retrieve it reliably**.                                                          | Persistence layer: stores structured/unstructured data (users, posts, transactions). Relational (PostgreSQL, MySQL) or NoSQL (MongoDB, Redis). |
| **Node.js**  | Node JavaScript Runtime Environment | 2009                         | Ryan Dahl                                                 | Traditional servers (Apache, PHP) were inefficient for **real-time, concurrent apps**. Introduced **event-driven, non-blocking I/O**. | Backend option: Serves APIs, handles requests, scalable for real-time apps (chat, streaming).                                                  |
| **npm**      | Node Package Manager                | 2010                         | Isaac Z. Schlueter                                        | JavaScript needed a **centralized dependency manager** for sharing/reusing libraries.                                                 | Package manager: installs JavaScript libraries, runs scripts (`npm start`, `npm build`).                                                       |
| **React**    | React.js (React JavaScript Library) | 2013                         | Facebook (Meta)                                           | Building dynamic UIs with plain JavaScript was hard; React introduced **component-based architecture + virtual DOM**.                 | Frontend framework: builds modular, fast user interfaces. Works with npm for dependencies.                                                     |



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




<br>

| Feature                | Example Code                                                         | Notes                                                           |
| ---------------------- | -------------------------------------------------------------------- | --------------------------------------------------------------- |
| **Python Philosophy**  | `# Python = readability + productivity`                              | Emphasizes simplicity, readability, and rapid development       |
| **Print to Console**   | `print("Hello, World")`                                              | No need for headers; built-in `print()` function                |
| **Variable**           | `x = 42` <br> `name = "Alice"`                                       | Dynamically typed, no explicit type declaration needed          |
| **Data Types**         | `int`, `float`, `str`, `bool`, `list`, `dict`, `tuple`, `set`        | Rich built-in data structures                                   |
| **List (Array)**       | `nums = [1, 2, 3]` <br> `nums.append(4)`                             | Dynamic, heterogeneous, supports slicing `nums[1:3]`            |
| **Dictionary (Map)**   | `scores = {"Alice": 90, "Bob": 85}`                                  | Key-value store, efficient lookups                              |
| **Tuple (Immutable)**  | `point = (3, 4)`                                                     | Fixed-size, immutable sequence                                  |
| **Set**                | `unique = {1, 2, 3}`                                                 | Unordered, no duplicates                                        |
| **If Statement**       | `if x > 0:\n    print("Positive")`                                   | Indentation defines blocks (no braces)                          |
| **Loop (for)**         | `for i in range(5):\n    print(i)`                                   | Iterates over sequences or ranges                               |
| **Loop (while)**       | `while x > 0:\n    x -= 1`                                           | Runs while condition is true                                    |
| **Function**           | `def add(a, b):\n    return a + b`                                   | Defined using `def`; supports default and keyword args          |
| **Lambda Function**    | `square = lambda x: x*x`                                             | Anonymous one-line functions                                    |
| **Class (OOP)**        | `class Dog:\n    def __init__(self,name):\n        self.name = name` | Object-Oriented Programming with constructors and methods       |
| **Import Module**      | `import math` <br> `from math import sqrt`                           | Supports both full and selective imports                        |
| **Exception Handling** | `try:\n    x=1/0\nexcept ZeroDivisionError:\n    print("Error")`     | Robust error handling with `try/except/finally`                 |
| **List Comprehension** | `[x*x for x in range(5)]`                                            | Concise way to create transformed lists                         |
| **File I/O**           | `with open("file.txt","r") as f:\n    data=f.read()`                 | Context manager ensures safe open/close                         |
| **f-string**           | `name="Alice"; print(f"Hello {name}")`                               | Modern string interpolation                                     |
| **Built-in Functions** | `len()`, `type()`, `sorted()`, `sum()`                               | Python provides powerful standard library functions             |
| **Assignments Rule**   | `# Use built-in + standard libraries first`                          | Implement your own logic, only use external deps when justified |




<br>


## Python CLI & REPL Quick Commands

| Command / Feature                | Example Usage                                                                 | Notes                                                           |
| -------------------------------- | ----------------------------------------------------------------------------- | --------------------------------------------------------------- |
| **Run Python Script**            | `python3 script.py`                                                           | Executes a Python file in the current directory                 |
| **Start REPL (Interactive)**     | `python3`                                                                     | Opens interactive Python shell (exit with `exit()` or `Ctrl+D`) |
| **Check Python Version**         | `python3 --version`                                                           | Shows installed Python version                                  |
| **Install Package (pip)**        | `pip install numpy`                                                           | Installs package from PyPI                                      |
| **Upgrade Package**              | `pip install --upgrade numpy`                                                 | Updates to latest version                                       |
| **List Installed Packages**      | `pip list`                                                                    | Shows all installed dependencies                                |
| **Freeze Requirements**          | `pip freeze > requirements.txt`                                               | Export environment dependencies                                 |
| **Install from Requirements**    | `pip install -r requirements.txt`                                             | Recreate environment from file                                  |
| **Virtual Environment (Create)** | `python3 -m venv venv`                                                        | Creates isolated environment                                    |
| **Activate Virtual Env**         | `source venv/bin/activate` (Linux/Mac) <br> `venv\Scripts\activate` (Windows) | Activates environment                                           |
| **Deactivate Virtual Env**       | `deactivate`                                                                  | Exit the virtual environment                                    |
| **REPL Built-in Help**           | `help(str)`                                                                   | Shows documentation for type/function                           |
| **List Object Attributes**       | `dir(list)`                                                                   | Lists all methods/attributes of object                          |
| **Check Type**                   | `type(3.14)`                                                                  | Returns object type (`float`)                                   |
| **Inspect Object**               | `vars(obj)`                                                                   | Returns object’s `__dict__` (attributes)                        |
| **Run Module as Script**         | `python3 -m http.server 8000`                                                 | Example: starts a simple HTTP server on port 8000               |
| **Run Inline Code**              | `python3 -c "print(2+2)"`                                                     | Executes one-line Python command                                |
| **Open Python File in REPL**     | `python3 -i script.py`                                                        | Runs script, then drops into interactive mode                   |



<br>

## python vs python3

Historically, many systems installed Python 2.x as python, and Python 3.x as python3.

Today:

On Linux/Mac, python3 explicitly refers to Python 3.

python may still point to Python 2 (deprecated) or be symlinked to Python 3.

On Windows, only python is usually installed (and it’s Python 3).

👉 Best Practice:
Always use python3 in commands to ensure consistency across systems.




<br>



