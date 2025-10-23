# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h>
void EMI(double P, double R, int n) {
    double r = R / 1200; 
    double amt = (P * r * pow(1 + r, n)) / (pow(1 + r, n) - 1);
    printf("EMI = %.2f\n", amt);
}

int main() {
    double principal, rate;
    int months;

    printf("Enter principal, annual rate, and months: ");
    scanf("%lf %lf %d", &principal, &rate, &months);
    EMI(principal, rate, months); 
    return 0;
}

```

## OUTPUT
<img width="723" height="177" alt="{542FDDC5-3E4B-4C73-A90C-B614CD088101}" src="https://github.com/user-attachments/assets/d4fe4f27-b69c-41cf-b845-ab0a6732ea23" />





## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, i;
    int t1 = 0, t2 = 1, next; 
    printf("Enter number of terms: ");
    scanf("%d", &n);

    printf("Fibonacci Series: ");

    for(i = 1; i <= n; i++) {
        printf("%d ", t1);  
        next = t1 + t2;     
        t1 = t2;            
        t2 = next;
    }

    return 0;  
}

```
## OUTPUT

<img width="488" height="188" alt="{3D896EDA-F78C-43FD-BE5E-20FA853F1D1E}" src="https://github.com/user-attachments/assets/ad8ac0f2-38d1-4b97-a393-3afef1872de9" />







## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n;
    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];  
    printf("Enter %d elements: ", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);  
    }
    printf("Last element = %d\n", arr[n-1]);

    return 0;  
}

```
## OUTPUT

<img width="563" height="254" alt="{D75A6AD3-00B5-456F-9207-56962FD6CFF0}" src="https://github.com/user-attachments/assets/bd2778cd-4d34-4293-8db7-39c4be26e3e7" />








## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, count = 0;
    printf("Enter number of elements: ");
    scanf("%d", &n);
    int arr[n];  
    printf("Enter %d elements: ", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]); 
        if(arr[i] % 2 == 0) {
            count++;
        }
    }
    printf("Number of even elements = %d\n", count);

    return 0;  
}

```

## OUTPUT

<img width="479" height="208" alt="{A19E5BA7-90AD-46F5-9C72-A544F9AC2A72}" src="https://github.com/user-attachments/assets/635f8075-44d4-44ab-b62c-903e2961e4a4" />




## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include <stdio.h>

int main() {
    int n;
    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements: ", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    char updated[n]; 
    for(int i = 0; i < n; i++) {
        if(arr[i] % 2 == 0) {
            updated[i] = 'E';  
        } else {
            updated[i] = arr[i] + '0';  
        }
    }
    printf("Updated array: ");
    for(int i = 0; i < n; i++) {
        printf("%c ", updated[i]);
    }

    return 0;
}

```

## Output:
 
<img width="451" height="170" alt="{0BB23D0F-B020-4648-A290-FC8ECAFB51CA}" src="https://github.com/user-attachments/assets/62ed1db2-0c32-4663-b0e0-8f6ff807d218" />


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



