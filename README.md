## AIM:
To write a C program that prints the following number pattern using nested loops:

12345

4321

123

21

1

## ALGORITHM:
1. Start
2. Declare integer variables i and j for loop control.
3. Use a for loop to print each line of the pattern based on the line number.
4. For odd-numbered lines (1, 3, 5, ...), print numbers in increasing order.
5. For even-numbered lines (2, 4, ...), print numbers in decreasing order.
6. Use nested loops — outer loop for rows, inner loop for printing numbers.
7. Stop

## PROGRAM:
```
#include <stdio.h>

int main()
{
    int N=5,row,col;
    
    printf("The pattern is: \n");
    for(row=1;row<=N;row++)
    {
        int temp = 1;
        int temp1 = N;
        int temp2 = 2;
        for(col=N;col>=row;col--)
        {
            if(row%2==1)
            {
                printf("%d",temp);
                temp++;
            }
            else if(row==2)
            {
                temp1--;
                printf("%d",temp1);
            }
            else
            {
                printf("%d",temp2);
                temp2--;
            }
        }
        printf("\n");
    }
}
```

## OUTPUT:

<img width="682" height="247" alt="image" src="https://github.com/user-attachments/assets/edfe469a-3a98-4af6-9f12-04b9f49b2361" />

## RESULT:

The program successfully prints the required number pattern using nested loops and conditional statements.
