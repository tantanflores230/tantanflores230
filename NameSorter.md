using System;

namespace NameSorter
{
    class Program
    {
        static void Main(string[] args)
        {
            string[] names = new string[5];

            Console.WriteLine("Enter 5 names:");

            for (int i = 0; i < 5; i++)
            {
                Console.Write("Input: ");
                names[i] = Console.ReadLine();
            }

            Array.Sort(names);

            Console.WriteLine("\nAlphabetical order:");
            foreach (string name in names)
            {
                Console.WriteLine(name);
            }
        }
    }
}
