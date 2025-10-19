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
void monthemi(float p,float aunnalrate,float years)
{
    float r = aunnalrate / (12 *100);
    float n = 12*  years ;
    float EMI = (p*r*pow(1+r,n)) / (pow(1+r,n) - 1);
    printf("Monthly EMI is= %.3f",EMI);
}
int main()
{
    
    float principle,rate,time;
    scanf("%f %f %f",&principle,&rate,&time);
    monthemi(principle,rate,time);
    return 0;
    
}
````
## OUTPUT

![WhatsApp Image 2025-10-19 at 17 45 53_710c6edd](https://github.com/user-attachments/assets/5bff8b3e-cc3c-4654-85bb-97964e969c78)


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
int main()
{
    int n,a=0,b=1,c;
    scanf("%d",&n);
    printf("%d %d ",a,b);
    for(int i=3; i<=n; i++)
    {
        c = a+b;
        printf("%d ",c);
        
        a=b;
        b=c;
    }
    return 0;
}
## OUTPUT

![WhatsApp Image 2025-10-19 at 17 47 29_56812e5f](https://github.com/user-attachments/assets/cbc9e09f-f88d-4efc-a474-fbc0be319943)


## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 
```

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

int main()
{
    int n;
    scanf("%d",&n);
    int a[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
}
   printf("%d ",a[n]);
    return 0;

          

}
```

## OUTPUT

```
input
5
10 20 30 40
output
40
```

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
int main()
{
    int n, i, count =0;
    scanf("%d", &n);
    int a[n];
    for(i=0; i<n; i++)
    {
        scanf("%d", &a[i]);
    }
    
    for(i=0; i<n; i++)
    {
      {if(a[i]>0)
       count++;}
    }
       printf("count  of positive numbers  in array: %d", count);
      return 0;
}
```

## OUTPUT
![WhatsApp Image 2025-10-19 at 17 57 30_38703dbf](https://github.com/user-attachments/assets/38d21113-0e66-45cd-a50b-2c760e7ff8fb)


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
    scanf("%d",&n);
    int arr[n];
    for(int i=0;i<n;i++)
    { 
        scanf("%d",&arr[i]);
        
    }
    
    for(int i=0;i<n;i++)
    { 
        
        if(arr[i]%2==0) arr[i]=arr[i];
        else arr[i]='E;
    }
    for(int i=0;i<n;i++)
        printf("%d ",arr[i]);
    
    
    return 0;
}
```

## Output:
```
 Input		
10
5 6 4 12 19
output
5 E E E 19
```

## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



