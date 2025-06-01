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
    
    #include <stdio.h>
    #include <math.h>
    void emi(float p, float r, float t) {
        r = r/1200;
        t = t*12;
        float e = (p*r*pow(1+r,t))/(pow(1+r,t)-1);
        printf("%.2f", e);
    }
    int main() {
        float principal, rate, time;
        scanf("%f%f%f", &principal, &rate, &time);
        emi(principal, rate, time);
        return 0;
    }
## OUTPUT

![image](https://github.com/user-attachments/assets/157b633e-bc69-45fb-91ff-4108254807f2)




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
    #include <stdio.h>
    int main() {
        int n = 6, a = 0, b = 1, c;
        for(int i=0; i<n; i++) {
            printf("%d ", a);
            c = a + b;
            a = b;
            b = c;
        }
        return 0;
    }
## OUTPUT
 ![image](https://github.com/user-attachments/assets/5e2ba3f4-87b6-44e7-a13f-13cb26a1ead5)








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
    #include <stdio.h>
    int main() {
        int n;
        scanf("%d", &n);
        int arr[n];
        for(int i=0; i<n; i++) scanf("%d", &arr[i]);
        printf("%d", arr[n-1]);
        return 0;
    }
## OUTPUT

![image](https://github.com/user-attachments/assets/0a139cad-35a3-4358-96d9-3d4c370c9cd2)








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
#include <stdio.h>
int main() {
    int n, count=0;
    scanf("%d", &n);
    int arr[n];
    for(int i=0; i<n; i++) {
        scanf("%d", &arr[i]);
        if(arr[i] > 0) count++;
    }
    printf("%d", count);
    return 0;
}

## OUTPUT
![image](https://github.com/user-attachments/assets/b7faad4e-e1b8-443e-a597-e8d309c2aa6e)





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
    #include <stdio.h>
    int main() {
        int n;
        scanf("%d", &n);
        int arr[n];
        for(int i=0; i<n; i++) {
            scanf("%d", &arr[i]);
            if(arr[i]%2 == 0) arr[i] = 'E';
            else{
            arr[i]==arr[i];
            }
            printf("%c ", arr[i]);
        }
        return 0;
       }
## Output:
![Uploading image.png…]()



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



