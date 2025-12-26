# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 26.12.2025
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
```
#include<stdio.h>
int main()
{
    int a=10;
    float b=65.78;
    char c='A';
    char d[]="Hello C";
    printf("Integer Literal: %d ",a);
    printf("Size: %d\n",sizeof(a));
    printf("Float Literal: %.2f ",b);
    printf("Size: %d\n",sizeof(b));
    printf("Character Literal: %c ",c);
    printf("Size: %d\n",sizeof(c));
    printf("String Literal: %s ",d);
    printf("Size: %d",sizeof(d));
    return 0;
}
```
# Output:
<img width="440" height="173" alt="image" src="https://github.com/user-attachments/assets/0ccbc061-8221-41a5-b5b2-cbba3ea0a89c" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 26.12.2025
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
```
#include<stdio.h>
#define pi 3.14159
int main()
{
    int days=7;
    printf("Macro Constant PI= %f\n",pi);
    printf("Constant Days= %d",days);
    return 0;
}
```
# Output:
<img width="457" height="154" alt="image" src="https://github.com/user-attachments/assets/b3b93faa-94d7-4a89-9d4d-a35f5ebff362" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 26.12.2025
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
```
#include<stdio.h>
int main()
{
    int a=100;
    float b=78.56;
    double c=345.7864;
    char d='C';
    printf("Integer value: %d\n",a);
    printf("Float value: %.2f\n",b);
    printf("Double value: %.4lf\n",c);
    printf("Character value: %c\n",d);
    return 0;
}
```
# Output:
<img width="476" height="211" alt="image" src="https://github.com/user-attachments/assets/4ad0f42b-ef0f-4d27-a3a8-e13fb0b25d9e" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 26.12.2025
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
```
#include<stdio.h>
int main()
{
    int a,b;
    printf("Enter two integers: ");
    scanf("%d %d",&a,&b);
    printf("\n-------ARITHMETIC OPERATIONS-------\n");
    printf("Addition: %d + %d = %d\n",a,b,a+b);
    printf("Subtraction: %d - %d = %d\n",a,b,a-b);
    printf("Multiplication: %d * %d = %d\n",a,b,a*b);
    printf("Quotient: %d / %d = %d\n",a,b,a/b);
    printf("Remainder: %d %% %d = %d\n\n",a,b,a%b);
    printf("-------BITWISE OPERATIONS-------\n");
    printf("AND: %d & %d = %d\n",a,b,a&b);
    printf("OR: %d | %d = %d\n",a,b,a|b);
    printf("XOR: %d ^ %d = %d\n",a,b,a^b);
    printf("Left Shift: %d << %d = %d\n",a,b,a<<b);
    printf("Right Shift: %d >> %d = %d\n",a,b,a>>b);
    printf("NOT (~a): %d\n",~a);
    printf("NOT (~b): %d\n",~b);
    return 0;
}
```
# Output:
<img width="591" height="560" alt="image" src="https://github.com/user-attachments/assets/61b3c47e-6f47-46d8-90bc-f1b58c99920f" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 26.12.2025
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
#include <stdio.h>
int main()
{
    char ch;
    scanf("%c", &ch);
    (ch >= '0' && ch <= '9') ? printf("DIGIT") :
    ((ch >= 'a' && ch <= 'z') || (ch >= 'A' && ch <= 'Z')) ?
        ((ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u'||
          ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U') ?
            printf("VOWEL") : printf("CONSONANT"))
    : printf("SPECIAL CHARACTER");
    return 0;
}
# Output:
<img width="418" height="138" alt="image" src="https://github.com/user-attachments/assets/86544c28-3d5e-4d3f-b46d-ae3125ce2888" />
<img width="396" height="131" alt="image" src="https://github.com/user-attachments/assets/99f5d3a8-81cd-4def-bcd8-967cfb008dd0" />
<img width="397" height="125" alt="image" src="https://github.com/user-attachments/assets/7884b4d0-99fb-4543-a5ca-a7d19449adc2" />
<img width="400" height="133" alt="image" src="https://github.com/user-attachments/assets/f89b3171-dd88-40fb-adc6-2f7740c8618b" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


