----------
## **Experiment No : 01**

## **Experiment Name : Use three separate function to
a) take input from a 1d array,
b) sum the elements and
c) show the sum and elements
**

## **Submission Date : 22 November 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```C
#include <stdio.h>

void in(int ar[], int n)//this order is important. Don't know why but sometimes code doesn't work if you don't put them in this order
{
    for(int i=0; i<n; i++)
    {
      scanf("%d",&ar[i]);
    }
}
void out(int ar[], int n)
{
    for(int i=0; i<n; i++)
    {
      printf("%d\t",ar[i]);
    }
}
int su(int ar[], int n, int sum)
{
    for(int i=0; i<n; i++)
    {
      sum+= ar[i];
    }
    printf("\nSum of all the elements: %d",sum);
    return sum;
}
int main()
{
    int n,sum=0;
    printf("Number of input? ");
    scanf("%d",&n);
    int ar[n];
    in(ar,n);
    out(ar,n);
    su(ar,n,sum);
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/JQymzxM/image.png" alt="image" border="0"></a>
</p>

-----------------------------------------

----------
## **Experiment No : 02**

## **Experiment Name :
For 2d Array:
 Use three separate function to
a) take input from a 2d array,
b) sum the elements and
c) show the sum and elements
**

## **Submission Date : 22 November 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```C
#include <stdio.h>
void in( int n, int a, int ar[n][a])//for 2d array: first put int variables then the arrays in this format
{
    for(int i=0; i<n; i++)
    {
        for(int j=0; j<a; j++)
        {
         scanf("%d",&ar[i][j]);
        }
    }
}
void out(int n, int a, int ar[n][a])
{
    printf("Output: \n");
    for(int i=0; i<n; i++)
    {
        for(int j=0; j<a; j++)
        {
         printf("%d ",ar[i][j]);
        }
        printf("\n");
    }
    printf("\n");
}
int sum(int n, int m, int arr[n][m])
{
    int total = 0;
    for (int i = 0; i < n; i++)
    {
        for (int j = 0; j < m; j++)
        {
            total += arr[i][j];
        }
    }
    return total;
}
int main()
{
    int n,a;
    printf("Number of rows? ");
    scanf("%d",&n);
    printf("Number of columns? ");
    scanf("%d",&a);
    int ar[n][a];
    in(n,a,ar);
    out(n,a,ar);
    printf("sum : %d\n", sum(n, a, ar));
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/VMF60BN/image.png" alt="image" border="0"></a>
</p>


