# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
## 3. Implementation of programs using conditional statements.
## 4. Implementation of programs using various control statements.
# Ex.No:6
  Build a C program to input a student’s marks in three subjects (Math, Science, and English). Calculate the average marks and determine the grade using nested if-else statements with safe floating-point comparisons based on the following grading criteria:
    
  A: 90 and above
  
  B: 75 to 89.99
  
  C: 50 to 74.99
  
  F: below 50
  
  The program should display the average marks up to two decimal places and the corresponding grade. 
  
# Date : 18-05-2026.
# Aim:
 To build a C program that receives inputs for a student’s marks in three subjects, calculates the average, and determines the grade using nested if-else statements with safe floating-point comparisons.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare float variables math, science, english to store marks of each subject.
### Step 4: 
  Declare a float variable average to store the average marks.
### Step 5: 
  Prompt the user to enter marks for Math, Science, and English.
### Step 6: 
  Read the input marks.
### Step 7: 
  Calculate the average marks using the formula:
   
  average=(math + science + english​)/3.0f
### Step 8: 
  Check if average is greater than or equal to 90.0f

  If yes, print Grade A.

  Else, proceed to Step 9.  
### Step 9:
  Check if average is greater than or equal to 75.0f

  If yes, print Grade B.

  Else, proceed to Step 10.
### Step 10:
  Check if average is greater than or equal to 50.0f

  If yes, print Grade C.

  Else, print Grade F.
### Step 11:
  Stop
# Program:
```
#include <stdio.h>
int main() {
    float math, science, english, average;
    scanf("%f %f %f", &math, &science, &english);
    average = (math + science + english) / 3.0f;
    printf("Average Marks: %.2f\n", average);
    if (average >= 90.0f) {
        printf("Grade: A\n");
    } else {
        if (average >= 75.0f) {
            printf("Grade: B\n");
        } else {
            if (average >= 50.0f) {
                printf("Grade: C\n");
            } else {
                printf("Grade: F\n");
            }
        }
    }
}
```
# Output:
<img width="228" height="121" alt="image" src="https://github.com/user-attachments/assets/2eee1d74-7f02-415c-8351-32008fb8fc64" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
# Ex.No:7
  Develop a C program to display the multiplication table of a given number (15) up to 10.
# Date : 18-05-2026.
# Aim:
 To develop a C program that prints the multiplication table of the number 15 up to 10 using a for loop.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare an integer variable number and initialize it with 15.
### Step 4: 
  Declare another integer variable i to use as a loop counter.
### Step 5: 
  Use a for loop to iterate from i = 1 to i = 10.
  
  In each iteration:
  
  a. Multiply number by i.
  
  b. Print the result in the format: number x i = result.
### Step 6: 
  Stop

# Program:
```
#include <stdio.h>
int main() {
    int num = 15;
    printf("Multiplication Table of %d:\n", num);
    for (int i = 1; i <= 10; i++) {
        printf("%d x %d = %d\n", num, i, num * i);
    }

    return 0;
}
```
# Output:
<img width="257" height="249" alt="image" src="https://github.com/user-attachments/assets/cf6bca7e-ee9d-4fa1-b10d-0d43f2948e3f" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
# Ex.No:8
  Develop a C program to check whether a given number is prime or not.
# Date : 18-05-2026.
# Aim:
 To develop a C program that determines whether an input number is a prime number using a while loop.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare integer variables:
  
  n to store the number entered by the user.
  
  i to use as a counter (initialize to 2).
  
  f as a flag to indicate whether the number is divisible (initialize to 0).
### Step 4: 
  Read the value of n from the user.
### Step 5: 
  Use a while loop to iterate while i <= n-1:
  
  Check if n % i == 0:

  If yes, set f = 1 (number is not prime) and break the loop.
  
  Increment i by 1.
### Step 6: 
  After the loop:
  
  If f == 0, print that the number is prime.
  
  Else, print that the number is not prime.
### Step 7:   
  Stop
# Program:
```
#include <stdio.h>
int main() {
    int num, i = 2, is_prime = 1;
    scanf("%d", &num);
    if (num <= 1) {
        is_prime = 0;
    } else {
        while (i <= num / 2) {
            if (num % i == 0) {
                is_prime = 0;
                break;
            }
            i++;
        }
    }
    if (is_prime == 1) {
        printf("%d is a Prime number.\n", num);
    } else {
        printf("%d is not a Prime number.\n", num);
    }
}
```
# Output:
<img width="218" height="56" alt="image" src="https://github.com/user-attachments/assets/97b1e2c3-c7eb-4175-bee9-f648f54e6c77" />
<img width="240" height="46" alt="image" src="https://github.com/user-attachments/assets/82e7f012-dde5-440f-a4ae-d88e83815413" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
# Ex.No:9
  Generate the C code to display the pattern below.  
 ``` 
 12345  
 2   4  
 3   3  
 4   2  
 54321
 ```
# Date : 18-05-2026.
# Aim:
 To build a C program that prints the required numeric pattern for a given value of n using nested loops.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare variables i, j, n, and k.
### Step 4: 
  Read the value of n from the user.
### Step 5: 
  Set i = 1.
### Step 6:  
  Repeat the following steps until i > n:
  
  Step 6.1: For j from i to n, print j if i == 1 or j == i, otherwise print a space.
  
  Step 6.2: Set k = j - 2.
  
  Step 6.3: For j from 1 to i - 1, print k if i == n or j == i - 1, otherwise print a space.
  
  Step 6.4: Decrease k after each print.
  
  Step 6.5: Move to the next line.
  
### Step 7: 
  Increase i and repeat Step 6.
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
int main() {
    int n = 5;
    for (int i = 1; i <= n; i++) {
        for (int j = 1; j <= n; j++) {
            if (i == 1) {
                printf("%d", j);
            } else if (i == n) {
                printf("%d", n - j + 1);
            } else if (j == 1) {
                printf("%d", i);
            } else if (j == n) {
                printf("%d", n - i + 1);
            } else {
                printf(" ");
            }
        }
        printf("\n");
    }
}
```
# Output:
<img width="76" height="113" alt="image" src="https://github.com/user-attachments/assets/5e10f814-983d-4a2d-aaab-e917dfabe8a1" />

# Result: 
  Thus, the program was implemented and executed successfully, and the required output was obtained.

  
# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
### Date: 18-05-2026.
# Ex.No:10
  Generate the C code to display the pattern below.  
  
 0
 
 7  0  7
 
 6  7  0  7  6
 
 5  6  7  0  7  6  5
 
 4  5  6  7  0  7  6  5  4
 
 3  4  5  6  7  0  7  6  5  4  3
 
 2  3  4  5  6  7  0  7  6  5  4  3  2
 
 1  2  3  4  5  6  7  0  7  6  5  4  3  2  1

# Aim: 
  To formulate a C program to print a symmetric numeric pattern in which each row contains an increasing sequence of numbers from the row value up to 7, followed by 0 in the center, and then a decreasing sequence of numbers back to the row value.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare integer variables i and j.
### Step 4: 
  Print 0 on the first line.
### Step 5:
  Set i = 7.
### Step 6:
   Repeat Steps 6.1 to 6.4 while `i >= 1`:

   Step 6.1: For `j = i` to `7`, print `j`.

   Step 6.2: Print `0` in the center.

   Step 6.3: For `j = 7` down to `i`, print `j`.

   Step 6.4: Move to the next line.
### Step 7:
  Decrease i by 1 and go back to Step 6.
### Step 8:
  Stop
### Program:
```
#include <stdio.h>
int main() {
    int start_num = 7;
    for (int i = 8; i >= 1; i--) {
        for (int j = i; j <= start_num; j++) {
            printf("%d ", j);
        }
        printf("0");
        for (int j = start_num; j >= i; j--) {
            printf(" %d", j);
        }
        printf("\n");
    }
}
```
### Output:
<img width="272" height="175" alt="image" src="https://github.com/user-attachments/assets/787dd400-dae4-4fec-b0fd-40f0aac6ef64" />

# Result:
  Thus, the program was implemented and executed successfully, and the required output was obtained.

