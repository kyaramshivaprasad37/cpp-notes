
# Table of Contents

1.  [C++ Basics](#org5ce41f1)
    1.  [Objects and Variables](#org36c0b20)
        1.  [Variable assigment](#org9aa1da9)
        2.  [maybe unused](#org33e55af)
        3.  [cout and cin](#org4f6319c)
        4.  [Uninitialized variables and undefined behavioure](#orge5896dc)
        5.  [Keywords and Identifiers](#org803542d)
    2.  [Functions and Files](#org58615f6)
        1.  [Void functions](#org3aa03dc)
    3.  [size<sub>t</sub> link to topic](#orgac7389c)
    4.  [Char(ASCII TABLE LINK) here](#orgdd9affb)
    5.  [Implicit and Explicit Coversion](#orgc5d690d)
        1.  [Sign conversion using static<sub>cast</sub>](#orgb853944)
        2.  [Quiz Questions](#org365fabb)
2.  [Fundamental Data Types](#orgf6c1d96)
    1.  [Numeral Systems (decimal, binary, hexadecimal)](#orgcbd8f93)
        1.  [Octal](#orge1e6bd6)
        2.  [hexadecimal](#org8cfcbc4)
        3.  [Binary](#orgea1a8ec)
        4.  [Outputting values in decimal, octal and hexadecimal](#org47d96e8)
        5.  [Outputting values in Binary using std::bitset](#org023e152)
3.  [Strings](#org3479492)
    1.  [Strings (std::string)](#org9b651d7)
    2.  [Strings (std::string<sub>view</sub>)](#orgfa59d85)
4.  [Operators](#org3179013)
5.  [Bit Manipulation](#org4ff886c)

filetags: CPP


<a id="org5ce41f1"></a>

# C++ Basics


<a id="org36c0b20"></a>

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


<a id="org9aa1da9"></a>

### Variable assigment

    #include <iostream>
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


<a id="org33e55af"></a>

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


<a id="org4f6319c"></a>

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


<a id="orge5896dc"></a>

### Uninitialized variables and undefined behavioure

Returns garbage value -&#x2014;> Memory address

    #include <iostream>
    
    int main() {
        int x;
        std::cout << x << '\n';
        return 0;
    }


<a id="org803542d"></a>

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


<a id="org58615f6"></a>

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


<a id="org3aa03dc"></a>

### Void functions

    #include <iostream>
    
    void printHi()
    {
        std::cout << "Hi" << '\n';
    }
    
    int main() {
    
        //printHi();
        std::cout << printHi() << '\n';
        printf()
            printf()printf(jsbcb)print()
        return 0;printf
    }

    #include <iostream>
    
    int main() {
    
        unsigned short a{0};
        std::cout << a << '\n';
    
        a = -4;
        std::cout << a << '\n';
    
        return 0;
    }


<a id="orgac7389c"></a>

## size<sub>t</sub>[ link to topic](https://www.learncpp.com/cpp-tutorial/fixed-width-integers-and-size-t/)

    #include <iostream>
    
    int main(){
        bool a = 0;
        bool b = 30;
    
        std::cout << a << '\n';
        std::cout << b << '\n';
        return 0;
    }


<a id="orgdd9affb"></a>

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


<a id="orgc5d690d"></a>

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


<a id="orgb853944"></a>

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


<a id="org365fabb"></a>

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


<a id="orgf6c1d96"></a>

# Fundamental Data Types


<a id="orgcbd8f93"></a>

## Numeral Systems (decimal, binary, hexadecimal)


<a id="orge1e6bd6"></a>

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


<a id="org8cfcbc4"></a>

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


<a id="orgea1a8ec"></a>

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


<a id="org47d96e8"></a>

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


<a id="org023e152"></a>

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


<a id="org3479492"></a>

# Strings


<a id="org9b651d7"></a>

## Strings (std::string)

The header <string> helps to input and output stings of different size

    #include <iostream>
    using namespace std;
    
    int main() {
        string name {"Shiva"};
        cout << name << '\n';
    
        name = "Prasad37";
        cout << name << '\n';
    
        return 0;
    }


<a id="orgfa59d85"></a>

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


<a id="org3179013"></a>

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


<a id="org4ff886c"></a>

# Bit Manipulation

Uses of <bitset> library

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

[Quiz
](https://www.learncpp.com/cpp-tutorial/bitwise-operators/)

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

