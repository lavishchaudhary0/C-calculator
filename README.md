using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Practice
{
    internal class Program
    {
            static void Main(string[] args)
            {
                string value;
                do
                {
                    int res;
                    Console.Write("Enter first number:");
                    int num1 = Convert.ToInt32(Console.ReadLine());
                    Console.Write("Enter second number:");
                    int num2 = Convert.ToInt32(Console.ReadLine());
                    Console.Write("Enter symbol(/,+,-,*):");
                    string symbol = Console.ReadLine();

                    switch (symbol)
                    {
                        case "+":
                            res = num1 + num2;
                            Console.WriteLine("Addition:" + res);
                            break;
                        case "-":
                            res = num1 - num2;
                            Console.WriteLine("Subtraction:" + res);
                            break;
                        case "*":
                            res = num1 * num2;
                            Console.WriteLine("Multiplication:" + res);
                            break;
                        case "/":
                            res = num1 / num2;
                            Console.WriteLine("Division:" + res);
                            break;
                        default:
                            Console.WriteLine("Wrong input");
                            break;
                    }
                   
                    Console.Write("Do you want to continue(y/n):");
                    value = Console.ReadLine();
                }
                while (value == "y" || value == "Y");
            }
       
    }
}# C-calculator
C# calculator
