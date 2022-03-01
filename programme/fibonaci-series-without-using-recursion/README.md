## Write a program to print Fibonacci series without using recursion.

```
Input: 10
Output: 0 1 1 2 3 5 8 13 21 34
```

---

<CodeBlock slots="heading, code" repeat="1" languages="C" />

#### C

```c
#include <stdio.h>
int main()
{
    int a = 0, b = 1, temp = 0, n;
    printf("Input  : ");
    scanf("%d", &n);
    int i = 0;
    printf("Output : ");
    while (i != n)
    {
        printf("%d ", a);
        temp = a;
        a = b;
        b = temp + b;
        i++;
    }
    printf("\n");
    return 0;
}
```

## Write a program to print Fibonacci series without using recursion.

```
Input: 10
Output: 0 1 1 2 3 5 8 13 21 34
```

---

<CodeBlock slots="heading, code" repeat="1" languages="python" />

#### Python

```Python
first_num = int(input("Enter the first number of the fibonacci series : "))
second_num = int(input("Enter the second number of the fibonacci series : "))
num_of_terms = int(input("Enter the number of terms : "))
print(first_num,second_num)
print("The numbers in fibonacci series are : ")
while(num_of_terms-2):
   third_num = first_num + second_num
   first_num=second_num
   second_num=third_num
   print(third_num)
   num_of_terms -= 1
```
