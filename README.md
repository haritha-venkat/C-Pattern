## Aim:
To write a C# Program for Pascal Triangle.

## Equipment Required:
Hardware - PC Software - Microsoft Studio Code (C#)

## Algorithm:
## Step 1:
Import the 'System' namespace to use the classes present in the 'System' namespace.

## Step 2:
Declare the Main method.

Step 3:
Declare variable n,i,j,space.

Step 4:
Using " Console.Write " print the statement and get the input from user using " Console.ReadLine " .

Step 5:
Using for loop print the required pattern.

Step 6: Print the result.

## Program:
using System;
using System.Globalization;

namespace Pattern
{
    class Program
    {
        static void Main(string[] args)
        {
            int n,i,j,c=1,space;
            Console.Write("Enter the No of Rows : ");
            n=Convert.ToInt32(Console.ReadLine());
            for(i = 0; i < n; i++)
            {
                for(space=1;space<=n-i;space++)
                {
                    Console.Write(" ");
                }
               for( j=0 ; j<=i ; j++)
               {
                    if(i==0 || j==0)
                    {
                        c = 1;
                    }
                    else
                    {
                        c = c*(i - j + 1) / j;
                    }
                    Console.Write("{0} ",c);
                }
                Console.WriteLine();
            }
        }
    }
}
## Output:
![image](https://github.com/haritha-venkat/C-Pattern/assets/121285701/9ad13be6-fd2f-4b88-a84e-0fa4d4feca81)

![Screenshot (83)](https://github.com/haritha-venkat/C-Pattern/assets/121285701/ce39f3b6-5f66-43e6-aef4-e8ba9ee5e274)

## result:
Thus,the C# program to print pascals triangle is executed sucessfully.
