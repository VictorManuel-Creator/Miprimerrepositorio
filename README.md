int n, suma = 0, cont = 0;
int c1 = 0, c2 = 0, c3 = 0, c4 = 0;

do
{
    n = int.Parse(Console.ReadLine());
    if (n > 0)
    {
        suma += n;
        cont++;
        if (n < 10) c1++;
        else if (n < 100) c2++;
        else if (n < 1000) c3++;
        else if (n < 10000) c4++;
    }
} while (n != 0);

if (cont > 0)
{
    Console.WriteLine($"Promedio: {(double)suma / cont}");
    Console.WriteLine($"1 cifra: {c1}");
    Console.WriteLine($"2 cifras: {c2}");
    Console.WriteLine($"3 cifras: {c3}");
    Console.WriteLine($"4 cifras: {c4}");
}
