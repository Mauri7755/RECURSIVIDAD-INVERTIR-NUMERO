# RECURSIVIDAD-INVERTIR-NUMERO
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication68
{
     class Program
    {
        
         public void invertir(int n)
         {
             Console.Write(n % 10);
             
             if (n > 10)
                 invertir(n / 10);
         }
        static void Main(string[] args)
        {
            Program p=new Program();
            int n2=0;
            Console.WriteLine("Ingrese el numero que desea invertir: ");
             n2 = int.Parse(Console.ReadLine());
            Console.WriteLine("");
            Console.WriteLine("El numero invertido de " + n2 + " es:");
            p.invertir(n2);
            Console.ReadKey();
        }
    }
}
