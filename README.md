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
```c
#include <stdio.h>
#include <math.h>
float emic(float, float, float);
int main()
{
    float p,r,t;
    scanf("%f %f %f",&p,&r,&t);
    printf("Monthly EMI is= %.3f",emic(p,r,t));
}
float emic(float p, float r, float t)
{
    float rate = r / (12*100);
    float time = t * 12;
    float emi;
    emi = (p * rate * pow(1+rate,time))/(pow(1+rate,time)-1);
    return emi;
}
```                 

## OUTPUT

![Screenshot_29-4-2025_81740_training saveetha in](https://github.com/user-attachments/assets/92489c34-6736-4bdb-9038-79f111d39bf1)

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
```c
#include <stdio.h>
int main() 
{
    int n1=0,n2=1,n3,terms,i;
    printf("Enter the number of terms:\n");
    scanf(" %d",&terms);
    printf("The %d terms of fibonacci series are:\n",terms);
    printf("%d %d ",n1,n2);
    for (i=2;i<terms;i++)
    {
        n3 = n1 + n2;
        n1 = n2;
        n2 = n3;
        printf("%d ",n1);
    }
}
```

## OUTPUT

![Screenshot_29-4-2025_82333_www programiz com](https://github.com/user-attachments/assets/5b927f60-a91f-498b-af9b-567908045a15)

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
```c
#include <stdio.h>
int main()
{
    int n,i;
    printf("Enter no. of values needed\n");
    scanf(" %d",&n);
    int arr[n];
    printf("Enter the elements of the array:\n");
    for (i=0;i<n;i++)
    {
        scanf(" %d",&arr[i]);
    }
    printf("The last element of the array is: %d",arr[n-1]);
}
```

## OUTPUT

![Screenshot_29-4-2025_83110_www programiz com](https://github.com/user-attachments/assets/f8940a46-3203-41ea-90f5-c7a07442c730)

## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value is greater than 0 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```c
#include <stdio.h>
int main()
{
    int n,i,count=0;
    printf("Enter no. of values needed\n");
    scanf(" %d",&n);
    int arr[n];
    printf("Enter the elements of the array:\n");
    for (i=0;i<n;i++)
    {
        scanf(" %d",&arr[i]);
    }
    for (i=0;i<n;i++)
    {
        if (arr[i] > 0)
            count += 1;
    }
    printf("The total number of positive numbers in the array is %d",count);
}
```


## OUTPUT

![Screenshot_29-4-2025_83851_www programiz com](https://github.com/user-attachments/assets/aa9ea0c0-1295-44ae-b2e0-f47dfe4c2cc1)

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
```c
#include <stdio.h>
int main()
{
    int n,i,count=0;
    printf("Enter no. of values needed\n");
    scanf(" %d",&n);
    int arr[n];
    printf("Enter the elements of the array:\n");
    for (i=0;i<n;i++)
    {
        scanf(" %d",&arr[i]);
    }
    for (i=0;i<n;i++)
    {
        if (arr[i] % 2 == 0)
            arr[i] = 'E';
    }
    printf("The updated array is:\n");
    for (i = 0; i < n; i++)
    {
        if (arr[i] == 'E') 
        {
            printf("%c ", arr[i]); 
        } 
        else 
        {
            printf("%d ", arr[i]);
        }
    }
}
```

## Output:
 
![Screenshot_29-4-2025_84848_www programiz com](https://github.com/user-attachments/assets/9ed84482-5e17-4eef-a1d5-923fdb184412)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



