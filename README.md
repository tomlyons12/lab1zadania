# lab1zadania
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Program do obliczania pola koła");
        
        Console.Write("Podaj promień koła: ");
        string input = Console.ReadLine();

        if (double.TryParse(input, out double radius) && radius >= 0)
        {
            double area = Math.PI * radius * radius;
            Console.WriteLine($"Pole koła o promieniu {radius} wynosi {area:F2}");
        }
        else
        {
            Console.WriteLine("Niepoprawne dane. Promień musi być liczbą nieujemną.");
        }
    }
}
