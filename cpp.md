
# Table of Contents

1.  [C++ Basics](#org0e33789)
    1.  [Objects and Variables](#orge453bc6)
        1.  [Variable assigment](#org50b3ea6)
        2.  [maybe unused](#orgca9d818)
        3.  [cout and cin](#orgab5fe6a)
        4.  [Uninitialized variables and undefined behavioure](#orgaef4985)
        5.  [Keywords and Identifiers](#orgbd6ce48)
    2.  [Functions and Files](#org1baa9ac)
        1.  [Void functions](#orgd93ce26)
    3.  [size<sub>t</sub> link to topic](#org887f85f)
    4.  [Char(ASCII TABLE LINK) here](#orgf2aed50)
    5.  [Implicit and Explicit Coversion](#org1ea68cb)
        1.  [Sign conversion using static<sub>cast</sub>](#orgf33e80c)
        2.  [Quiz Questions](#org1218f2a)
2.  [Fundamental Data Types](#orgcd15f4d)
    1.  [Numeral Systems (decimal, binary, hexadecimal)](#org7e4be16)
        1.  [Octal](#orgb307271)
        2.  [hexadecimal](#org460a94d)
        3.  [Binary](#orgbe2f71a)
        4.  [Outputting values in decimal, octal and hexadecimal](#org30b8841)
        5.  [Outputting values in Binary using std::bitset](#orgeab48e5)
3.  [Strings](#org0a84f01)
    1.  [Strings (std::string)](#orge975a43)
    2.  [Strings (std::string<sub>view</sub>)](#org8eb33a0)
    3.  [some functions](#orgec5ec41)
4.  [Operators](#orgde15f65)
5.  [Bit Manipulation](#org06ce963)
    1.  [Uses of <bitset> library](#org6ece0f8)
    2.  [Bitmanipulation by bit masks](#org5f8b0be)
6.  [Namespace and scope resolution](#org9f8b3da)
    1.  [Static local variables](#org42d5974)
7.  [Control Flow](#org6d9cbc1)
    1.  [Switch case](#org0d31cfc)
    2.  [goto statements](#org4d7b3ed)
    3.  [While loop](#org9be293f)
    4.  [Do While](#org6919d50)
    5.  [For Loop](#org5a9740d)
    6.  [std::exit](#orgf60e0d8)
8.  [Mersenne Twister](#org938ad45)
9.  [Function Templates](#org08d55ae)
10. [Constexpr and Consteval Functions](#orgc717479)
11. [Compound data types](#org02f6401)
    1.  [L-value references](#org6c01415)
        1.  [Non-const L value references](#org7f36f3b)
        2.  [Const L-value referencs](#org3eeae32)
    2.  [R-value refernces](#org04734c5)
    3.  [Pass by reference](#org785286b)
    4.  [pass by const lvalue reference](#org99f66fc)
    5.  [why prefer std::string<sub>view</sub> to const std::string&](#orgb3974fa)
    6.  [Pointers](#org714cb1e)
        1.  [Deference operator](#org0c107a1)
        2.  [Pointer](#orgfc4bf6a)
        3.  [Address of operator returns a pointer](#orgdb95fca)
        4.  [null pointers as boolean values](#org604b07d)
        5.  [pointer to const](#org4b23354)
        6.  [pass by address](#orgf8e7a6d)
    7.  [Operator overloading](#org6ebbbd1)
    8.  [Enumerations](#org50a2f89)
        1.  [Unscoped Enumerations](#org2450862)
        2.  [scoped Enumerations](#org2eae6eb)
    9.  [Struct](#org594122a)
    10. [Classes (OOP)](#org02b3681)
        1.  [member functions](#org401926f)
        2.  [returning data members by lvalue reference](#orgebe18e4)
        3.  [constructor](#org3c405f9)
        4.  [temporary object](#org62b12fa)
        5.  [delegating constructor](#org7869046)
        6.  [copy constructor](#org59502b6)
        7.  [pass by value and copy construtor](#org525606e)
        8.  [array of object](#org329339b)
        9.  [Copy elison](#orgd4bde7a)
        10. [User defined conversions](#org23b16ec)
        11. [constexpr member functions](#orgc376490)
        12. [the hidden this pointer](#org91237f6)
        13. [member function chaining using \*this](#orgcc83b19)
        14. [Destructor](#org90a745e)
        15. [static member variables and functions](#org71c4df7)
        16. [friend non-member functions](#org2fd4aff)
        17. [friend class and friend member function](#orgc6f0f79)
12. [Dynamic arrays](#orga2f1a21)
    1.  [Introduction to std::vector](#org7e7787f)
        1.  [passing a std::vector using generic template or abbreviated function template](#orgf29fb74)
        2.  [move semantics](#orgee2d0ea)
        3.  [arrays and loop](#org853d377)
        4.  [template arrays and loop](#org4cd926f)
    2.  [Range based for Loops](#org4183a9d)
    3.  [Using unscoped emumerators for indexing](#org5d7830a)
    4.  [resizing std::vector at runtime](#orge1f7f22)
        1.  [length and capacity](#org5e8dc7c)
        2.  [shrink<sub>to</sub><sub>fit</sub>](#org55fde8f)
    5.  [std::vector and stack behaviour](#orged70e85)
    6.  [reserve member function](#org94720fc)
    7.  [std::vector<bool>](#orgc9277c6)
    8.  [Quiz questions](#org0e6f5dc)
    9.  [std::arrays](#org0cb0fe8)
13. [Iterators](#orgbd1b873)
14. [Introduction to standard library algorithms](#org1b7014c)
    1.  [std::find - find an element by value](#org3b11276)
    2.  [std::find<sub>if</sub> - find an element that matches some condition](#org948589b)
    3.  [std::count and std::count<sub>if</sub> to count how many occurences there are](#org0374628)
    4.  [std::sort](#org3e5bec5)
    5.  [std::for<sub>each</sub>](#orgc7e1e35)
15. [Dynamic memory allocation with new and delete](#orgc83e858)
    1.  [new](#org38daea4)
    2.  [delete](#org8005a8b)
16. [Dynamically allocating arrays](#org392c459)
17. [Destructor indetail](#orgdf12888)
18. [RAII link](#orgb884f31)
19. [Introduction to Lamdas (anonymous functions)](#org11e3be1)
    1.  [Generic Lamdas](#org2c9569a)
20. [Operator overloading.](#org519ff62)
    1.  [opearator overloading using friend function\*](#org3fd0522)
    2.  [overloading operator using normal functions](#org3668b9a)
    3.  [overloading I/O operators](#orgadb4f89)
    4.  [overloading operators using member function](#orgb7e8457)
    5.  [overloading unary operators +,-,!](#orgca2a2d7)
    6.  [overloading comparison operators](#orgccdd612)
    7.  [overloading operator[]](#org27dd1d7)
    8.  [shallow vs deep copying](#org2ed8f47)
21. [Smart pointers](#orgc7ea5c6)
    1.  [move semantics](#org7096705)

filetags: CPP


<a id="org0e33789"></a>

# C++ Basics


<a id="orge453bc6"></a>

## Objects and Variables

In C++ direct memory access is discouraged. So we use objects for that.
Instead of telling go get the value stored in mailbox number 7532, we tell go get the value stored by this object.
So that the compiler can figure it out how to retrive the value

Variable

Memory is allocated during the run time.

    #include <iostream>
    
    int main() {
    
        int x;
    
        return 0;
    }


<a id="org50b3ea6"></a>

### Variable assigment

    #include <iosteam>
    using namespace std;
    int main() {
        int x {5};
        cout << x;
        return 0;
    }

    int a;         // default-initialization (no initializer)
    
    // Traditional initialization forms:
    int b = 5;     // copy-initialization (initial value after equals sign)
    int c ( 6 );   // direct-initialization (initial value in parenthesis)
    
    // Modern initialization forms (preferred):
    int d { 7 };   // direct-list-initialization (initial value in braces)
    int e {};      // value-initialization (empty braces)


<a id="orgca9d818"></a>

### maybe unused

    #include <iostream>
    
    int main()
    {
        [[maybe_unused]] double pi { 3.14159 };  // Don't complain if pi is unused
        [[maybe_unused]] double gravity { 9.8 }; // Don't complain if gravity is unused
        [[maybe_unused]] double phi { 1.61803 }; // Don't complain if phi is unused
    
        std::cout << pi << '\n';
        std::cout << phi << '\n';
    
        // The compiler will no longer warn about gravity not being used
    
        return 0;
    }


<a id="orgab5fe6a"></a>

### cout and cin

    #include <iostream>
    using namespace std;
    int main() {
        int x{},y{};
        cin >> x >> y;
        cout << x << " " <<  y << '\n';
        return 0;
    }

    #include <iostream>
    using namespace std;
    int main() {
        int x{};
        cin >> x;
    
        int y{};
        cin >> y;
    
        cout << x << " " << y << "\n";
        return 0;
    }

    #include <iostream>  // for std::cout and std::cin
    
    int main()
    {
        std::cout << "Enter a number: "; // ask user for a number
        int x{}; // define variable x to hold user input
        std::cin >> x; // get number from keyboard and store it in variable x
        std::cout << "You entered " << x << '\n';
    
        return 0;
    }


<a id="orgaef4985"></a>

### Uninitialized variables and undefined behavioure

Returns garbage value -&#x2014;> Memory address

    #include <iostream>
    
    int main() {
        int x;
        std::cout << x << '\n';
        return 0;
    }


<a id="orgbd6ce48"></a>

### Keywords and Identifiers

List of 92 keywords

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">Keyword</th>
<th scope="col" class="org-left">Keyword</th>
<th scope="col" class="org-left">Keyword</th>
<th scope="col" class="org-left">Keyword</th>
</tr>
</thead>
<tbody>
<tr>
<td class="org-left">alignas</td>
<td class="org-left">const<sub>cast</sub></td>
<td class="org-left">int</td>
<td class="org-left">static<sub>assert</sub></td>
</tr>

<tr>
<td class="org-left">alignof</td>
<td class="org-left">continue</td>
<td class="org-left">long</td>
<td class="org-left">static<sub>cast</sub></td>
</tr>

<tr>
<td class="org-left">and</td>
<td class="org-left">co<sub>await</sub></td>
<td class="org-left">mutable</td>
<td class="org-left">struct</td>
</tr>

<tr>
<td class="org-left">and<sub>eq</sub></td>
<td class="org-left">co<sub>return</sub></td>
<td class="org-left">namespace</td>
<td class="org-left">switch</td>
</tr>

<tr>
<td class="org-left">asm</td>
<td class="org-left">co<sub>yield</sub></td>
<td class="org-left">new</td>
<td class="org-left">template</td>
</tr>

<tr>
<td class="org-left">auto</td>
<td class="org-left">decltype</td>
<td class="org-left">noexcept</td>
<td class="org-left">this</td>
</tr>

<tr>
<td class="org-left">bitand</td>
<td class="org-left">default</td>
<td class="org-left">not</td>
<td class="org-left">thread<sub>local</sub></td>
</tr>

<tr>
<td class="org-left">bitor</td>
<td class="org-left">delete</td>
<td class="org-left">not<sub>eq</sub></td>
<td class="org-left">throw</td>
</tr>

<tr>
<td class="org-left">bool</td>
<td class="org-left">do</td>
<td class="org-left">nullptr</td>
<td class="org-left">true</td>
</tr>

<tr>
<td class="org-left">break</td>
<td class="org-left">double</td>
<td class="org-left">operator</td>
<td class="org-left">try</td>
</tr>

<tr>
<td class="org-left">case</td>
<td class="org-left">dynamic<sub>cast</sub></td>
<td class="org-left">or</td>
<td class="org-left">typedef</td>
</tr>

<tr>
<td class="org-left">catch</td>
<td class="org-left">else</td>
<td class="org-left">or<sub>eq</sub></td>
<td class="org-left">typeid</td>
</tr>

<tr>
<td class="org-left">char</td>
<td class="org-left">enum</td>
<td class="org-left">private</td>
<td class="org-left">typename</td>
</tr>

<tr>
<td class="org-left">char8<sub>t</sub></td>
<td class="org-left">explicit</td>
<td class="org-left">protected</td>
<td class="org-left">union</td>
</tr>

<tr>
<td class="org-left">char16<sub>t</sub></td>
<td class="org-left">export</td>
<td class="org-left">public</td>
<td class="org-left">unsigned</td>
</tr>

<tr>
<td class="org-left">char32<sub>t</sub></td>
<td class="org-left">extern</td>
<td class="org-left">register</td>
<td class="org-left">using</td>
</tr>

<tr>
<td class="org-left">class</td>
<td class="org-left">false</td>
<td class="org-left">reinterpret<sub>cast</sub></td>
<td class="org-left">virtual</td>
</tr>

<tr>
<td class="org-left">compl</td>
<td class="org-left">float</td>
<td class="org-left">requires</td>
<td class="org-left">void</td>
</tr>

<tr>
<td class="org-left">concept</td>
<td class="org-left">for</td>
<td class="org-left">return</td>
<td class="org-left">volatile</td>
</tr>

<tr>
<td class="org-left">const</td>
<td class="org-left">friend</td>
<td class="org-left">short</td>
<td class="org-left">wchar<sub>t</sub></td>
</tr>

<tr>
<td class="org-left">consteval</td>
<td class="org-left">goto</td>
<td class="org-left">signed</td>
<td class="org-left">while</td>
</tr>

<tr>
<td class="org-left">constexpr</td>
<td class="org-left">if</td>
<td class="org-left">sizeof</td>
<td class="org-left">xor</td>
</tr>

<tr>
<td class="org-left">constinit</td>
<td class="org-left">fnline</td>
<td class="org-left">static</td>
<td class="org-left">xor<sub>eq</sub></td>
</tr>
</tbody>
</table>


<a id="org1baa9ac"></a>

## Functions and Files

    #include <iostream>
    
    int returnvalue()
    {
        int a;
        std::cin >> a;
        return a;
    }
    
    int main()
    {
        int num { returnvalue() };
    
        std::cout << num << '\n';
    
        return 0;
    }


<a id="orgd93ce26"></a>

### Void functions

    #include <iostream>
    
    void printHi()
    {
        std::cout << "Hi" << '\n';
    }
    
    int main() {
    
        //printHi();
        std::cout << printHi() << '\n';
        return 0;
    }

    #include <iostream>
    
    int main() {
    
        unsigned short a{0};
        std::cout << a << '\n';
    
        a = -4;
        std::cout << a << '\n';
    
        return 0;
    }


<a id="org887f85f"></a>

## size<sub>t</sub>[ link to topic](https://www.learncpp.com/cpp-tutorial/fixed-width-integers-and-size-t/)


<a id="orgf2aed50"></a>

## Char(ASCII TABLE LINK) [here](https://www.learncpp.com/cpp-tutorial/chars/)

    #include <iostream>
    
    int main() {
        char grade{65};
        std::cout << grade << '\n';
        return 0;
    }

    #include <iostream> //
    
    int main() {
    
        char grade {};
    
        std::cin >> grade;
    
        std::cout << grade << '\n';
    
        return 0;
    }


<a id="org1ea68cb"></a>

## Implicit and Explicit Coversion

Implicit conversion are made by compilers whereas explicit are made manually

Syntax for Exclipit conversion -&#x2014;> static<sub>cast</sub><new<sub>type</sub>>(expression)

    #include <iostream>
    
    int main() {
    
        double a{65.5};
    
        std::cout << a << '\n';
    
        std::cout << static_cast<int>(a) << '\n';
    
        std::cout << static_cast<char>(a) << '\n';
    
        std::cout << static_cast<float>(a) << '\n';
        return 0;
    }


<a id="orgf33e80c"></a>

### Sign conversion using static<sub>cast</sub>

    #include <iostream>
    
    int main() {
    
        int x{-1};
    
        unsigned int y {static_cast<unsigned int>(x)};
    
        std::cout << y << '\n';
    
        unsigned int u {4294967295}; //here 4294967295 is largest 32bit unsigned int
    
        std::cout << static_cast<signed int>(u);
    
        return 0;
    }

    #include <iostream>
    
    int main() {
        char a {};
    
        std::cin >> a;
    
        int b = a;
    
        std::cout << "You entered " << a << "," << "which has ACCII code " << b << '\n'; // OR use static_cast<int>(a) instead of another variable
    
        return 0;
    }


<a id="org1218f2a"></a>

### Quiz [Questions](https://www.learncpp.com/cpp-tutorial/chapter-4-summary-and-quiz/)

Q2.

    #include <iostream>
    
    int main() {
        double x,y;
        char c;
        std::cin >> x >> y;
        std::cout << "Enter +, -, *, /: " << '\n';
        std::cin >> c;
    
        if(c == '+') {
            std::cout << x+y << '\n';
        }else if (c == '-'){
            std::cout << x-y << '\n';
    
        }else if (c == '*'){
            std::cout << x*y << '\n';
        }else if (c == '/'){
            std::cout << x/y << '\n';
        }else {
            std::cout << "" << '\n';
        }
    
    
        return 0;
    }

Q3.

    #include <iostream>
    using namespace std;
    
    int main() {
        double height{};
        cout << "Enter the height of the tower in meters: ";
        cin >> height;
    
        double new_height{height};
    
        for(int i=0;new_height > 0;i++) {
            double distance_fallen = 9.8 * (i*i) /2.0;
    
           new_height = height - distance_fallen;
    
           if(new_height < 0) {
               cout << "At " << i << " seconds, " << "the ball is on the ground" << '\n';
               break;
           }
           cout << "At " << i << " seconds, " << "the ball is at height: " << new_height << " meters" << '\n';
    
    
        }
    
        return 0;
    }


<a id="orgcd15f4d"></a>

# Fundamental Data Types


<a id="org7e4be16"></a>

## Numeral Systems (decimal, binary, hexadecimal)


<a id="orgb307271"></a>

### Octal

In octal there are no 8 and 9.
So 8 is represented as 10 and
9 - 11
10 - 12
15 - 17
16 - 20
17 - 21 and so on

For representing it as octal number we use &ldquo;0&rdquo; infront of the number

    #include <iostream>
    using namespace std;
    
    int main() {
        int x{017};
        cout << x << '\n';
        return 0;
    }


<a id="org460a94d"></a>

### hexadecimal

Hexadecimal base is 16 and we count like  0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F, 10, 11, 12, …
To use hexadecimal we use prefix &ldquo;0x&rdquo;

    #include <iostream>
    using namespace std;
    
    int main() {
        int x{0xF};
        int y{0x1A}; //here 1A in hexadecimal means 26 in decimal
        cout << x << '\n';
        cout << y << '\n';
        return 0;
    }


<a id="orgbe2f71a"></a>

### Binary

Binary has base 2.
We use prefix 0b for binary numbers

    #include <iostream>
    using namespace std;
    
    int main() {
        int x{0101}; //octal
        int y{0x101}; //hexadecimal
        int z{0b101}; //binary
    
        cout << x << '\n';
        cout << y << '\n';
        cout << z << '\n';
        return 0;
    }


<a id="org30b8841"></a>

### Outputting values in decimal, octal and hexadecimal

    #include <iostream>
    using namespace std;
    
    int main() {
        int x{44};
    
        cout << hex << x << '\n';
        cout << oct << x << '\n';
        cout << dec << x << '\n';
        cout <<  x << '\n';
    
        return 0;
    }


<a id="orgeab48e5"></a>

### Outputting values in Binary using std::bitset

    #include <iostream>
    #include <bitset>
    
    using namespace std;
    
    int main() {
        bitset<4> x {5};
        bitset<8> y {20};
        bitset<8> z {0xF}; //decimal 15
    
        cout << x << '\n';
        cout << y << '\n';
        cout << z << '\n';
        return 0;
    }


<a id="org0a84f01"></a>

# Strings


<a id="orge975a43"></a>

## Strings (std::string)

The header <string> helps to input and output strings of different size

    #include <iostream>
    using namespace std;
    
    int main() {
        string name {"Shiva"};
        cout << name << '\n';
    
        name = "Prasad37";
        cout << name << '\n';
    
        return 0;
    }


<a id="org8eb33a0"></a>

## Strings (std::string<sub>view</sub>)

-   string<sub>view</sub> is used for reading a string in a more cleaner way.
-   Instead of creating a copy of string again where required like std::string.
-   It just points to the original data.

-   For modifies and chaning the original string value -&#x2014; std::string
-   For viewing the data in the string -&#x2014; std::string<sub>view</sub>

For using string<sub>view</sub> we have to use <string<sub>view</sub>> header file

    #include <iostream>
    #include <string>
    #include <string_view>
    using namespace std;
    
    void string_View(string_view x) {  // here no copy is made it just points to original data
        cout << x << '\n';
    
        //string z {"Kyaram"};    Doesnt work here
        //x += z;
        //cout << x << '\n';
    }
    
    void String(string y) {  //here it creates the copy so we can modify the contents here
        cout << y << '\n';
    
        string z {"Kyaram"};
        y += z;
        cout << y << '\n';
    }
    
    int main() {
        string name {"Shivaprasad"};
    
        string_View(name);
    
        String(name);
    
        return 0;
    }

Example

    #include <iostream>
    #include <string>
    #include <string_view>
    using namespace std;
    
    int main() {
    
        string name {"Shiva"};
        string_view name1 {name};
    
        cout << name1 << '\n';
    
        name1 = "Kyaram";
        cout << name1 << '\n';
    
        cout << name << '\n';
    
        return 0;
    }


<a id="orgec5ec41"></a>

## some functions

    #include <iostream>
    using namespace std;
    
    int main() {
        string name = "Shiva";
        cout << name.front();
        cout << name.back();
    
        const char* ptr = name.c_str();
    
        cout << *ptr << '\n';
        ptr++;
        cout << *ptr << '\n';
    
        name.reserve(100);
        cout << name.capacity()<< '\n';
    
        name.shrink_to_fit();
        cout << name.capacity() << '\n';
    
        name.resize(20); //pad with \0;
        name.resize(15, '!'); //pad with !
        name.resize(3); //trancate
    
    
        string s = "Hello";
        cout << s.substr(1,3)<<'\n';
        cout << s.substr(1) << '\n';
    
        string h = "Hello world";
        size_t pos = h.find_first_of("aeiou"); //any vowel
        size_t pos1 = h.find_first_not_of("aeiou"); //any vowel
        cout << pos << '\n';
        cout << pos1 << '\n';
    
        string str = "hello hello";
        size_t start = 0;
        while((pos = str.find("o",start)) != string::npos) {
            cout << pos << " ";
            start = pos +1;
        }
        cout << '\n';
    
        string hi = "Hello world!";
        hi.replace(7,4, "hehe");
    
        // auto start = hi.begin(); //same result
        // auto end = start + 5;
        cout << hi  << '\n';
        return 0;
    }


<a id="orgde15f65"></a>

# Operators

[Operator Precedence table](https://www.learncpp.com/cpp-tutorial/operator-precedence-and-associativity/)

Exponent

    #include <iostream>
    #include <cmath>
    
    int main() {
        int x{2};
        std::cout << std::pow(x,2) << '\n';
        return 0;
    }


<a id="org06ce963"></a>

# Bit Manipulation


<a id="org6ece0f8"></a>

## Uses of <bitset> library

It has

1.  test()
2.  set()
3.  reset()
4.  flip()

    #include <iostream>
    #include <bitset>
    using namespace std;
    
    int main() {
        bitset<8> bits{0b0000'0101};
    
        cout << bits << '\n';
        cout << bits.test(2) << '\n';
        bits.set(1);
        cout << bits << '\n';
        bits.reset(0);
        cout << bits << '\n';
        bits.flip(0);
        cout << bits << '\n';
    
        return 0;
    }

[Quiz](https://www.learncpp.com/cpp-tutorial/bitwise-operators/)

    #include <bitset>
    #include <iostream>
    
    // "rotl" stands for "rotate left"
    std::bitset<4> rotl(std::bitset<4> bits)
    {
        if(bits.test(3) == 0) {
            bits <<= 1;
        }else {
           bits <<= 1;
           bits.set(0);
        }
    
        return bits;
    }
    
    int main()
    {
        std::bitset<4> bits1{ 0b0001 };
        std::cout << rotl(bits1) << '\n';
    
        std::bitset<4> bits2{ 0b0101 };
        std::cout << rotl(bits2) << '\n';
    
        return 0;
    }

    #include <bitset>
    #include <iostream>
    
    std::bitset<4> rotl(std::bitset<4> bits)
    {
        return (bits<<1) | (bits>>3);
    }
    
    int main()
    {
        std::bitset<4> bits1{ 0b0001 };
        std::cout << rotl(bits1) << '\n';
    
        std::bitset<4> bits2{ 0b1001 };
        std::cout << rotl(bits2) << '\n';
    
        return 0;
    }


<a id="org5f8b0be"></a>

## Bitmanipulation by bit masks

Bit masks &#x2014; These are predefined set of bits used to select which specific will be modified

    #include <cstdint>
    
    constexpr std::uint8_t mask0{ 0b0000'0001 }; // represents bit 0
    constexpr std::uint8_t mask1{ 0b0000'0010 }; // represents bit 1
    constexpr std::uint8_t mask2{ 0b0000'0100 }; // represents bit 2
    constexpr std::uint8_t mask3{ 0b0000'1000 }; // represents bit 3
    constexpr std::uint8_t mask4{ 0b0001'0000 }; // represents bit 4
    constexpr std::uint8_t mask5{ 0b0010'0000 }; // represents bit 5
    constexpr std::uint8_t mask6{ 0b0100'0000 }; // represents bit 6
    constexpr std::uint8_t mask7{ 0b1000'0000 }; // represents bit 7

1.  Checking if a bit is on or off by using bit masks - We use AND(&) operator.
2.  To set a bit - we use OR equals(|=) operator
3.  To reset a bit - We use bitwise AND and bitwise NOT operator (&= ~)
4.  To flip a bit - we use bitwise XOR (^=) operator

    #include <iostream>
    #include <cstdint>
    
    int main() {
        constexpr std::uint8_t mask0{ 0b0000'0001 }; // represents bit 0
        constexpr std::uint8_t mask1{ 0b0000'0010 }; // represents bit 1
        constexpr std::uint8_t mask2{ 0b0000'0100 }; // represents bit 2
        constexpr std::uint8_t mask3{ 0b0000'1000 }; // represents bit 3
        constexpr std::uint8_t mask4{ 0b0001'0000 }; // represents bit 4
        constexpr std::uint8_t mask5{ 0b0010'0000 }; // represents bit 5
        constexpr std::uint8_t mask6{ 0b0100'0000 }; // represents bit 6
        constexpr std::uint8_t mask7{ 0b1000'0000 }; // represents bit 7
    
        std::uint8_t flags {0b0000'0101}; // It means bit 0 and 2 are ON.
    
        std::cout << (static_cast<bool>(flags & mask0)? "ON\n" : "OFF\n");  // TO CHECK ON AND OFF
    
        std::cout << (static_cast<bool>(flags & mask1)? "ON\n" : "OFF\n");
    
        flags |= mask1; // TO SET THE BIT
        flags |= (mask3 | mask4 | mask5); // TO SET MULTIPLE BITS
        std::cout << (static_cast<bool>(flags & mask1)? "ON\n" : "OFF\n");
    
        flags &= ~mask1; //TO RESET THE BIT
        std::cout << (static_cast<bool>(flags & mask1)? "ON\n" : "OFF\n");
    
        flags ^= mask1; //TO FLIP THE BIT
        std::cout << (static_cast<bool>(flags & mask1)? "ON\n" : "OFF\n");
    
        return 0;
    }

[Quiz](https://www.learncpp.com/cpp-tutorial/bit-manipulation-with-bitwise-operators-and-bit-masks/)

    #include <bitset>
    #include <cstdint>
    #include <iostream>
    
    int main()
    {
        [[maybe_unused]] constexpr std::uint8_t option_viewed{ 0x01 };
        [[maybe_unused]] constexpr std::uint8_t option_edited{ 0x02 };
        [[maybe_unused]] constexpr std::uint8_t option_favorited{ 0x04 };
        [[maybe_unused]] constexpr std::uint8_t option_shared{ 0x08 };
        [[maybe_unused]] constexpr std::uint8_t option_deleted{ 0x10 };
    
        std::uint8_t myArticleFlags{ option_favorited };
        std::cout << std::bitset<8>{ myArticleFlags } << '\n';
    
        myArticleFlags |= option_viewed;
        std::cout << (static_cast<bool>(option_favorited & option_deleted)? "NOT DELETED\n" : "DELETED\n");
    
        myArticleFlags &= ~option_favorited;
        std::cout << std::bitset<8>{ myArticleFlags } << '\n';
        return 0;
    }

Q1. Write a program that asks the user to input a number between 0 and 255. Print this number as an 8-bit binary number (of the form #### ####). Don’t use any bitwise operators. Don’t use std::bitset

    #include <iostream>
    using namespace std;
    
    int main() {
        int decimal_num{};
    
        cout << "Enter a number between 0 and 255\n";
        cin >> decimal_num;
    
        for(int divisor{128}; divisor >= 1; divisor /= 2) {
            if((decimal_num/divisor)%2 == 0) {
                cout << '0';
            }else {
                cout << '1';
            }
        }
    
        return 0;
    }


<a id="org9f8b3da"></a>

# Namespace and scope resolution

    #include <iostream>
    using namespace std;
    
    namespace Foo
    {
        int dosomething(int a, int b) {
            return a+b;
        }
    }
    namespace Goo
    {
        int dosomething(int a, int b) {
            return a-b;
        }
    }
    
    int main()
    {
        cout << Goo::dosomething(1,2) << '\n';  // "::" ------> called scope resolution operator
        cout << Foo::dosomething(1,2) << '\n';
        return 0;
    }


<a id="org42d5974"></a>

## Static local variables

local varibales &#x2014; created at the start of block and destroyed at the end of block
static local varibales &#x2013;&#x2014; created at the start of program and destroyed at the end of program.

example without static

    #include <iostream>
    using namespace std;
    
    void increment()
    {
        int x{1};
        ++x;
        cout << x << "\n";
    }
    
    int main() {
        increment();
        increment();
        increment();
        return 0;
    }

example with static

    #include <iostream>
    using namespace std;
    
    void increment()
    {
        static int x{1};
        x++;
        cout << x << "\n";
    }
    int main() {
       increment();
       increment();
       increment();
        return 0;
    }


<a id="org6d9cbc1"></a>

# Control Flow


<a id="org0d31cfc"></a>

## Switch case

    #include <iostream>
    using namespace std;
    
    int main() {
    
        int x{3};
    
        switch(x)
        {
        case 1:
            cout << "One" << "\n";
            break;
        case 2:
            cout << "Two" << "\n";
            break;
        default:
            cout << "Error" << "\n";
            break;
        }
    
        return 0;
    }


<a id="org4d7b3ed"></a>

## goto statements

    #include <iostream>
    using namespace std;
    
        void printhello(bool is)
        {
            if(is)
            {
                goto end;
            }
            cout << "Hello" << "\n";
    end:
         cout << "end" << "\n";
        }
    
    int main() {
        printhello(true);
        //printhello(false);
        return 0;
    }


<a id="org9be293f"></a>

## While loop

    #include <iostream>
    using namespace std;
    
    int main() {
        char alp{65};
    
       while(alp <= 90)
       {
           cout << alp << "-" << static_cast<int>(alp) << "\n";
           alp++;
       }
    
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    int main() {
        int x{5};
    
        while(x > 0)
        {
            int i = x;
            while(i > 0)
            {
                cout << i << " ";
                i--;
            }
            cout << "\n";
            x--;
        }
    
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    int main() {
        int x{1};
    
        while(x <= 5)
        {
            int y{5};
    
            while(y>=1){
               if(y <= x){
                   cout << y << ' ';
               }else {
                   cout << " ";
               }
               --y;
            }
            cout << "\n";
            ++x;
        }
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    void fizzbuzz(int x)
    {
        for(int i=1;i<=x;i++)
        {
            if(i%3==0 && i%5==0) {
                cout << "FizzBuzz" << "\n";
            }else if(i%5==0){
               cout << "Buzz" << "\n";
            }else if(i%3==0){
                cout << "Fizz" << "\n";
            }else if(i%7==0){
                cout << "pop" << "\n";
            }else{
                cout << i << "\n";
            }
        }
    }
    
    int main() {
        int y;
        cin >> y;
        fizzbuzz(y);
    
        return 0;
    }


<a id="org6919d50"></a>

## Do While


<a id="org5a9740d"></a>

## For Loop


<a id="orgf60e0d8"></a>

## std::exit

When main function is returned a special function std::exit() is called with return value from main.

-   It performs number of cleanup functions.
    1.  Objects with static storage duration are destroyed.
    2.  Then some other miscellaneous file cleanup is done if any files were used.
-   calling std::exit explicitly.
    std::exit() is called implicitly when main function is returned. But we can also explicitly call the function
    For that we have to use <cstdlib> library
    
        #include <iostream>
        #include <cstdlib>
        using namespace std;
        
        int main() {
        
            cout << "Before exit" << "\n";
        
            exit(0);
        
            cout << "after exit" << "\n"; //This statement is never exucuted
        
            return 0;
        }

std::exit() doesnt clean up local variable.Means

1.  closing database and networks.
2.  deallocating memory

For this we have to call another cleanup function before std::exit.
For making this easier there is another fucntion called std::atexit
std::atexit is called automatically when std::exit is called --------&#x2013;&#x2014;> std::atexit(cleanup)
here cleanup is a function.


<a id="org938ad45"></a>

# Mersenne Twister

    #include <iostream>
    #include <random>
    
    int main() {
        std::mt19937 mt{};
    
        for(int i=0;i<=10;i++)
        {
            std::cout << mt() << "\n";
        }
        return 0;
    }


<a id="org08d55ae"></a>

# Function Templates

    #include <iostream>
    using namespace std;
    
    template <typename T>
    
    T add(T x,T y)
    {
        return x+y;
    }
    
    int main() {
       cout <<  add<float>(1.2,2.5) << "\n";
        return 0;
    }


<a id="orgc717479"></a>

# Constexpr and Consteval Functions

constexpr functions are initialized at the compile time.
They may or maybe not be initialized at the compile time. But consteval functions are always evaluated at the compile time.

    #include <iostream>
    using namespace std;
    
    constexpr int add(int x,int y)
    {
        return x+y;
    }
    
    int main() {
        constexpr int x {add(1,2)};
        cout << x << "\n";
    
        return 0;
    }

consteval functions have to evaluate at the compile time only or else it will through an error.
These functions are also called as immediate fucntions

    #include <iostream>
    using namespace std;
    
    consteval int add(int x,int y)
    {
        return x+y;
    }
    
    int main() {
    
        constexpr int a{add(10,20)}; // This will evaluate
        cout << a << "\n";
    
        cout << add(10,20) << "\n"; // This will evaluate
    
        int b{20};
        cout << add(10,b); //This will not evaluate.
        return 0;
    }


<a id="org02f6401"></a>

# Compound data types

<div class="mindmap" id="orgd3d4539">
<p>
   ╭─ Functions
   ├─ C-style arrays
   ├─ Pointer Types ┬─ Pointer to Object
   │                ╰─ pointer to function
   ├─ Pointer to member types ┬─ pointer to data member
   │                          ╰─ pointer to member function
«» ┼─ Reference types ┬─ L-value references
   │                  ╰─ R-value references
   ├─ Enumerated Types ┬─ Unscoped enumerations
   │                   ╰─ Scoped enumerations
   │              ╭─ Structs
   ╰─ Class Types ┼─ Classes
                  ╰─ Unions
</p>

</div>


<a id="org6c01415"></a>

## L-value references


<a id="org7f36f3b"></a>

### Non-const L value references

    #include <iostream>
    using namespace std;
    
    int main() {
        int x{2};
        int& y{x};
        cout << y << "\n";
        cout << x << "\n";
    
        x = 4;
        cout << y << "\n";
        cout << x << "\n";
    
        y = 5;
        cout << y << "\n";
        cout << x << "\n";
        return 0;
    }


<a id="org3eeae32"></a>

### Const L-value referencs

    #include <iostream>
    using namespace std;
    
    int main() {
    
        const int x {2};
        const int& ref{x};
    
        cout << ref << "\n";
    
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    int main() {
        int x{2};
        const int& ref{x};
    
        cout << ref << "\n";
        cout << x << "\n";
    
        x = 3;      // Modified by variables.
        cout << ref << "\n";
    
        ref = 4;    // Cannot be modified by ref since it is const
        cout << ref << "\n";
    
        return 0;
    }

If we initialize lvalue const reference to rvalue.
Then a temporary object is created with rvalue and reference to const is bound to that temporary object.
Temporary objects are destroyed at the end of the statement.
But this creates a dangling ref so that compilers extend the lifetime of temporary objects to match the lifetime of ref.

Non-const lvalue references require an lvalue (an object with a persistent memory address) because they are designed to allow modification of the referenced object.  Rvalues (such as temporary objects or literals) do not have a persistent memory address and are immutable; binding a non-const reference to them would allow modifications to an object that is immediately destroyed or cannot be changed, leading to undefined behavior or logical errors.

    #include <iostream>
    using namespace std;
    
    int main() {
        const int& ref{2};
        cout << ref << "\n";
        return 0;
    }

with diif data types.

    #include <iostream>
    using namespace std;
    
    int main() {
        char alp{'T'};
    
        const int& ref{alp};
    
        cout << ref << "\n";
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    int main() {
        double x {5};
        const int& ref{x};
        cout << ref << "\n";
        return 0;
    }


<a id="org04734c5"></a>

## R-value refernces

    #include <iostream>
    using namespace std;
    
    int main() {
        int& rvalueref = 5; // we cannot do this. Because we are assigning lvalueref to rvalue;
        int&& rvalueref = 5; // rvalue ref can be done like this
        cout << rvalueref << '\n';
        return 0;
    }


<a id="org785286b"></a>

## Pass by reference

    #include <iostream>
    #include <string>
    using namespace std;
    
    void printname(string x)
    {
        cout << x << "\n" ;
    }
    
    int main() {
    
        string name {"Shiva"};
    
        printname(name);
    
        return 0;
    }

Although the above program works fine.It is inefficent to make a copy of a string and will be destroyed  after the function.
So we use pass by reference.

    #include <iostream>
    #include <string>
    using namespace std;
    
    void printname(string& ref)  //here we ref to name instead of making a copy
    {
        cout << ref << "\n";
        ref = "Shiva";
        cout << ref << "\n";
    }
    
    int main() {
        string name{"Prasad"};
        printname(name);
    
        return 0;
    }

    #include <iostream>
    using namespace std;
    void passbyvalue(int x)
    {
        cout << &x << "\n";
    }
    
    void passbyreference(int& x)
    {
        cout << &x << "\n";
    }
    int main() {
        int x{2};
        cout << &x << "\n";
        passbyvalue(x);
        passbyreference(x);
        return 0;
    }

Here we can notice the address of passbyreference and original varible is same.


<a id="org99f66fc"></a>

## pass by const lvalue reference

Unlike non-const lvalue reference for which we can bind to modifiable lvalues.
pass by const lvalue reference can be bind to modifiable, non-modifiable lvalues and rvalues.

    #include <iostream>
    using namespace std;
    
    void print(const int& ref)
    {
        cout << ref << "\n";
    }
    
    int main() {
    
        int x{2};  // we can pass nonconst varibales (modifiable)
        print(x);
    
        const int y{3};  // we can pass const varibales (non-modifiable)
        print(y);
    
        print(4);  // we can pass literal
    
        return 0;
    }


<a id="orgb3974fa"></a>

## why prefer std::string<sub>view</sub> to const std::string&

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">Argument Type</th>
<th scope="col" class="org-left">std::string<sub>view</sub> parameter</th>
<th scope="col" class="org-left">const std::string&amp; parameter</th>
</tr>
</thead>
<tbody>
<tr>
<td class="org-left">std::string</td>
<td class="org-left">Inexpensive conversion</td>
<td class="org-left">Inexpensive reference binding</td>
</tr>

<tr>
<td class="org-left">std::string<sub>view</sub></td>
<td class="org-left">Inexpensive copy</td>
<td class="org-left">Expensive explicit conversion to std::string</td>
</tr>

<tr>
<td class="org-left">C-style string/literal</td>
<td class="org-left">Inexpensive conversion</td>
<td class="org-left">Expensive conversion</td>
</tr>
</tbody>
</table>

    #include <iostream>
    #include <string>
    #include <string_view>
    
    void printSV(std::string_view sv)
    {
        std::cout << sv << '\n';
    }
    
    void printS(const std::string& s)
    {
        std::cout << s << '\n';
    }
    
    int main()
    {
        std::string s{ "Hello, world" };
        std::string_view sv { s };
    
        // Pass to `std::string_view` parameter
        printSV(s);              // ok: inexpensive conversion from std::string to std::string_view
        printSV(sv);             // ok: inexpensive copy of std::string_view
        printSV("Hello, world"); // ok: inexpensive conversion of C-style string literal to std::string_view
    
        // pass to `const std::string&` parameter
        printS(s);              // ok: inexpensive bind to std::string argument
        printS(sv);             // compile error: cannot implicit convert std::string_view to std::string
        printS(static_cast<std::string>(sv)); // bad: expensive creation of std::string temporary
        printS("Hello, world"); // bad: expensive creation of std::string temporary
    
        return 0;
    }


<a id="org714cb1e"></a>

## Pointers


<a id="org0c107a1"></a>

### Deference operator

& is address-of operator which returns address of object.
While \* is used to return value at a given memory address as an lvalue.

    #include <iostream>
    using namespace std;
    
    int main() {
        int x{1};
    
        cout << x << "\n";
        cout << &x << "\n";  // gives address
        cout << *(&x) << "\n";  // gives value at that address
    
        return 0;
    }


<a id="orgfc4bf6a"></a>

### Pointer

A Pointer is an object that holds a memory address as its value. This allows us to store the address of some other objects to use later.

    int;  // a normal int
    int&; // an lvalue reference to an int value
    
    int*; // a pointer to an int value (holds the address of an integer value)

    #include <iostream>
    using namespace std;
    
    int main() {
        int x{1};
        int* ptr{&x};
        cout << *ptr << "\n";
        *ptr = 2;
        cout << *ptr << "\n";
    
        return 0;
    }

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">Pointers</th>
<th scope="col" class="org-left">References</th>
</tr>
</thead>
<tbody>
<tr>
<td class="org-left">It can change the varibale it is being pointed</td>
<td class="org-left">It cannot be changed it is being refered to.</td>
</tr>

<tr>
<td class="org-left">Pointers are objects</td>
<td class="org-left">References are not objects.</td>
</tr>

<tr>
<td class="org-left">Pointers can point to nothing</td>
<td class="org-left">References must always bound to an object</td>
</tr>

<tr>
<td class="org-left">Pointers are not required to be initialized</td>
<td class="org-left">References must be initialized</td>
</tr>
</tbody>
</table>

-   The size of the pointer is independent to it is being pointed, instead it depends on architecture of the computer.
-   In a 32 bit computer 4 bytes are taken and in 64 bit computer 8 bytes are taken.


<a id="orgdb95fca"></a>

### Address of operator returns a pointer

The address of operator doesnt returns address of its operand as literal, Instead it returns a pointer to the operand.

    #include <iostream>
    #include <typeinfo>
    using namespace std;
    
    int main() {
        int x{1};
    
        cout << typeid(x).name() << "\n";
        cout << typeid(&x).name() << "\n";
    
        return 0;
    }


<a id="org604b07d"></a>

### null pointers as boolean values

-   Null pointer is implicitly converted to boolean value false.
-   Not Null pointer is implicitly converted to boolean value true.

    #include <iostream>
    using namespace std;
    
    int main() {
        int* ptr{};
    
        if(ptr) {
            cout << "Not Null" << "\n";
        }else {
            cout << "Null" << "\n";
        return 0;
    }


<a id="org4b23354"></a>

### pointer to const

1.  If the object is const then the pointer should be const.
2.  If the object is non-const, we can still point a const pointer to it but we cannot change the value of object by deferencing pointer.

    #include <iostream>
    using namespace std;
    
    int main() {
    
        const int x{2};
        const int* ptr{&x};
    
        cout << *ptr << "\n";
    
        return 0;
    }

we also make pointer ifself const. i.e, it doesnt change the address it is holding.

    #include <iostream>
    using namespace std;
    
    int main() {
        int x{1};
    
        int* const ptr{&x};
        cout << *ptr << "\n";
    
        int y{2}
        ptr = &y; // Do not possible
    
        return 0;
    }

Const pointer to a const value
With this we cannot change the address and the value.

    #include <iostream>
    using namespace std;
    
    int main() {
        int x{2};
        const int* const ptr{&x};
    
        cout << *ptr << "\n";
    
        int y{3};
    
        *ptr = 3; // Not possible
        ptr = &y
        return 0;
    }


<a id="orgf8e7a6d"></a>

### pass by address

    #include <iostream>
    #include <string>
    
    void printByValue(std::string val) // The function parameter is a copy of str
    {
        std::cout << val << '\n'; // print the value via the copy
    }
    
    void printByReference(const std::string& ref) // The function parameter is a reference that binds to str
    {
        std::cout << ref << '\n'; // print the value via the reference
    }
    
    void printByAddress(const std::string* ptr) // The function parameter is a pointer that holds the address of str
    {
        std::cout << *ptr << '\n'; // print the value via the dereferenced pointer
    }
    
    int main()
    {
        std::string str{ "Hello, world!" };
    
        printByValue(str); // pass str by value, makes a copy of str
        printByReference(str); // pass str by reference, does not make a copy of str
        printByAddress(&str); // pass str by address, does not make a copy of str
    
        return 0;
    }


<a id="org6ebbbd1"></a>

## Operator overloading

Operator overloading = writing your own function that runs when someone uses +, ==, <<, etc. on your custom data type.

    #include <iostream>
    using namespace std;
    
    struct Point {
        int x;
        int y;
    };
    
    Point operator+(Point a, Point b) {
        Point result;
        result.x = a.x + b.x;
        result.y = a.y + b.y;
    
        return result;
    }
    
    int main() {
        Point P1{1,2};
        Point P2{4,5};
        Point P3;
        P3 = P1 + P2;
        cout << P3.y;
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    struct Point {
        int x;
        int y;
    };
    
    bool operator==(Point a, Point b) {
       return (a.x == b.x) && (a.y == b.y);
    }
    
    int main() {
        Point p1{1,2};
        Point p2{1,2};
        if(p1 == p2)
            cout << "Equal" << "\n";
        else
            cout << "Not equal" << "\n";
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    struct Point {
        int x; int y;
    };
    
    ostream& operator+(ostream& hi, Point& p) {
        hi << "X: " << p.x << " Y: " << p.y;
        return hi;
    }
    
    int main() {
        Point P1{1,2};
        cout + P1;
        return 0;
    }


<a id="org50a2f89"></a>

## Enumerations

Enumerations are implicitly constexpr.


<a id="org2450862"></a>

### Unscoped Enumerations

Each enumeration is numbered from 0. We can explicitly number a enumeration, any undefined enumeration will be given one value greater than the previous one.

    #include <iostream>
    using namespace std;
    
    enum Color {red,white, yellow};
    
    int main() {
        Color car{white};
        cout << car << "\n";
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    namespace nothing{
        enum Color {
            red,
            white,
            yellow,
        };
    }
    
    int main() {
    
        nothing::Color apple{nothing::red}; //apple will store integral value 0.
    
        cout << apple << "\n";
    
        return 0;
    }

    #include <iostream>
    using namespace std;
    enum color {
        red,
        white,
        yellow,
    };
    
    int main() {
        color apple{static_cast<color>(2)};
        cout << apple << "\n";
        Return 0;
    }

    #include <iostream>
    #include <string_view>
    using namespace std;
    
    enum Color {red, white, yellow, blue};
    
    constexpr string_view Print(Color ref)
    {
        switch(ref) {
            case red: return "red";
            case white: return "white";
            case yellow: return "Yellow";
            default: return "Error";
        }
    }
    
    int main() {
        constexpr Color apple{yellow};
        cout << Print(apple) << "\n";
        return 0;
    }

    #include <iostream>
    #include <string_view>
    using namespace std;
    
    namespace nothing {
        enum Color {white, yellow, red};
    };
    
    constexpr string_view print(nothing::Color ref) {
        switch(ref){
            case white: return "white";
            case yellow: return "yellow";
            case red: return "red";
            default: return "Error";
        }
    }
    
    
    int main() {
    
        nothing::Color jersey{nothing::white};
    
        cout << print(jersey) << "\n";
    
        return 0;
    }


<a id="org2eae6eb"></a>

### scoped Enumerations

    #include <iostream>
    using namespace std;
    
    enum class Color {white, red, green};
    
    int main() {
        Color color {Color::white};
        cout << color << "\n";
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    enum class cartoon {doreman, shinchan, bheem};
    
    int main() {
    
        using enum cartoon;
    
        cartoon fav{shinchan};
    
        return 0;
    }


<a id="org594122a"></a>

## Struct

A struct is a program defined data type that allows us to bundle multiple variables together into a single type.

1.  Defining a struct

    #include <iostream>
    using namespace std;
    
    struct Employee {
        int id;
        int age;
        double salary;
    }
    
    int main() {
    
        return 0;
    }

By declaring the struct it cannot occupy any space. But by initialization the object does.

Variables inside a group are called members.

1.  Initialing a object.

    #include <iostream>
    using namespace std;
    
    struct Employee {
        int id;
        int age;
        double salary;
    }
    
    int main() {
        Employee gachibowli{};  // Object as created with the three varibles.
        return 0;
    }

1.  To access a specific member we use member selecion operator (.).

    #include <iostream>
    using namespace std;
    
    struct Employee {
        int id;
        int age;
        double salary;
    };
    
    int main() {
        Employee gachibowli{};  // Object as created with the three varibles.
    
        gachibowli.id = 1;
        cout << gachibowli.id << "\n";
    
        gachibowli.age = 67;
        cout << gachibowli.age << "\n";
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    struct Point {
        int x{};
        int y{};
    };
    
    struct triangle {
        Point a{};
        Point b{};
        Point c{};
    };
    
    int main() {
    
        Point a{2,3};
        Point b{3,4};
        Point c{4,5};
    
        triangle tri{a,b,c};
    
        triangle* ptr(&tri);
    
        cout << (ptr -> c).x << "\n";
    
        return 0;
    }


<a id="org02b3681"></a>

## Classes (OOP)

    #include <iostream>
    using namespace std;
    
    class Date {
    public:
        int m_day{};
        int m_month{};
        int m_year{};
    };
    
    void printdate(Date& date)
    {
        cout << date.m_day << "/" << date.m_month << "/" << date.m_year << "\n";
    }
    int main() {
        Date date{19, 06, 2026};
        printdate(date);
        return 0;
    }


<a id="org401926f"></a>

### member functions

    #include <iostream>
    using namespace std;
    
    class Date {
    public:
        int m_day{};
        int m_month{};
        int m_year{};
    
        void print() {
            cout << m_day << "/" << m_month << "/" << m_year << "\n";
        }
    };
    
    int main() {
        Date date{19, 06, 2026};
    
        date.print();
        return 0;
    }

-   member function with const object
    
    if the object is const then the member fucntion should also have to be a member fucntion.

    #include <iostream>
    using namespace std;
    class Car
    {
    public:
        int model{};
        int color_code{};
    
        void print() const {
           cout << "Model: " << model << " Color Code: " << color_code << "\n";
        }
    };
    int main() {
    
        const Car swift{1,79879};
    
        swift.print();
    
        return 0;
    }

\j*\*\* access functions

    #include <iostream>
    usjing namespace std;
    
    class House {
        int m_house_no{21};
        int m_members{9};
    
    public:
        void print() {
            cout << m_house_no << " " << m_members << "\n";
        }
    
        int gethouseno() const {return m_house_no;}
        void sethouseno(int houseno) {m_house_no = houseno;}
    
        int getmembers() const {return m_members;}
        void setmembers(int members) {m_members = members;}
    };
    
    int main() {
    
        House my_house{};
    
        my_house.print();
    
        my_house.sethouseno(44);
        my_house.setmembers(4);
    
        cout << my_house.gethouseno() << "\n";
        cout << my_house.getmembers() << "\n";
    
        return 0;
    \}


<a id="orgebe18e4"></a>

### returning data members by lvalue reference

    #include <iostream>
    using namespace std;
    
    class House {
        int m_houseno{12};
        int m_members{3};
    
    public:
        void print() {
            cout << m_houseno << " " << m_members << "\n";
        }
    
        int& gethouseno() {return m_houseno;}
    };
    
    int main() {
        House myhouse{};
        cout <<  myhouse.gethouseno();
        return 0;
    }

    #include <iostream>
    #include <string>
    using namespace std;
    class Bike{
        string m_name{};
    public:
    
        void setname(string_view name) {m_name = name;}
    
        string getname_byvalue() {
            return m_name;
        }
    
        string& getname_byreference() {
            return m_name;
        }
    };
    
    int main() {
        Bike bmw{};
        cout << bmw.getname_byvalue() << "\n";
        bmw.setname("BMW");
        cout << bmw.getname_byreference() << "\n";
        return 0;
    }


<a id="org3c405f9"></a>

### constructor

    #include <iostream>
    using namespace std;
    
    class Foo{
        int m_a;
        int m_b;
    
    public:
        Foo(int a,int b) {
            this->m_a = a;
            this->m_b = b;
        }
    
        //Foo(int a,int b) : m_a {a}, m_b {b}; {}
    
        void print() {
            cout << m_a << " " << m_b << "\n";
        }
    };
    
    int main() {
        Foo f{3,9};
        f.print();
        return 0;
    }

1.  A constructor is a special member function invoked when an object of class is created. It shares same name as class and has no return type.
2.  It is responsible for initializing data members and setting initial state.

Delegating constructors
Constructors are allowed to delegate (transfer responsibility for) initialization to another constructor from the same class type. This process is sometimes called constructor chaining and such constructors are called delegating constructors.

    #include <iostream>
    using namespace std;
    
    class Employee{
        string m_name{};
        int m_id{};
    public:
        Employee(string name) :Employee(name, 0) {}
    
        Employee(string name, int id) : m_name {name}, m_id {id} {}
    
        void print() {
            cout << m_name << " " << m_id << "\n";
        }
    };
    
    int main() {
        Employee e1{"shiva"};
        e1.print();
    
        Employee e2{"shiva",9};
        e2.print();
        return 0;
    }

Reducing construtor using default arguments

    #include <iostream>
    using namespace std;
    
    class Employee{
        string m_name{};
        int m_id{};
    public:
        Employee(string name, int id = 0) : m_name {name}, m_id {id} {}
    
        void print() {
            cout << m_name << " " << m_id << "\n";
        }
    };
    
    int main() {
        Employee e1{"shiva"};
        e1.print();
    
        Employee e2{"shiva",9};
        e2.print();
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    class Ball {
        string m_color{"black"};
        double m_radius{10.0};
    public:
        Ball() {
            print();
        }
    
        Ball(string color) : m_color {color} {
            print();
        }
    
        Ball(double radius) : m_radius {radius} {
            print();
        }
    
        Ball(string color, double radius) : m_color {color} , m_radius {radius} {
            print();
        }
    
        void print() {
            cout << "Ball(" << m_color << ", " << m_radius << ")" <<  "\n";
        }
    };
    int main() {
        Ball def{};
        Ball blue("blue");
        Ball twenty{20};
        Ball bluetwenty{"blue", 20};
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    class Ball{
        string m_name{};
        double m_radius{};
    public:
        Ball(double radius) : Ball{"black", radius} {}
    
        Ball(string name = "black",double radius = 10.0) : m_name {name} , m_radius {radius} {print();}
    
        void print() {
            cout << "Ball(" << m_name << ", " << m_radius << ")" <<  "\n";
        }
    };
    
    int main() {
        Ball def{};
        Ball blue("blue");
        Ball twenty{20};
        Ball bluetwenty{"blue", 20};
        return 0;
    }


<a id="org62b12fa"></a>

### temporary object

    #include <iostream>
    using namespace std;
    
    class Point{
        int m_x{};
        int m_y{};
    
    public:
        Point(int x, int y) : m_x {x} , m_y {y} {};
    
        int x() {return m_x;}
        int y() {return m_y;}
    };
    
    void print(Point p) {
        cout << p.x() << " " << p.y() << "\n";
    }
    
    int main() {
        Point p1{1,2};
        print(p1);
        print(Point {3,4}  );
        print({1,2});
        return 0;
    }

-   callling a constructor in a function creates a temporary object


<a id="org7869046"></a>

### delegating [constructor](#org3c405f9)

To make one [constructor](#org3c405f9) delegate to another construtor simply call the constructor in member initialization list of another [constructor](#org3c405f9).

    #include <iostream>
    using namespace std;
    
    class Employee {
        string m_name{};
        int m_age{};
    public:
        Employee(string name) : Employee(name, 0) {}
    
        Employee(string name, int age) : m_name {name} , m_age {age} {cout << m_name << " " << m_age << "\n";}
    };
    
    int main() {
        Employee e1{"Shiva"};
        Employee e2{"PRASAD",2};
        return 0;
    }


<a id="org59502b6"></a>

### copy [constructor](#org3c405f9)

A copy construtor is a construtor that is used to initialize an object using an existing object.

A copy [constructor](#org3c405f9) is implicitly created by compiler when we create a object using another object like in below. Although we can create copy [constructor](#org3c405f9) manually.

    #include <iostream>
    using namespace std;
    
    class Number {
        int m_a{};
        int m_b{};
    public:
        Number(int a, int b) : m_a {a}, m_b{b} {}
    
        void print() {
            cout << m_a << " " << m_b << endl;
        }
    };
    
    int main() {
        Number x{3,5};
        Number y{x};
        x.print();
        y.print();
        return 0;
    }

initiallzing a copy construtor manually.

    #include <iostream>
    using namespace std;
    
    class Number {
        int m_a{};
        int m_b{};
    public:
        Number(int a, int b) : m_a {a}, m_b{b} {}
    
        Number(Number& num) : m_a {num.m_a} , m_b {num.m_b} {
            cout << "Copy constructor is called" << "\n";
        }
    
        void print() {
            cout << m_a << " " << m_b << endl;
        }
    };
    
    int main() {
        Number x{3,5};
        Number y{x}; // here copy construtor is called
        x.print();
        y.print();
        return 0;
    }

creating a default copy construtor using **default**

    #include <iostream>
    using namespace std;
    
    class Fraction {
        int m_a{};
        int m_b{};
    public:
        Fraction(int a, int b) : m_a{a}, m_b {b} {}
    
        Fraction(const Fraction& fraction) = default;
    
        void print() {
            cout << m_a << " " << m_b << "\n";
        }
    };
    
    int main() {
        Fraction f{1,2};
        Fraction f1{f};
        f.print();
        f1.print();
        return 0;
    }

using = delete to prevent copies

    #include <iostream>
    
    class Fraction
    {
    private:
        int m_numerator{ 0 };
        int m_denominator{ 1 };
    
    public:
        // Default constructor
        Fraction(int numerator=0, int denominator=1)
            : m_numerator{numerator}, m_denominator{denominator}
        {
        }
    
        // Delete the copy constructor so no copies can be made
        Fraction(const Fraction& fraction) = delete;
    
        void print() const
        {
            std::cout << "Fraction(" << m_numerator << ", " << m_denominator << ")\n";
        }
    };
    
    int main()
    {
        Fraction f { 5, 3 };
        Fraction fCopy { f }; // compile error: copy constructor has been deleted
    
        return 0;
    }


<a id="org525606e"></a>

### pass by value and copy construtor

when we pass an object by value to a function if the argument and parameter are of same class type then implicitly copy construtort is called.

in the beow code when an object is passed as value to a function then explicitly created copy construtor is invoked.

    #include <iostream>
    using namespace std;
    
    class Number {
        int m_a{};
        int m_b{};
    public:
        Number(int a, int b) : m_a {a}, m_b{b} {}
    
        Number(Number& num)  : m_a {num.m_a} , m_b {num.m_b} {
           cout << "copy construtor is called" << "\n";
       }
    
        void print() {
            cout << m_a << " " <<  m_b << "\n";
        }
    };
    
    void fun(Number x) {
        x.print();
    }
    
    int main() {
        Number x{12,3};
        fun(x);
        return 0;
    }


<a id="org329339b"></a>

### array of object

    #include <iostream>
    using namespace std;
    
    class Student{
    public:
        string name;
        int age;
        Student() {}
        Student(string s, int a) : name{s},age{a} {}
    };
    
    int main() {
        Student s[10];
        s[0].name = "shiva";
        s[0].age = 19;
        s[1].name = "Prasad";
        s[1].age = 19;
        s[2].name = "shiva";
        s[2].age = 19;
        for(int i =0;i<3;i++) {
            cout << s[i].name <<  " " <<  s[i].age << '\n';
        }
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    class Student{
    public:
        string name;
        int age;
        Student() {}
        Student(string s, int a) : name{s},age{a} {}
    };
    
    int main() {
        Student s[] = {
            {"shiva",1},
            {"Prasad",2},
            {"sunny",3},
        };
    
        for(int i =0;i<3;i++) {
            cout << s[i].name <<  " " <<  s[i].age << '\n';
        }
        return 0;
    }


<a id="orgd4bde7a"></a>

### Copy elison

Copy elision is a compiler optimization technique that allows the compiler to remove unnecessary copying of objects. In other words, in cases where the compiler would normally call a copy constructor, the compiler is free to rewrite the code to avoid the call to the copy constructor altogether. When the compiler optimizes away a call to the copy constructor, we say the constructor has been elided.


<a id="org23b16ec"></a>

### User defined conversions

here even though we the function **gets** has parameter Numbers class type in arguments we gave int. So the compiler implicitly converts the types.
These type of functions are called **user defined functions**.

    #include <iostream>
    using namespace std;
    
    class Numbers {
        int m_a{};
    public:
        Numbers(int a) : m_a {a} {}
    
        void print() {
            cout << m_a << "\n";
        }
    
    };
    
    void gets(Numbers num) {
        num.print();
    }
    
    int main() {
        gets(2);
        return 0;
    }


<a id="orgc376490"></a>

### constexpr member functions

    #include <iostream>
    using namespace std;
    
    struct Numbers {
        int m_a{};
        int m_b{};
    
        constexpr void print() {
            cout << m_a << " " << m_b << "\n";
        }
    };
    
    int main() {
        Numbers num{1,2};
        num.print();
    
        constexpr num1{3,4};
        num1.print();
    
        return 0;
    }

This works for aggregate functions functions like **struct** but not for **class**

    #include <iostream>
    using namespace std;
    
    class Numbers {
        int m_a{};
        int m_b{};
    
    public:
        Numbers(int a, int b) : m_a{ a } , m_b {b} {}
    
        constexpr void print() {
            cout << m_a << " " << m_b << "\n";
        }
    };
    int main() {
        constexpr Numbers num{21,2};
        num.print() ;
        return 0;
    }

here when object is created the construtor is called which is of type class Numbers which is not constexpr so it doesnt run at runtime.

    #include <iostream>
    using namespace std;
    
    class Numbers {
        int m_a{};
        int m_b{};
    
    public:
        constexpr Numbers(int a, int b) : m_a{ a } , m_b {b} {}
    
        constexpr void print() {
            cout << m_a << " " << m_b << "\n";
        }
    };
    int main() {
        constexpr Numbers num{21,2};
        num.print();
        return 0;
    }

😭

    #include <iostream>
    using namespace std;
    
    class so{
        int m_a{};
    public:
        so(int a) : m_a {a} {}
    
        void print() {
            cout << m_a << "\n";
        }
    };
    
    int main() {
        so a{1};
        a.print();
    
        so* b{&a};
        b->print();
        return 0;
    }


<a id="org91237f6"></a>

### the hidden this pointer

Inside every member function the keyword this is a const pointer that holds the address of current of object.

    #include <iostream>
    using namespace std;
    
    class numbers{
        int m_a{};
    public:
        numbers(int a) :m_a {a} {}
    
        void print() {
            cout << this->m_a<< "\n";
        }
    };
    
    int main() {
        numbers n{1};
        n.print(&n);
        return 0;
    }

in the above the code can work simply if we put **m<sub>a</sub>** instead of **this->m<sub>a</sub>**
but this proves that there is a pointer of type numbers which stores address of object. so by using this->m<sub>a</sub> it can access the m<sub>a</sub> member.

    #include <iostream>
    using namespace std;
    
    class Simple{
       int m_a{};
    public:
        void set_a(int a) {
            m_a = a;
        }
    
        int get_a() {
            return m_a;
        }
    };
    
    int main() {
        Simple x{};
        x.set_a(2);
        cout << x.get_a() << "\n";
        return 0;
    }

here the compiler rewrites **x.set<sub>a</sub>(2)** as **Simple::set<sub>a</sub>(&Simple, 2)** internally

then the set<sub>a</sub> function also changes in the class as

**void set<sub>a</sub>(int a) {m<sub>a</sub> = a}** ------&#x2013;&#x2014;>>  static void set<sub>a</sub>(Simple\* const this, int a) {this->m<sub>a</sub> =a;}

1.  When we call simple.set<sub>a</sub>(2), the compiler actually calls Simple::set<sub>a</sub>(&simple, 2) and simple is passed by address to the function
2.  The function has hidden parameter named **this** which receives the address of simple.
3.  member variables inside set<sub>a</sub>() are prefixed with **this->** which points to simple. So when compiler evaluates this->m<sub>a</sub>, its actually resolving to simple.m<sub>a</sub>

4.  Each member function has single this pointer parameter that points to the implicit object.
    
    Explicitly referencing this
    
        #include <iostream>
        using namespace std;
        
        struct something {
            int a{};
        
            void set_a(int a) {
                this->a = a;
            }
        
            int get_a() {
                return a;
            }
        };
        
        int main() {
            something a{};
            a.set_a(1);
            cout << a.get_a();
            return 0;
        }

    1

    #include <iostream>
    using namespace std;
    
    class something{
        int a{};
    public:
        void get() {
            cout << *this << "\n";
        }
    };
    
    int main() {
        int a{1};
        int* ptr{&a};
        cout << *ptr << "\n";
        something s{};
        s.get();
        return 0;
    }


<a id="orgcc83b19"></a>

### member function chaining using \*this

    #include <iostream>
    using namespace std;
    
    class Cal{
        int m_a{0};
    public:
        void add(int a) {m_a += a;}
        void sub(int a) {m_a -= a;}
        void mul(int a) {m_a *= a;}
    
        int get() {
            return m_a;
        }
    };
    
    int main() {
        Cal cal{};
        cal.add(3);
        cal.sub(1);
        cal.mul(4);
        cout << cal.get();
        return 0;
    }

Here to add, sub, and mul we need to call three diffrent member fuuntions seperating but with member fucntion chaining we can do it in a single line.

    #include <iostream>
    using namespace std;
    
    class Cal{
        int m_a{0};
    public:
        Cal& add(int a) {
            m_a += a;
            return *this;
        }
    
        Cal& sub(int a) {
            m_a -= a;
            return *this;
        }
    
        Cal& mul(int a) {
            m_a *= a;
            return *this;
        }
    
        int get() {
            return m_a;
        }
    
        void reset() {
            *this = {};
        }
    };
    
    int main() {
        Cal a{};
        a.add(3).sub(1).mul(3);
        cout << a.get() << "\n";
    
        a.reset();
    
        cout << a.get();
        return 0;
    }

here first add(3) runs and adds value 3 to m<sub>a</sub> then it returns reference of the Cal object so
a.add(3).sub(1).mul(3) -&#x2013;&#x2014;> a.sub(1).mul(3)

-   Here we can reset the value of members using a member fucntion reset by \*this = {}
-   it creates a temporary Cal using default values of members and assigns it to current object.


<a id="org90a745e"></a>

### Destructor

-   Destructor is used for cleaning
-   It is called automatically when an object of a class is destroyed.
-   It doesnt have any arguments.
-   It doesnt have any return type.
-   It has name name as class preceding with a tilde(~).
-   Although we can call destructor explicitly it is called automatically almost every time.
-   If we dont not declare a dedtructot the compiler will implicitly declare a destructor with empty body.
    
        #include <iostream>
        using namespace std;
        
        class Simple{
            int m_id{};
        public:
            Simple(int id)  : m_id {id} {}
        
            ~Simple() {
                cout << "Destructor" << m_id << "\n";
            }
        
        };
        
        int main() {
            Simple s1(1);
            {
                Simple s2(2);
            }//s2 dies here so destructor of s2 is called first.
            return 0;
        }//s1 dies here.

    Destructor2
    Destructor1


<a id="org71c4df7"></a>

### static member variables and functions

    #include <iostream>
    using namespace std;
    
    struct Something{
        static int a;
    };
    
    int Something::a{1};
    
    int main() {
    
        Something something1{};
        Something something2{};
    
        something1.a = 2;
    
        cout << something1.a << "\n";
        cout << something2.a << "\n";
    
        return 0;
    }

Here we can see eventhough we changed the value of a for **something1** it has also changed for **something2**

**Static members are not associated with class objects** - we know that when we create a object it occupies memory for it, but when it comes to static member variables it will be created at the start of the program and destroyed at the program so it is independent of class object.

**When can say that - static members are global variables that live inside the scope region of a class**

Because it is independent of object we can access it with class name and scope resolution operator. just like above

It is declared as forward declare and the static members are accessed independent of access control like **private** **protected**, because the forward definations are not considered a way to access.

If we include a header file which has class definations there wont be initialized.
We have to initialize using access specifier but we can initialize to a static member if is inline.

    #include <iostream>
    using namespace std;
    
    struct Something{
        static inline int a{1};
    };
    
    int main() {
        Something something{};
        cout << something.a;
        return 0;
    }

Consider this

    #include <iostream>
    using namespace std;
    
    class Something {
        static inline int m_a{1};
    
    public:
        int get() {
            return m_a;
        }
    };
    
    int main() {
        Something s{};
        cout << s.get();
        return 0;
    }

even though this works for getting the value it need to create a object.
for this reason we use static member functions.

    #include <iostream>
    using namespace std;
    
    class Something{
        static inline int m_a{1};
    public:
        static int get() {
            return m_a;
        }
    };
    
    int main() {
        cout << Something::get();
        return 0;
    }

here we accessed a private data member using static member function without creating an object.

-   static member functions do not have \*this pointer.


<a id="org2fd4aff"></a>

### friend non-member functions

Friend function or member is used for access private or protected data of a class to another class or function.

**friend is a class or function (member or non-member) that has been granted full access to the private and protected members of another class.**

    #include <iostream>
    using namespace std;
    
    class Something{
        int m_a{};
    public:
        Something(int a) : m_a {a} {}
    
        friend void print(const Something& something); //declaration of friend function
    };
    
    
    void print(const Something& something) {
        cout << something.m_a;
    }
    
    int main() {
        Something nothing{1};
        print(nothing);
        return 0;
    }

defining friend non-member inside a class

    #include <iostream>
    using namespace std;
    
    class Something{
        int m_a{};
    public:
        Something(int a) : m_a {a} {}
    
        friend void print(const Something& something) {
            cout << something.m_a;
        }
    };
    
    int main() {
        Something nothing{1};
        print(nothing);
        return 0;
    }


<a id="orgc6f0f79"></a>

### friend class and friend member function

A friend Class is that can access private and protected member of another class.

    #include <iostream>
    using namespace std;
    
    class Storage{
        int m_d{};
        int m_n{};
    public:
        Storage(int d,int n) : m_d {d} , m_n {n} {}
    
        friend class Display;
    };
    
    class Display{
        bool first{};
    
    public:
        Display(bool b) : first {b} {}
    
        void displaystorage(Storage& storage) {
            if(first) {
                cout << storage.m_d << " " << storage.m_n << "\n";
            }else {
                cout << storage.m_n<< " " << storage.m_d << "\n";
            }
        }
    };
    
    int main() {
        Storage storage{10,20};
        Display display{false};
    
        display.displaystorage(storage); //here we are acessing the members of class Storage from class display
    
        return 0;
    }

friend member funtion - instead of making an entire class friend we can make a function from another class a friend.
this can be done like this

    #include <iostream>
    using namespace std;
    
    class Display {};
    
    class Storage{
        int m_a{};
        int m_n{};
    
    public:
        Storage(int a, int n) : m_a {a} , m_n{n} {}
    
        friend void Display::displaystorage(const Storage& storage);
    };
    
    class Display{
        bool is{};
    public:
    
        Display(bool b) : b{is} {}
    
        void displaystorage(const Storage& storage) {
            if(is) {
                cout << m_a << " " << m_n << "\n";
            }else {
                cout << m_n << " " << m_a << "\n";
            }
        }
    };
    
    int main() {
    
        Storage storage{10,20};
        Display display{true};
    
        display.displaystorage();
    
        return 0;
    }

This doesnt work because the compiler will throw an error the it hasnt seen full defination of class Display

Instead we can do something like this

    #include <iostream>
    using namespace std;
    
    class Storage;
    
    class Display{
       bool is{};
    public:
        Display(bool b) : is{b} {}
        void displaystorage(Storage& storage);  // This is the reason we farward declared class Storage.
    };
    
    class Storage{
        int m_n{};
        int m_a{};
    public:
        Storage(int n, int a) : m_n{n} , m_a{a} {}
    
        friend void Display::displaystorage(Storage& storage);
    };
    
    void Display::displaystorage(Storage& storage) {
        if(is) {
            cout << storage.m_n << " " << storage.m_a << "\n";
        }else {
            cout << storage.m_a << " " << storage.m_n << "\n";
        }
    }
    
    int main() {
        Storage storage{10,20};
        Display display{false};
        display.displaystorage(storage);
        return 0;
    }

[Quiz](https://www.learncpp.com/cpp-tutorial/friend-classes-and-friend-member-functions/)

    #include <iostream>
    using namespace std;
    
    class Vector{
        double m_x{};
        double m_y{};
        double m_z{};
    public:
        Vector(double x, double y, double z) : m_x{x}, m_y{y} , m_z{z} {}
    
        void print() {
            cout << "x: " << m_x << " y: " << m_y << " z: " << m_z << "\n";
        }
    
        friend class Point;
    };
    
    class Point{
        double m_x{};
        double m_y{};
        double m_z{};
    public:
        Point(double x,double y,double z) :m_x {x}, m_y{y}, m_z{z} {}
    
        void print() {
            cout << "x: " << m_x << " y: " << m_y << " z: " << m_z << "\n";
        }
    
        void movebyvector(Point& point) {
            cout << point.m_x + m_x << " " << point.m_y + m_y << " " << point.m_z + m_z << "\n";
        }
    };
    
    int main() {
        Vector vector{1.2, 2.2, 3.4};
        Point point{2.3, 3.4, 4.9};
        point.movebyvector(point);
        return 0;
    }


<a id="orga2f1a21"></a>

# Dynamic arrays


<a id="org7e7787f"></a>

## Introduction to std::vector

    #include <iostream>
    #include <vector>
    
    int main() {
        std::vector<int> empty{};
        std::vector<int> whole{0,1,2,3};
    
        std::cout << whole[2];
        return 0;
    }

Containers typically have a special constructor called a list constructor that allows us to construct an instance of the container using an initializer list. The list constructor does three things:

1.  Ensures the container has enough storage to hold all the initialization values (if needed).
2.  Sets the length of the container to the number of elements in the initializer list (if needed).
3.  Initializes the elements to the values in the initializer list (in sequential order).

    #include <iostream>
    #include <vector>
    using namespace std;
    
    int main() {
        const vector<int> arr{1,2};
        cout << arr[1];
        return 0;
    }

length using size() member function.

    #include <iostream>
    #include <vector>
    using namespace std;
    
    int main() {
        vector arr{1,2,3};
        cout << arr.size() << "\n";
        cout << size(arr);
        return 0;
    }

Since size() member function supports only unsigned numbers when we assign the length to a variable using size() it may result in signed/unsigned conversion warnings

Instead we cast using static cast

    #include <iostream>
    #include <vector>
    using namespace std;
    
    int main() {
        vector arr{1,2};
        //int length {arr.size()}; gives warning
        int length (static_cast<int>(arr.size()));
        cout << length;
        return 0;
    }

using ssize for length

-   Since ssize is non-member function and returns lenght as long signed int we also need to cast this.j
    
        #include <iostream>
        #include <vector>
        using namespace std;
        
        int main() {
            vector arr{1,2,3};
            int length {std::ssize(arr)};
            cout << length << "\n";
            return 0;
        }

pass by reference

    #include <iostream>
    #include <vector>
    using namespace std;
    
    void fun(const vector<int>& arr) {
        cout << arr[0];
    }
    
    int main() {
        vector arr{1,2,3,4};
        fun(arr);
        return 0;
    }

we have to mention type of data in function parameter
we can use template

    #include <iostream>
    #include <vector>
    using namespace std;
    template <typename T>
    void fun(const vector<T>& arr) {
        cout << arr[0] << "\n";
    }
    
    int main() {
        vector arr1{1,2,3};
        vector arr2{1.2, 3.2};
        fun(arr1);
        fun(arr2);
        return 0;
    }


<a id="orgf29fb74"></a>

### passing a std::vector using generic template or abbreviated function template

we can also create a template that can accpet any type of object.

    #include <iostream>
    #include <vector>
    using namespace std;
    template<typename T>
    
    void print(const T& arr) {  // will accept any type of object that has an overload operator
    
        cout << arr[2] << "\n";
    }
    
    int main() {
        vector arr1{1,2,3};
        print(arr1);
        vector arr2{11.1,10.2,11.3};
        print(arr2);
    
        return 0;
    }

    #include <iostream>
    #include <vector>
    using namespace std;
    
    void print(const auto& arr) {
        cout << arr[0];
    }
    
    int main() {
        vector arr{1,2,3};
        print(arr);
        return 0;
    }

    #include <iostream>
    #include <vector>
    using namespace std;
    template <typename T>
    void print(const T& arr, int n) {
        if(n<arr.size()) {
            cout << arr[n] << "\n";
        }else {
            cout << "N should be less than the size of array" << "\n";
        }
    }
    
    int main() {
        vector arr{1,2,3,4};
        print(arr,5);
    
        vector arr1{4.5, 3.4, 6.7};
        print(arr1,2);
        return 0;
    }


<a id="orgee2d0ea"></a>

### move semantics

**Move semantics is an optimization that allow us, under certain circumstances, to inexpensively transfer ownership of some data members from one object to another object(rather than making a more expensive copy)**

-   Normally when an object is being initialized with an object of the same type, copy semantic will be used.


<a id="org853d377"></a>

### arrays and loop

    #include <iostream>
    #include <vector>
    #include <cstddef>
    using namespace std;
    
    void avg(vector<int>& arr){
        size_t length (arr.size());
        int sum = 0;
        for(size_t index = 0; index < length; ++index) {
            sum += arr[index];
        }
        int avg = sum / static_cast<int>(length);
        cout << avg << "\n";
    }
    
    int main() {
        vector arr{1,2,3,4,5,6,7};
        avg(arr);
        return 0;
    }


<a id="org4cd926f"></a>

### template arrays and loop

    #include <iostream>
    #include <vector>
    #include <cstddef>
    using namespace std;
    template <typename T>
    
    void avg(vector<T>& arr) {
        size_t length {arr.size()};
        T sum = 0;
    
        for(size_t index = 0; index < length; ++index) {
            sum += arr[index];
        }
        T avg = sum / static_cast<int>(length);
        cout << avg << "\n";
    }
    
    int main() {
        vector arr1{1,2,3};
        avg(arr1);
    
        vector arr2{2.4,5.6,7.8};
        avg(arr2);
        return 0;
    }

    #include <iostream>
    #include <vector>
    #include <cstddef>
    using namespace std;
    template <typename T>
    
    T print(vector<T>& arr) {
        size_t length {arr.size()};
    
    }
    
    T getnumber() {
        int n{};
        do {
            cout << "Enter a number blw 1 to 9" << "\n";
            cin >> n;
        }while(n < 1 || n > 9);
    
        return
    }
    
    int main() {
    
        vector arr{1,6,4,6,3,3,8};
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    int main() {
        int arr[5] = {2,2,3,4,5};
        int n;
        cin >> n;
        //int found = 0;
        for(int i=0;i<5;i++) {
            if(arr[i] == n){
                cout << i << "\n";
                //found = 1;
                return 0;
            }
        }
        // if(!found) {
        //     cout << "Element not found" << "\n";
        // }
        cout << "Element not found";
    
        return 0;
    }

    #include <iostream>
    #include <vector>
    #include <cstddef>
    #include <limits>
    using namespace std;
    
    int fun(vector<int>& arr, int val) {
        for(size_t index = 0; index < arr.size();++index) {
            if(arr[index] == val) {
                return static_cast<int>(index);
                //return true;
            }
        }
        return -1;
    }
    
    int get() {
        int num;
        do{
            cout << "Enter a number between 1 to 9: " << "\n";
            cin >> num;
    
            if(!cin) {
                cin.clear();
            }
            cin.ignore(numeric_limits<streamsize>::max(), '\n');
        } while(num < 1 || num > 9);
    
        return num;
    }
    
    int main() {
        vector arr{1,2,7,3,5};
        int num {get()};
        int ans = fun(arr , num);
        if(ans != -1) {
            cout << "The index of the number " << num << " is: " << ans << '\n';
        }else {
            cout << "The number does not exist in the array" << "\n";
        }
        return 0;
    }

Here we use cin.clear to start the broken input method, it checks if the input method is broken if it is then start it again.
And cin.ignore the dump what we dont want means it clear the clogged pipe of inputs and keeps only valid.
The &rsquo;\n&rsquo; is for the cin.ignore to know where it to stop.


<a id="org4183a9d"></a>

## Range based for Loops

    #include <iostream>
    #include <vector>
    using namespace std;
    
    int main() {
        vector arr {1,2,3,4,5};
        for(int num:arr) {
            cout << num << " ";
        }
        return 0;
    }

    #include <iostream>
    #include <vector>
    using namespace std;
    
    int main() {
        vector arr {1,2,3,44,4};
        for(auto num : arr) {
            cout << num << " ";
        }
        return 0;
    }

Avoid this for strings. use reference

    #include <iostream>
    #include <vector>
    using namespace std;
    
    int main() {
        vector arr {"Spiderman","No", "way", "Home"};
        for(auto& word : arr ) {
            //word = "Blank";  we can also change the values from here since it is reference
            cout << word << " ";
        }
    
    
        return 0;
    }

**For range based for loops, prefer to define the elements type as**

-   auto        - when u want to modify copies of elements
-   auto&       - when u want to modify original elements.
-   const auto& - when u only want to view elements.


<a id="org5d7830a"></a>

## Using unscoped emumerators for indexing

    #include <iostream>
    #include <vector>
    using namespace std;
    
    namespace Names {
        enum Name {Shiva,prasad,sunny,venkatesh};
    }
    
    int main() {
        vector marks {10,90,78,89};
        marks[Names::prasad] = 100;
        for(int mark : marks) {
            cout << mark << " ";
        }
        return 0;
    }


<a id="orge1f7f22"></a>

## resizing std::vector at runtime

    #include <iostream>
    #include <vector>
    using namespace std;
    
    int main() {
        vector a{1,2,4};
        cout << a.size() << "\n";
        a.resize(5);
    
        for(auto i : a) {
            cout << i << " ";
        }
        cout << "\n";
        cout << a.size();
        return 0;
    }

    #include <iostream>
    #include <vector>
    using namespace std;
    
    int main() {
        vector a{1,2,3,4,5};
        cout << a.size() << "\n";
    
        for(auto i : a) {
            cout << i << " ";
        }
        cout << "\n";
        a.resize(3);
        cout << a.size() << "\n";
    
        for(auto i : a) {
            cout << i << " ";
        }
        return 0;
    }

**Reallocation Process**

-   std::vector acquires new memory with capacity for the desired number of elements. These elements are value-initialized.
-   The elements in the old memory are copied (or moved, if possible) into the new memory. The old memory is then returned to the system.
-   The capacity and length of the std::vector are set to the new values.


<a id="org5e8dc7c"></a>

### length and capacity

    #include <iostream>
    #include <vector>
    using namespace std;
    
    void print(vector<int>& a){
        cout << "Length: " << a.size() << " Capacity: " << a.capacity() << "\n";
    }
    
    int main() {
        vector a{1,2,3,4,5};
    
        print(a);
        for(auto i:a) {
            cout << i << " ";
        }
        cout << "\n";
    
        a.resize(3);
        print(a);
        for(auto i:a) {
            cout << i << " ";
        }
        cout << "\n";
    
        a.resize(5);
        print(a);
        for(auto i:a) {
            cout << i << " ";
        }
        return 0;
    }

When we initialized our vector with 5 elements, the capacity was set to 5, indicating that our vector initially allocated space for 5 elements. The length was also set to 5, indicating that all of those elements are in use.

After we called v.resize(3), the length was changed to 3 to fulfill our request for a smaller array. However, note that the capacity is still 5, meaning that the vector did not do a reallocation!

Finally, we called v.resize(5). Because the vector already had a capacity of 5, it did not need to reallocate. It simply changed the length back to 5, and value-initialized the last two elements.


<a id="org55fde8f"></a>

### shrink<sub>to</sub><sub>fit</sub>

    #include <iostream>
    #include <vector>
    using namespace std;
    void print(vector<int>& a) {
        cout << "Length: " << a.size() << " Capacity: " << a.capacity() << "\n";
    }
    int main() {
        vector arr{1,2,3,4,5,6};
        print(arr);
        for(auto i : arr) {
            cout << i << " ";
        }
        cout << "\n";
    
        arr.resize(3);
        print(arr);
        for(auto i : arr) {
            cout << i << " ";
        }
        cout << '\n';
    
        arr.shrink_to_fit();
        print(arr);
        for(auto i : arr) {
            cout << i << " ";
        }
    
        return 0;
    }


<a id="orged70e85"></a>

## std::vector and stack behaviour

In programming, a stack is a container data type where the insertion and removal of elements occurs in a LIFO(last in first out) manner. This is commonly implemented via two operations named push and pop:

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<tbody>
<tr>
<td class="org-left">Push</td>
<td class="org-left">puts new element on top of stack</td>
<td class="org-left">&#xa0;</td>
</tr>

<tr>
<td class="org-left">Pop</td>
<td class="org-left">remove the top element from top</td>
<td class="org-left">may return removed element or void</td>
</tr>

<tr>
<td class="org-left">Top or Peek</td>
<td class="org-left">get the top element of the stack</td>
<td class="org-left">do not remove item</td>
</tr>

<tr>
<td class="org-left">Emptying</td>
<td class="org-left">Determine if stack has no elements</td>
<td class="org-left">&#xa0;</td>
</tr>

<tr>
<td class="org-left">Size</td>
<td class="org-left">count how many elememts in the stack</td>
<td class="org-left">&#xa0;</td>
</tr>
</tbody>
</table>

stack behaviour with std::vector

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<tbody>
<tr>
<td class="org-left">push<sub>back</sub>()</td>
<td class="org-left">put new element on top of stack</td>
<td class="org-left">Add elements to end of vector</td>
</tr>

<tr>
<td class="org-left">pop<sub>back</sub>()</td>
<td class="org-left">Remove element from the stack</td>
<td class="org-left">Returns void,removes element at the end of vector</td>
</tr>

<tr>
<td class="org-left">back()</td>
<td class="org-left">get the top element on the stack</td>
<td class="org-left">does not remove item</td>
</tr>

<tr>
<td class="org-left">emplace<sub>back</sub>()</td>
<td class="org-left">Alternate form of push<sub>back</sub>() more effcient</td>
<td class="org-left">Add elememts to the vector</td>
</tr>
</tbody>
</table>

    #include <iostream>
    #include <vector>
    using namespace std;
    
    void print(vector<int>& stack) {
        if(stack.empty()) {
            cout << "Empty" << '\n';
        }
    
        for(auto i : stack) {
            cout << i << ' ';
        }
        cout << '\n';
    
       cout << "Length: " << stack.size() << " capacity: " << stack.capacity() << '\n';
    }
    
    int main() {
        vector<int> stack{};
        print(stack);
    
        stack.push_back(1);
        print(stack);
    
        stack.push_back(2);
        print(stack);
        return 0;
    }


<a id="org94720fc"></a>

## reserve member function

    #include <iostream>
    #include <vector>
    using namespace std;
    
    void print(vector<int>& a) {
        if(a.empty()) {
            cout << "Empty" << '\n';
        }
        for(auto i : a) {
            cout << i << ' ';
        }
        cout << '\n';
        cout << "Length: " << a.size() << " Capacity: " << a.capacity() << '\n';
    }
    
    int main() {
        vector<int> stack{};
    
        print(stack);
    
        stack.reserve(6);
        print(stack);
    
        stack.push_back(1);
        print(stack);
    
        stack.push_back(2);
        print(stack);
        return 0;
    }

    #include <iostream>
    #include <vector>
    #include <limits>
    using namespace std;
    
    int main() {
        vector<int> a{};
    
        while(true) {
            cout << "Enter the digits or -1 to finish: "  << '\n';
            int x{};
            cin >> x;
    
            if(!cin) {
                cin.clear();
                cin.ignore(numeric_limits<streamsize>::max(),'\n');
            }
            if(x == -1) {
                break;
            }
    
            a.push_back(x);
        }
    
        for(auto i:a) {
            cout << i << ' ';
        }
    
        return 0;
    }


<a id="orgc9277c6"></a>

## std::vector<bool>

    #include <iostream>
    #include <vector>
    using namespace std;
    
    int main() {
        vector<bool> B{true,false,false};
        for(auto i : B) {
            cout << i << ' ';
        }
        cout << '\n';
        B[2] = true;
        for(auto i : B) {
            cout << i << ' ';
        }
        return 0;
    }

First, std::vector<bool> has a fairly high amount of overhead (sizeof(std::vector<bool>) is 40 bytes on the author’s machine), so you won’t save memory unless you’re allocating more Boolean values than the overhead for your architecture.

Second, the performance of std::vector<bool> is highly dependent upon the implementation (as implementations aren’t even required to do optimization, let alone do it well). Per this article, a highly optimized implementation can be significantly faster than alternatives. However, a poorly optimized implementation will be slower.

Third and most importantly, std::vector<bool> is not a vector (it is not required to be contiguous in memory), nor does it hold bool values (it holds a collection of bits), nor does it meet C++’s definition of a container.


<a id="org0e6f5dc"></a>

## Quiz questions

    #include <iostream>
    #include <vector>
    using namespace std;
    
    enum Game {health_portions,torches,arrows};
    
    int print(const vector<int>& a) {
        int sum = 0;
        for(auto i:a) {
            sum += i;
        }
        return sum;
    }
    
    int main() {
        vector<int> bag{1,5,10};
        cout << "You have total " << print(bag) << " items" << '\n';
        return 0;
    }

    #include <iostream>
    #include <vector>
    #include <string_view>
    using namespace std;
    
    enum Game {health_portions,torches,arrows};
    
    string_view enumtostring(Game ref) {
        switch(ref) {
            case health_portions : return "health portions";
            case  torches : return "torches";
            case arrows : return "arrows";
            default: return "Error";
        }
    }
    
    void print(vector<int>& a) {
       for(int i=0;i<3;i++) {
           cout << "You have " << a[i] << ' ' << enumtostring(static_cast<Game>(i)) << '\n';
       }
    }
    
    int total(vector<int>& a) {
        int sum = 0;
        for(auto i : a) {
            sum += i;
        }
        return sum;
    }
    
    int main() {
        vector<int> inventory{1,5,10};
        print(inventory);
        cout << "You have total " << total(inventory) << " items" << '\n';
        return 0;
    }

    #include <iostream>
    #include <vector>
    using namespace std;
    
    void max(const vector<int>& a) {
        int max = a[0];
        int maxindex;
        size_t length = a.size();
        for(size_t index = 0;index < length;index++) {
            if(a[index] > max) {
                max = a[index];
                maxindex = static_cast<int>(index);
            }
        }
        cout << "Max element has index " << maxindex << " and value " << max << '\n';
    }
    
    void min(const vector<int>& a) {
        int min = a[0];
        int minindex;
        size_t length = a.size();
        for(size_t index = 1;index < length; index++) {
            if(a[index] < min) {
                min = a[index];
                minindex = static_cast<int>(index);
            }
        }
    
        cout << "Min element has index "  << minindex << " and value " << min << '\n';
    }
    
    int main() {
        vector<int> a{3,8,2,5,7,8,2};
        min(a);
        max(a);
        return 0;
    }


<a id="org0cb0fe8"></a>

## std::arrays

    #include <iostream>
    #include <array>
    using namespace std;
    
    int main() {
        array<int, 5> a{};
        cout << a[0] << '\n';
    
        constexpr int len{8};
        array<int, len> b{};
        cout << b[1] << '\n';
    
        enum Colors {
            white,
            green,
            blue,
            black
        };
    
        array<int, black> c{};
        cout << b[10] << '\n';
    
        return 0;
    }

**Defining your std::array as constexpr whenever possible. if Your std::array is not a constexpr, consider using std::vector instead**

    #include <iostream>
    #include <array>
    using namespace std;
    
    int main() {
        array a1 {1,2,3,4};
        cout << a1[0];
        return 0;
    }


<a id="orgbd1b873"></a>

# Iterators

    #include <iostream>
    #include <array>
    using namespace std;
    
    int main() {
        array a{0,1,2,3,5,5};
    
        auto begin{&a[0]};
        auto end{begin + size(a)};
    
        for(auto ptr{begin};ptr != end;++ptr) {
            cout << *ptr << ' ';
        }
        return 0;
    }

    #include <iostream>
    #include <array>
    using namespace std;
    
    int main() {
        array a{0,1,2,3,4,5};
    
        auto begin{a.begin()};
        auto end{a.end()};
    
        for(auto ptr{begin}; ptr != end;++ptr) {
            cout << *ptr << ' ';
        }
        return 0;
    }


<a id="org1b7014c"></a>

# Introduction to standard library algorithms


<a id="org3b11276"></a>

## std::find - find an element by value

std::find searches for a first occurence of an element in a container.
 takes 3 parameters: an iterator to the starting element in the sequence, an iterator to the ending element in the sequence, and a value to search for. It returns an iterator pointing to the element (if it is found) or the end of the container (if the element is not found).

    #include <iostream>
    #include <array>
    #include <algorithm>
    using namespace std;
    
    int main() {
        array a{1,2,3,4,5,6};
        int ele{5};
        auto found{find(a.begin(), a.end(), ele)};
        if(found == a.end()) {
            cout << "element not found";
        }else {
            cout << *found << '\n';
        }
        return 0;
    }

iterators use or mimics the syntax of pointers to replace or see the value of element. But they are not actually pointers.


<a id="org948589b"></a>

## std::find<sub>if</sub> - find an element that matches some condition

    #include <iostream>
    #include <array>
    #include <string_view>
    #include <algorithm>
    using namespace std;
    
    bool contains(string_view str) {
        return str.find("sad") != string_view::npos;
    }
    
    int main() {
        array<string_view, 4> a{"shiva", "prasad", "kyaram", "sunny"};
    
        auto found {find_if(a.begin(), a.end(), contains)};
    
        if(found == a.end()) {
            cout << "Not found" << '\n';
        }else {
            cout << *found << '\n';
        }
    
        return 0;
    }


<a id="org0374628"></a>

## std::count and std::count<sub>if</sub> to count how many occurences there are

    #include <iostream>
    #include <string_view>
    #include <algorithm>
    #include <array>
    using namespace std;
    
    bool containsnut(string_view str) {
        return str.find("nut") != string_view::npos;
    }
    
    int main() {
        array<string_view, 5> a{"apple", "walnut", "peanut", "banana", "nut"};
    
        auto nuts {count_if(a.begin(), a.end(), containsnut)};
    
        cout << nuts << '\n';
    
        return 0;
    }


<a id="org3e5bec5"></a>

## std::sort

    #include <iostream>
    #include <array>
    #include <algorithm>
    using namespace std;
    bool greatest(int a, int b) {
        return (a>b);
    }
    
    int main() {
        array arr{1,7,4,6,2,6};
        sort(arr.begin(), arr.end(), greatest);
        for(int i : arr) {
            cout << i << ' ';
        }
        cout << '\n';
        return 0;
    }

    #include <iostream>
    #include <array>
    #include <algorithm>
    using namespace std;
    // bool greatest(int a, int b) {
    //     return (a<b);
    // }
    
    int main() {
        array arr{1,7,4,6,2,6};
        sort(arr.begin(), arr.end());
        for(int i : arr) {
            cout << i << ' ';
        }
        cout << '\n';
        return 0;
    }


<a id="orgc7e1e35"></a>

## std::for<sub>each</sub>

    #include <iostream>
    #include <array>
    #include <algorithm>
    using namespace std;
    
    void dou(int& i) {
        i = i*2;
    }
    
    int main() {
        array a{1,2,3,4};
        for_each(a.begin(), a.end(), dou);
    
        for(auto i : a) {
            cout << i << ' ';
        }
        cout << '\n';
        return 0;
    }

    #include <iostream>
    #include <array>
    #include <chrono> // for std::chrono functions
    
    using namespace std;
    class Timer
    {
    private:
    	// Type aliases to make accessing nested type easier
    	using Clock = std::chrono::steady_clock;
    	using Second = std::chrono::duration<double, std::ratio<1> >;
    
    	std::chrono::time_point<Clock> m_beg { Clock::now() };
    
    public:
    	void reset()
    	{
    		m_beg = Clock::now();
    	}
    
    	double elapsed() const
    	{
    		return std::chrono::duration_cast<Second>(Clock::now() - m_beg).count();
    	}
    };
    
    int main() {
        array a{12,3,4,5,6};
        Timer t;
        for(auto i : a) {
            cout << i << ' ';
        }
        cout << t.elapsed() << '\n';
        return 0;
    }


<a id="orgc83e858"></a>

# Dynamic memory allocation with new and delete


<a id="org38daea4"></a>

## new

    #include <iostream>
    using namespace std;
    
    int main() {
        new int a;
        return 0;
    }

In the above case, we’re requesting an integer’s worth of memory from the operating system. The new operator creates the object using that memory, and then returns a pointer containing the address of the memory that has been allocated.

    #include <iostream>
    using namespace std;
    
    int main() {
        int* ptr = new int;
        cout << *ptr << '\n';
    
        *ptr = 44;
        cout << *ptr << '\n';
    
        return 0;
    }

Note that accessing **heap-allocated** objects is generally slower than accessing stack-allocated objects. Because the compiler knows the address of stack-allocated objects, it can go directly to that address to get a value. Heap allocated objects are typically accessed via pointer. This requires two steps: **one to get the address of the object (from the pointer), and another to get the value.**

    #include <iostream>
    using namespace std;
    
    int main() {
        int* ptr{new int {9}};
        int* ptr1{new int {1}};
        cout << *ptr << '\n';
        cout << *ptr1 << '\n';
        return 0;
    }


<a id="org8005a8b"></a>

## delete

    #include <iostream>
    using namespace std;
    
    int main() {
        int* ptr {new int (9)};
        delete ptr;
        ptr = NULL;
        cout << *ptr << '\n';
        return 0;
    }

The delete operator does not actually delete anything. It simply returns the memory being pointed to back to the operating system. The operating system is then free to reassign that memory to another application (or to this application again later).

Although the syntax makes it look like we’re deleting a variable, this is not the case! The pointer variable still has the same scope as before, and can be assigned a new value (e.g. nullptr) just like any other variable.

Note that deleting a pointer that is not pointing to dynamically allocated memory may cause bad things to happen.

    int* value { new (std::nothrow) int{} }; // ask for an integer's worth of memory
    if (!value) // handle case where new returned null
    {
        // Do error handling here
        std::cerr << "Could not allocate memory\n";
    }

memory leak

    #include <iostream>
    using namespace std;
    
    int main() {
        {
            int* ptr{new int (5)};  //dynamically allocated int specific block
        }
        // ptr has been destroyed after the above block
        // but we never deallocated the memory so the os can now either access it or delete so it just becomes useless now;
    
        return 0;
    }


<a id="org392c459"></a>

# Dynamically allocating arrays

    #include <iostream>
    using namespace std;
    
    int main() {
        int length{3};
        int* ptr{new int[length]{}};
        ptr[0] = 1;
        cout << ptr[0];
        delete[] ptr;
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    int main() {
        size_t len=5;
        int* array {new int[len]{1,2,3,4,5}};
        cout << array[3];
        return 0;
    }

    #include <iostream>
    #include <algorithm>
    #include <string_view>
    using namespace std;
    
    // bool small(string_view a, string_view b) {
    //     return (a<b);
    // }
    
    int main() {
        size_t len;
        cout << "Enter the no of Names: " << '\n';
        cin >> len;
        auto *arr{new string[len]{}};
        for(size_t i = 0;i<len;i++) {
            getline(cin>>ws, arr[i]);
        }
    
        sort(arr, arr + len);
    
        for(size_t i= 0;i<len;i++){
            cout << arr[i] << '\n';
        }
    
        delete[] arr;
    
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    class Color{
    public:
        enum color {
            a,
            b,
            c,
            e,
            f
        };
    };
    
    int main() {
        Color::color o{};
        cout << o;
        cout << sizeof(o);
        return 0;
    }


<a id="orgdf12888"></a>

# Destructor indetail

A destructor is another special kind of class member function that is executed when an object of that class is destroyed. Whereas constructors are designed to initialize a class, destructors are designed to help clean up.

When an object goes out of scope normally, or a dynamically allocated object is explicitly deleted using the delete keyword, the class destructor is automatically called (if it exists) to do any necessary clean up before the object is removed from memory. For simple classes (those that just initialize the values of normal member variables), a destructor is not needed because C++ will automatically clean up the memory for you.

However, if your class object is holding any resources (e.g. dynamic memory, or a file or database handle), or if you need to do any kind of maintenance before the object is destroyed, the destructor is the perfect place to do so, as it is typically the last thing to happen before the object is destroyed.

    #include <iostream>
    using namespace std;
    
    class Array{
        int* m_ar{};
        int m_length{};
    public:
        Array(int length){
            m_ar = new int[static_cast<size_t>(length)]{};
            m_length = length;
        }
        ~Array() {
            delete[] m_ar;
        }
    
        void setValue(int index,int value) {
            m_ar[index] = value;
        }
    
        int getValue(int index) {
            return m_ar[index];
        }
    
        int getLength() {
            return m_length;
        }
    };
    
    int main() {
        Array ar(10);
        for(int i =0;i < ar.getLength(); i++) {
            ar.setValue(i,i+1);
        }
        cout << ar.getValue(2);
        return 0;
    } //ar is destroyed here


<a id="orgb884f31"></a>

# RAII[ link](https://share.gemini.google/3gFhyGLcNj3P)


<a id="org11e3be1"></a>

# Introduction to Lamdas (anonymous functions)

Syntax of Lamda function

[ captureClause ] ( parameters ) -> returnType
{
        statements;
}

Normal Function

    bool greater(int a, int b) {
        return a > b;
    }

Lamda function

    auto is_greater = [](int a,int b)
        {return a > b;};

    #include <iostream>
    #include <algorithm>
    #include <vector>
    using namespace std;
    
    int main() {
        vector<int> arr{1,2,3,4,5,6};
        int limit = 3;
    
        int count = count_if(arr.begin(), arr.end(), [limit](int n) {return n > limit;});
    
        cout << count;
    
        return 0;
    }

    #include <algorithm>
    #include <array>
    #include <iostream>
    #include <string_view>
    
    int main()
    {
      constexpr std::array<std::string_view, 4> arr{ "apple", "banana", "walnut", "lemon" };
    
      // Define the function right where we use it.
      auto found{ std::find_if(arr.begin(), arr.end(),
                               [](std::string_view str) // here's our lambda, no capture clause
                               {
                                 return str.find("nut") != std::string_view::npos;
                               }) };
    
      if (found == arr.end())
      {
        std::cout << "No nuts\n";
      }
      else
      {
        std::cout << "Found " << *found << '\n';
      }
    
      return 0;
    }

we can store lamda in a named variable and pass it to a function.

    auto isEven{
        [](int i)
        {
            return (i % 2) == 0;
        }
    };
    
    return std::all_of(array.begin(),array.end(),isEven);

Storing a lamda for post-defination

    #include <iostream>
    #include <functional>
    using namespace std;
    
    int main() {
        //using functional pointer
        double (*addnumbers1)(double, double) {
            [](double a,double b) {
                return a+b;
            }
        };
    
        cout << addnumbers1(1,2) << '\n';
    
        //using std::function
        function addnumbers2{
            [](double a, double b) {
                return a + b;
            }
        };
    
        cout << addnumbers2(5,6) << '\n';
    
        //using auto
        auto addnumbers3 {
            [](double a, double b) {
                return a + b;
            }
        };
    
        cout << addnumbers3(1,6) << '\n';
    
        return 0;
    }

passing lamda to a function
example of passing  a function as parameter to another function

    #include <iostream>
    using namespace std;
    
    int add(int a, int b) { return a + b; }
    int mul(int a, int b) { return a * b; }
    
    int apply(int x, int y, int (*op)(int, int)) {
        return op(x, y);
    }
    
    int main() {
        cout << apply(3, 4, add) << "\n";  // 7
        cout << apply(3, 4, mul) << "\n";  // 12
    }

now using lamda

    #include <iostream>
    #include <functional>
    using namespace std;
    //using std::function parameter
    void repeat(int n, const function<void(int)>& fn) {
        for(int i = 0; i < n;i++) {
            fn(i);
        }
    }
    
    //using template
    template <typename T>
    void repeat2(int n, const T& fn) {
        for(int i = 0; i < n ; i++){
            fn(i);
        }
    }
    
    int main() {
    
        auto lamda{
            [](int i) {
                cout << i << ' ';
            }
        };
    
        repeat(3,lamda);
        repeat2(3,lamda);
    
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    void repeat(int n, print()) {
        for(int i =0; i < n; i++){
            print(i);
        }
    }
    
    int print(int i) {
        cout << i;
    }
    
    int main() {
    
        return 0;
    }


<a id="org2c9569a"></a>

## Generic Lamdas

Lamdas woth one or more auto type parameters which works with wide variety of types are called generic lamdas

The std::adjacent<sub>find</sub> function in C++ searches a range [first, last) for the first pair of consecutive elements that are equal (or satisfy a given binary predicate), returning an iterator to the first element of that pair.  If no such pair is found, it returns the last iterator.

Syntax and Parameters
Defined in the <algorithm> header, the function has two primary overloads:

Equality Check: std::adjacent<sub>find</sub>(first, last) compares elements using operator==.
Predicate Check: std::adjacent<sub>find</sub>(first, last, pred) uses a binary predicate pred to determine if two elements match.

    #include <iostream>
    #include <array>
    #include <algorithm>
    #include <string_view>
    using namespace std;
    
    int main() {
        constexpr array month {
            "January",
            "February",
            "March",
            "April",
            "May",
            "June",
            "July",
            "August",
            "September",
            "October",
            "November",
            "December"
        };
    
         const auto sameletter{adjacent_find(month.begin(), month.end(),
                                             [](const auto& a,const auto& b){
                                                 return (a[0] == b[0]);
        })};
        if(sameletter != month.end()) {
            cout << *sameletter << " and " << *next(sameletter) << " are equal";
        }
    
        return 0;
    }

    #include <iostream>
    #include <array>
    #include <algorithm>
    #include <string_view>
    using namespace std;
    
    int main() {
        constexpr array month {
            "January",
            "February",
            "March",
            "April",
            "May",
            "June",
            "July",
            "August",
            "September",
            "October",
            "November",
            "December"
        };
    
        auto fiveletter{
            count_if(month.begin(), month.end(),
                [](std::string_view str) {
                return (str.length() == 5);
                })};
    
        cout << fiveletter << '\n';
    }


<a id="org519ff62"></a>

# Operator overloading.

using function overloading to overload operators is called operator overloading.i

First, almost any existing operator in C++ can be overloaded. The exceptions are: conditional (?:), sizeof, scope (::), member selector (.), pointer member selector (.\*), typeid, and the casting operators.

Second, you can only overload the operators that exist. You can not create new operators or rename existing operators. For example, you could not create an operator\*\* to do exponents.

Third, at least one of the operands in an overloaded operator must be a user-defined type. This means you could overload operator+(int, Mystring), but not operator+(int, double).

**Ways to overload operator**

1.  the member function way
2.  friend function way
3.  normal way


<a id="org3fd0522"></a>

## opearator overloading using friend function\*

    #include <iostream>
    using namespace std;
    
    class Cents{
        int m_cents{};
    public:
        Cents(int cents) : m_cents {cents} {}
    
        friend Cents operator+(Cents& c1, Cents& c2);
    
        int getCents() {
           return m_cents;
        }
    };
    
    Cents operator+(Cents& c1, Cents& c2) {
        return c1.m_cents + c2.m_cents;
    }
    
    
    int main() {
        Cents a{1};
        Cents b{2};
        cout << a.getCents() << '\n';
        Cents sum{a + b};
        cout  << sum.getCents() << '\n';
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    class Cents{
        int m_cents{};
    public:
        Cents(int cents) : m_cents{cents} {}
    
        friend Cents operator-(Cents& c1, Cents& c2);
    
        int getCents() {
            return m_cents;
        }
    };
    
    Cents operator-(Cents& c1, Cents& c2) {
        return c1.m_cents - c2.m_cents;
    }
    
    int main() {
        Cents a{2};
        Cents b{3};
        cout << b.getCents() << '\n';
        Cents minus{a- b};
        cout << minus.getCents() << '\n';
        return 0;
    }

with different type
Cents, int

For adding different types we need to write two oveloading functions one for  x + cents(4) and cents(4) + x because these are treated as diff rather than one like in same type.

    #include <iostream>
    using namespace std;
    class Cents{
        int m_cents{};
    public:
        Cents(int cents) : m_cents {cents} {}
    
        friend Cents operator+(Cents& c, int x);
    
        friend Cents operator+(int x, Cents& c);
    
        int getCents() {
            return m_cents;
        }
    };
    
    Cents operator+(Cents& c, int x) {
        return c.m_cents + x;
    }
    
    Cents operator+(int x, Cents& c) {
        return c.m_cents + x;
    }
    
    int main() {
        Cents a{3};
        Cents sum=a+4;
        cout << sum.getCents();
        return 0;
    }


<a id="org3668b9a"></a>

## overloading operator using normal functions

    #include <iostream>
    using namespace std;
    
    class Cents{
        int m_cents{};
    public:
        Cents(int cents) : m_cents{cents} {}
    
        int getCents() {
            return m_cents;
        }
    };
    
    Cents operator+(Cents& c1, Cents& c2) {
        return (c1.getCents() + c2.getCents());
    }
    
    int main() {
        Cents a{2};
        Cents b{3};
        Cents sum{a + b};
        cout << sum.getCents();
        return 0;
    }


<a id="orgadb4f89"></a>

## overloading I/O operators

overloading >> operator

    #include <iostream>
    using namespace std;
    
    class Cents{
        int m_cents{};
        string m_country{};
    public:
        Cents(int cents, string country) : m_cents {cents}, m_country {country} {};
    
        friend ostream& operator<<(ostream& out, Cents& c);
    
        int getCents() {
            return m_cents;
        }
    };
    
    ostream& operator<<(ostream& out, Cents& c) {
        out << c.m_cents << ' '  << c.m_country;
        return out;
    }
    
    int main() {
        Cents a{20, "India"};
        cout << a;
        return 0;
    }

    #include <iostream>
    using namespace std;
    
    class Point{
        int m_x{};
        int m_y{};
        int m_z{};
    public:
        Point(int x= 0, int y=0 , int z=0) : m_x {x}, m_y{y} , m_z{z} {};
    
        friend ostream& operator<<(ostream& out, Point& p);
        friend istream& operator>>(istream& out, Point& p);
    };
    
    ostream& operator<<(ostream& out, Point& p) {
        out << "( " << p.m_x << ", " << p.m_y << ", " << p.m_z << " )";
        return out;
    }
    
    istream& operator>>(istream& in, Point& p) {
        in >> p.m_x >> p.m_y >> p.m_z;
        return in;
    }
    
    int main() {
        Point p;
        cin >> p;
        cout << p;
        return 0;
    }


<a id="orgb7e8457"></a>

## overloading operators using member function

    #include <iostream>
    using namespace std;
    
    class Cents{
        int m_cents{};
    public:
        Cents(int cents) : m_cents{cents} {}
    
        int getCents() {
            return m_cents;
        }
    };
    
    Cents Cents::operator+(int value) {
        return Cents {m_cents + value};
    }
    
    int main() {
    
        Cents c1{1};
        Cents c2{c1 + 1};
        cout << c2.getCents();
    
        return 0;
    }


<a id="orgca2a2d7"></a>

## overloading unary operators +,-,!

    #include <iostream>
    using namespace std;
    
    class Cents{
        int  m_cents{};
    public:
        Cents(int cents) : m_cents{cents}{}
        Cents operator-();
    
        int getCents() {
            return m_cents;
        }
    };
    
    Cents Cents::operator-() {
        return -m_cents;
    }
    
    int main() {
        Cents c{2};
        cout << -c.getCents();
        return 0;
    }


<a id="orgccdd612"></a>

## overloading comparison operators

    #include <iostream>
    using namespace std;
    
    class Car{
        string m_make{};
        string m_model{};
    public:
        Car(string make, string model) : m_make {make} , m_model {model} {}
    
        friend bool operator==(Car& c1, Car& c2);
        friend bool operator!=(Car& c1, Car& c2);
    };
    
    bool operator==(Car& c1, Car& c2) {
        return (c1.m_make == c2.m_make && c1.m_model == c2.m_model);
    }
    
    bool operator!=(Car& c1, Car& c2) {
        return (c1.m_make != c2.m_make || c1.m_model != c2.m_model);
    }
    
    int main() {
        Car c1{"Toyota", "A"};
        Car c2("Toyota", "B");
        if(c1 == c2) {
            cout << "Equal" << '\n';
        }else {
            cout << "Not equal" << '\n';
        }
        return 0;
    }


<a id="org27dd1d7"></a>

## overloading operator[]

    #include <iostream>
    
    class IntList
    {
    private:
        int m_list[10]{};
    
    public:
        int& operator[] (int index)
        {
            return m_list[index];
        }
    };
    
    /*
    // Can also be implemented outside the class definition
    int& IntList::operator[] (int index)
    {
        return m_list[index];
    }
    */
    
    int main()
    {
        IntList list{};
        list[2] = 3; // set a value
        std::cout << list[2] << '\n'; // get a value
    
        return 0;
    }


<a id="org2ed8f47"></a>

## shallow vs deep copying

    #include <cassert>
    #include <iostream>
    
    class Fraction
    {
    private:
        int m_numerator { 0 };
        int m_denominator { 1 };
    
    public:
        // Default constructor
        Fraction(int numerator = 0, int denominator = 1)
            : m_numerator{ numerator }
            , m_denominator{ denominator }
        {
            assert(denominator != 0);
        }
    
        // Possible implementation of implicit copy constructor
        Fraction(const Fraction& f)
            : m_numerator{ f.m_numerator }
            , m_denominator{ f.m_denominator }
        {
        }
    
        // Possible implementation of implicit assignment operator
        Fraction& operator= (const Fraction& fraction)
        {
            // self-assignment guard
            if (this == &fraction)
                return *this;
    
            // do the copy
            m_numerator = fraction.m_numerator;
            m_denominator = fraction.m_denominator;
    
            // return the existing object so we can chain this operator
            return *this;
        }
    
        friend std::ostream& operator<<(std::ostream& out, const Fraction& f1)
        {
         out << f1.m_numerator << '/' << f1.m_denominator;
         return out;
        }
    };

    #include <iostream>
    using namespace std;
    
    class Something{
    public:
        int* m_data;
        Something(int data) {
            m_data = new int(data);
        }
        ~Something() {
            delete m_data;
        }
    };
    
    int main() {
        Something S{20};
        Something R = S;
        cout << *R.m_data << '\n';
        return 0;
    }


<a id="orgc7ea5c6"></a>

# Smart pointers

    #include <iostream>
    using namespace std;
    
    template <typename T>
    class Auto_ptr{
        T* m_ptr;
    public:
        Auto_ptr(T* ptr= nullptr) : m_ptr{ptr} {}
    
        ~Auto_ptr() { delete m_ptr; }
    
        T& operator*() const {return *m_ptr;}  // returns the actual resource object
        T* operator->() const {return m_ptr;}  // returns raw pointer m_ptr
    };
    
    class Resource{
        string m_name{};
        int m_data{};
    public:
        Resource(string name, int data) : m_name{name} , m_data {data} {cout << "constructor ran\n";}
        ~Resource() {{cout << "Destructor ran\n";}}
    
        void print() {
            cout << m_name << " " << m_data << '\n';
        }
    };
    
    int main() {
        Auto_ptr<Resource> res = new Resource("Shiva", 20);
        res->print();
        return 0;
    }

Exaplanation from claude

    #include <iostream>
    #include <string>
    
    template <typename T>
    class Auto_ptr1
    {
        T* m_ptr {};
    public:
        Auto_ptr1(T* ptr = nullptr) : m_ptr(ptr) {}
        ~Auto_ptr1() { delete m_ptr; }
    
        T& operator*() const { return *m_ptr; }
        T* operator->() const { return m_ptr; }
    };
    
    class Resource
    {
        std::string m_name;
        int m_health;
    public:
        Resource(std::string name, int health)
            : m_name(name), m_health(health)
        {
            std::cout << m_name << " created with health " << m_health << "\n";
        }
    
        ~Resource() { std::cout << m_name << " destroyed\n"; }
    
        void takeDamage(int dmg) { m_health -= dmg; }
        void show() const { std::cout << m_name << " health: " << m_health << "\n"; }
    };
    
    int main()
    {
        std::cout << "main starts\n";
    
        {   // inner scope
            Auto_ptr1<Resource> player(new Resource("Player", 100));
    
            player->show();        // calls m_ptr->show()
            player->takeDamage(30);
            player->show();
            (*player).show();      // same thing using operator*
    
            std::cout << "leaving inner scope\n";
        }   // player (the Auto_ptr1) dies here -> delete m_ptr -> Resource destructor runs
    
        std::cout << "back in main, player is gone\n";
    }


<a id="org7096705"></a>

## move semantics

What if, instead of having our copy constructor and assignment operator copy the pointer (“copy semantics”), we instead transfer/move ownership of the pointer from the source to the destination object? This is the core idea behind move semantics. Move semantics means the class will transfer ownership of the object rather than making a copy

    #include <iostream>
    using namespace std;
    
    template <typename T>
    class Auto_ptr{
        T* m_ptr{};
    public:
        Auto_ptr(T* ptr = nullptr) : m_ptr {ptr} {}
    
        ~Auto_ptr() {
            delete m_ptr;
        }
    
        Auto_ptr& operator=(Auto_ptr& a) {
            if(&a == this) {
                return *this;
            }
            delete m_ptr;
            m_ptr = a.m_ptr;
            a.m_ptr = nullptr;
            return *this;
        }
    
        T& operator*() {return *m_ptr;}
        T* operator->() {return m_ptr;}
    };
    
    class Resource{
        int m_data;
    public:
        Resource(int data) : m_data {data} {cout << "Constrouctor ran\n";}
        void getData() {
            cout << m_data << '\n';
        }
        ~Resource() {cout << "Destrouctor ran\n";}
    };
    
    int main() {
        Auto_ptr<Resource> res1 = new Resource(10);
        Auto_ptr<Resource> res2;
        res2 = res1;
        res2->getData();
        return 0;
    }

**rvalue reference** - the rvalue reference allows to capture temporary object in the move constructor and move its resources to another object.

**move constructor** - Allows stealing resources from a temporary object and provide those resources to some other object.

    #include <iostream>
    #include <cstring>
    using namespace std;
    
    class String{
        char* m_data;
    public:
        // Constructor
        String(const char* s)  {
            m_data = new char[strlen(s) + 1]; // + 1 for terminator
            strcpy(m_data, s);
            cout << "Constructed" << '\n';
        }
    
        //Copy construtor
        String(const String& other)  {
            m_data = new char[strlen(other.m_data) + 1];
            strcpy(m_data , other.m_data);
            cout << "copied" << '\n';
        }
    
        //Destructor
        ~String() {
            delete[] m_data;
            cout << "Destroyed" << '\n';
        }
    
        void print() {
            cout << m_data << '\n';
        }
    };
    
    int main() {
        String s1{"shiva"};
        String s2 = s1;
        s1.print();
        s2.print();
        return 0;
    }

In the above program we just copied one object data to another using copy constructor with this two strings will be created and memory is occupied by both.
Lets see how this is done by move constructor using rvalue references

    #include <iostream>
    #include <cstring>
    using namespace std;
    
    class String{
        char* m_data{};
    public:
        String(const char* s) {
            m_data = new char[strlen(s) + 1];
            strcpy(m_data, s);
            cout << "Constructed" << '\n';
        }
    
        //move constructor
        String(String&& other) {  // here we used && because in the main s1 is treated as temporary object which is rvalue
            m_data = other.m_data;  // here s1 and s2 are pointing to same data because of reference
            other.m_data = nullptr;  // set data of s1 to null
            cout << "Moved\n";
        }
    
        ~String() {
            delete[] m_data;
            cout << "Destroyed" << '\n';
        }
    
        void print() {
            if(m_data) {
                cout << m_data << "\n";
            }else{
                cout << "Empty" << '\n';
            }
        }
    };
    
    int main() {
        String s1{"shiva"};
        String s2 = move(s1);  // here s1 is treated as a temporary object
        s1.print();
        s2.print();
        return 0;
    }

