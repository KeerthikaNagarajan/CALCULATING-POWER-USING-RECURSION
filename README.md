## Ex-6
## CALCULATING POWER USING RECURSION
### Aim:
To Write a Java program to calculate the power of a number raised to other using recursion where the numbers a and b are to be entered by the user.

### Procedure:
* Create the class and declare the main method so that the JVM will identify the main program to run.
* The user is prompted to enter the base number (a) and the power (b) using the Scanner class.
* The power method is called with the base number (x) and the power (y).
* In the power method, if the power (y) is not zero, it recursively calls itself with the same base number (x) and decremented power (y-1), and multiplies the base number with the result.
* The recursion continues until the power reaches zero, at which point the method returns 1.
* The result of the power operation is stored in the res variable, and finally the result is displayed to the user.

### Code:
```
import java.util.Scanner;
public class Ex6
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter the base number: ");
        int a = sc.nextInt();
        System.out.print("Enter the power: ");
        int b = sc.nextInt();
        int res = power(a,b);
        System.out.println(a+"^"+b+" = "+res);
    }
    public static int power(int x, int y)
    {
        if(y != 0)
            return (x * power(x,y-1));
        else
            return 1;
    }
}
```

### Output:
<img width="170" alt="6" src="https://github.com/KeerthikaNagarajan/Java-Ex-6/assets/93427089/baee48f5-462c-4396-9803-9bf164eeac60">

### Result:
Thus, a java program is created to calculate the power of a number raised to other using recursion.
