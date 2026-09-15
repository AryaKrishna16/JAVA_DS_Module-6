# EX3 Write a program to count the number of digits in an integer.
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
Read the input number Take an integer num from the user.
Convert the number to a non-negative value Use Math.abs(num) and store it in n to handle negative numbers.
Check if the number is zero If n == 0, set digit count to 1 (since zero has one digit).
Count digits for non-zero numbers Repeatedly divide n by 10 and increment the counter until n becomes 0.
Display the digit count Output the total number of digits. 

## Program:
```
/*
Program to to count the number of digits in an integer
Developed by: E ARYA KRISHNA
RegisterNumber: 212225240014
*/
import java.util.Scanner;

public class CountDigits {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();

        int count = 0;
        int n = Math.abs(num); 

        if (n == 0) {
            count = 1; 
        } else {
            while (n > 0) {
                n /= 10; 
                count++;
            }
        }

        System.out.println("Number of digits: " + count);
    }
}
```

## Output:
<img width="822" height="353" alt="image" src="https://github.com/user-attachments/assets/5c57072a-84ad-4fd6-81b4-c72db1c55cf4" />




## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
