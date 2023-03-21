# Pattern

## Aim:
To write a C# program for a pascal's triangle.
## Equipment Required:
Visual studio 
## Algorithm:
### Step 1:
Start.
### Step 2:
Create a class and declare two variables rows,Val using integer datatype.
### Step 3:
Using nested for loop create a pascal's triangle.
### Step 4:
Stop.
## Program:
```
using System;
using System.Data;

namespace condition
{
    public class pascal
    {
        public static void Main(string[] args)
        {
            int rows=5,Val=1;
            for(int i=0;i<rows;i++)
            {
                for (int blank = 1; blank < rows - i; blank++)
                {
                    Console.Write(" ");
                }
                    for(int j=0;j<=i;j++)
                    {
                    if (i == 0 || j == 0)
                    {
                        Val = 1;
                    }
                    else
                    {
                        Val = Val * (i - j + 1) / j;
                    }
                            Console.Write(Val +" ");
                        
                       
                    }
                Console.WriteLine();
            }
            }
        }
    }

```

## Output:
![1](https://user-images.githubusercontent.com/75235212/189470131-664bca16-2e99-4aa7-b604-caf351ea595a.png)


## Result:
Thus the C# program to print the pascal's triangle is executed successfully.
