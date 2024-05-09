# 19AI308-Object-Oriented-Programming-using-CSharp-Exp-9---Interface-with-abstract-methods

## AIM:
To develop a small bank application by declaring deposit() and withdrawal() as an abstract methods in the interface. 

## ALGORITHM:
### STEP 1. 
Interface Bank: defines deposit and withdraw methods.
### STEP 2. 
Program class: implements Bank, manages deposit and withdrawal operations.
### STEP 3. 
Constructor: prompts user for deposit or withdrawal choice.
### STEP 4. 
deposit method: adds entered amount to balance, displays updated balance.
### STEP 5. 
withdraw method: subtracts entered amount from balance, displays updated balance.
### STEP 6. 
Main method: creates Program object, initiates banking operations based on user input.

## PROGRAM:
Developed by:Yogabharathi S 
Register number:212222230179
```
using System;
using System.Transactions;
public interface Bank
{
    void deposit();
    void withdraw();
}
public class Program:Bank
{
    public int amount,balance=5000;
    public Program()
    {
        Console.WriteLine("Enter your Choice:\n1.Deposit\n2.WithDraw");
        int opt;
        opt = Convert.ToInt32(Console.ReadLine());
        if (opt == 1)
            deposit();
        else if (opt == 2)
            withdraw();
        else
        {
            Console.WriteLine("Enter a valid input");
        }
    }
    public void deposit()
    {
        Console.WriteLine("Enter the amount to deposit");
        amount = Convert.ToInt32(Console.ReadLine());
        balance += amount;
        Console.WriteLine("The Balance is " + balance);
    }
    public void withdraw()
    {
        Console.WriteLine("Enter the amount to withdraw");
        amount = Convert.ToInt32(Console.ReadLine());
        balance -= amount;
        Console.WriteLine("The Balance is " + balance);
    }
}
public class Exp9
{
    public static void Main(string[] args)
    {
        Program n = new Program();
    }
}
```

## OUTPUT:
![image](https://github.com/Yogabharathi3/19AI308-Object-Oriented-Programming-using-CSharp-Exp-9---Interface-with-abstract-methods/assets/118899387/e57da53f-8ca4-4870-8470-a38a1f6a5ab3)

## RESULT:
Thus, a C# program has created for developing a small bank application by declaring deposit() and withdraw() as an abstract methods in the interface and it is executed and verified successfully.
