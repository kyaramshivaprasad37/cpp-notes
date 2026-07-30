
# Table of Contents

1.  [C++ Basics](#org2f2a857)
    1.  [Objects and Variables](#org5d3b60a)
        1.  [Variable assigment](#org1daebad)
        2.  [maybe unused](#org3fa717a)
        3.  [cout and cin](#org8375dc9)
        4.  [Uninitialized variables and undefined behavioure](#org15e175b)
        5.  [Keywords and Identifiers](#org602fa76)
    2.  [Functions and Files](#orgab1df8a)
        1.  [Void functions](#orgbc6fff9)
    3.  [size<sub>t</sub> link to topic](#orge9bb897)
    4.  [Char(ASCII TABLE LINK) here](#orgbe77678)
    5.  [Implicit and Explicit Coversion](#org534ffdf)
        1.  [Sign conversion using static<sub>cast</sub>](#orgf3c394f)
        2.  [Quiz Questions](#orged0aae1)
2.  [Fundamental Data Types](#orgb7eb5a2)
    1.  [Numeral Systems (decimal, binary, hexadecimal)](#org8d0791f)
        1.  [Octal](#orgbd7925c)
        2.  [hexadecimal](#org8c6f1c3)
        3.  [Binary](#orgc51f97d)
        4.  [Outputting values in decimal, octal and hexadecimal](#orgf0af727)
        5.  [Outputting values in Binary using std::bitset](#org5d28953)
3.  [Strings](#org2fcaab5)
    1.  [Strings (std::string)](#orgd255c44)
    2.  [Strings (std::string<sub>view</sub>)](#org2d76be8)
4.  [Operators](#org9dba00f)
5.  [Bit Manipulation](#orgadd5df5)
    1.  [Uses of <bitset> library](#orgb3ed89d)
    2.  [Bitmanipulation by bit masks](#org6cad92b)
6.  [Namespace and scope resolution](#orgc96ed56)
    1.  [Static local variables](#org562a8d5)
7.  [Control Flow](#org1b61556)
    1.  [Switch case](#orgd07e2b1)
    2.  [goto statements](#orgc4d38a6)
    3.  [While loop](#org369dfa3)
    4.  [Do While](#org11bdbea)
    5.  [For Loop](#org478623e)
    6.  [std::exit](#org43b8354)
8.  [Mersenne Twister](#orgc149021)
9.  [Function Templates](#org6706983)
10. [Constexpr and Consteval Functions](#org82cba16)
11. [Compound data types](#org8d422e7)
    1.  [L-value references](#org8ebda4c)
        1.  [Non-const L value references](#orgcc743fe)
        2.  [Const L-value referencs](#orgaa6e0f6)
    2.  [Pass by reference](#orgfb333c7)
    3.  [pass by const lvalue reference](#orgc43e82a)
    4.  [why prefer std::string<sub>view</sub> to const std::string&](#org5b1917f)
    5.  [Pointers](#orgda01cd2)
        1.  [Deference operator](#orge5a20a6)
        2.  [Pointer](#org7f6a0a1)
        3.  [Address of operator returns a pointer](#org3be4a2e)
        4.  [null pointers as boolean values](#orgb42b231)
        5.  [pointer to const](#orgb146ffc)
        6.  [pass by address](#org8ccc027)
    6.  [Operator overloading](#org0598a61)
    7.  [Enumerations](#org2e080fd)
        1.  [Unscoped Enumerations](#org9628e9a)
        2.  [scoped Enumerations](#org068d341)
    8.  [Struct](#org06ad57b)
    9.  [Classes (OOP)](#orgc1a890c)
        1.  [member functions](#orgab24533)
        2.  [returning data members by lvalue reference](#org76e9e08)
        3.  [constructor](#org6eac825)
        4.  [temporary object](#orgd42c3ef)

filetags: CPP


<a id="org2f2a857"></a>

# C++ Basics


<a id="org5d3b60a"></a>

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


<a id="org1daebad"></a>

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


<a id="org3fa717a"></a>

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


<a id="org8375dc9"></a>

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


<a id="org15e175b"></a>

### Uninitialized variables and undefined behavioure

Returns garbage value -&#x2014;> Memory address

    #include <iostream>
    
    int main() {
        int x;
        std::cout << x << '\n';
        return 0;
    }


<a id="org602fa76"></a>

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


<a id="orgab1df8a"></a>

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


<a id="orgbc6fff9"></a>

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


<a id="orge9bb897"></a>

## size<sub>t</sub>[ link to topic](https://www.learncpp.com/cpp-tutorial/fixed-width-integers-and-size-t/)


<a id="orgbe77678"></a>

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


<a id="org534ffdf"></a>

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


<a id="orgf3c394f"></a>

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


<a id="orged0aae1"></a>

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


<a id="orgb7eb5a2"></a>

# Fundamental Data Types


<a id="org8d0791f"></a>

## Numeral Systems (decimal, binary, hexadecimal)


<a id="orgbd7925c"></a>

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


<a id="org8c6f1c3"></a>

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


<a id="orgc51f97d"></a>

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


<a id="orgf0af727"></a>

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


<a id="org5d28953"></a>

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


<a id="org2fcaab5"></a>

# Strings


<a id="orgd255c44"></a>

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


<a id="org2d76be8"></a>

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


<a id="org9dba00f"></a>

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


<a id="orgadd5df5"></a>

# Bit Manipulation


<a id="orgb3ed89d"></a>

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


<a id="org6cad92b"></a>

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


<a id="orgc96ed56"></a>

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


<a id="org562a8d5"></a>

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


<a id="org1b61556"></a>

# Control Flow


<a id="orgd07e2b1"></a>

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


<a id="orgc4d38a6"></a>

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


<a id="org369dfa3"></a>

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


<a id="org11bdbea"></a>

## Do While


<a id="org478623e"></a>

## For Loop


<a id="org43b8354"></a>

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


<a id="orgc149021"></a>

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


<a id="org6706983"></a>

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


<a id="org82cba16"></a>

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


<a id="org8d422e7"></a>

# Compound data types

<div class="mindmap" id="orgf1a82c1">
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


<a id="org8ebda4c"></a>

## L-value references


<a id="orgcc743fe"></a>

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


<a id="orgaa6e0f6"></a>

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


<a id="orgfb333c7"></a>

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


<a id="orgc43e82a"></a>

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


<a id="org5b1917f"></a>

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


<a id="orgda01cd2"></a>

## Pointers


<a id="orge5a20a6"></a>

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


<a id="org7f6a0a1"></a>

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


<a id="org3be4a2e"></a>

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


<a id="orgb42b231"></a>

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


<a id="orgb146ffc"></a>

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


<a id="org8ccc027"></a>

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


<a id="org0598a61"></a>

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


<a id="org2e080fd"></a>

## Enumerations

Enumerations are implicitly constexpr.


<a id="org9628e9a"></a>

### Unscoped Enumerations

Each enumeration is numbered from 0. We can explicitly number a enumeration, any undefined enumeration will be given one value greater than the previous one.

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


<a id="org068d341"></a>

### scoped Enumerations

    #include <iostream>
    using namespace std;
    
    enum class Color {white, red, green};
    
    int main() {
        Color color {Color::white};
    
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


<a id="org06ad57b"></a>

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


<a id="orgc1a890c"></a>

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


<a id="orgab24533"></a>

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


<a id="org76e9e08"></a>

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


<a id="org6eac825"></a>

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


<a id="orgd42c3ef"></a>

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

