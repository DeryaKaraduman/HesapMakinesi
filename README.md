# HesapMakinesi
using System;

namespace HesapMakinesi
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.Write("lütfen ilk sayıyı giriniz: ");
            double sayi1 = Convert.ToDouble(Console.ReadLine());

            Console.Write("lütfen ikinci sayıyı giriniz: ");
            double sayi2 = Convert.ToDouble(Console.ReadLine());

            Console.Write("lütfen yapmak istediğiniz işlemi tuşlayınız;  \ntoplama(+)\nçıkartma(-)\nçarpma(*)\nbölme(/) ");
            Console.WriteLine();
            string islem = Console.ReadLine();
            switch (islem)
            {
                case "+":
                        Console.WriteLine(sayi1 + sayi2);
                    break;
                case"-":
                    Console.WriteLine(sayi1 - sayi2);
                    break;
                case "*":
                    Console.WriteLine(sayi1 * sayi2);
                    break;
                case "/":
                    Console.WriteLine(sayi1 / sayi2);
                    break;
                default:
                    Console.WriteLine("hatalı işlem girdiniz.");
                    break;
                   
            }
            
            Console.Read();
        }
    }
}
