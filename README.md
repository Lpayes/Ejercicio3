```csharp
int suma(int num1, int num2)
{
    int resuls = 0;
    resuls = num1 + num2;
    return resuls;

int division(int num1, int num2)
{
    int resuld = 0;
    resuld = num1 / num2;
    return resuld;
}
int resta(int num1, int num2)
{
    int resulr = 0;
    resulr = num1 - num2;
    return resulr;
}
int multiplicacion(int num1, int num2)
{
    int resulm = 0;
    resulm = num1 * num2;
    return resulm;
}


Console.WriteLine("ingresa el numero de la operacion que desea realizar:");
Console.WriteLine("1: Suma");
Console.WriteLine("2: Resta");
Console.WriteLine("3: Division");
Console.WriteLine("4: Multiplicacion");
int select = Convert.ToInt32(Console.ReadLine());

Console.WriteLine("Ingrese el primer digito");
int param1 = Convert.ToInt32(Console.ReadLine());
Console.WriteLine("Ingrese el segundo digito");
int param2 = Convert.ToInt32(Console.ReadLine());

switch (select)
{
    case 1:
        Console.WriteLine($"la suma es: {suma(param1, param2)}");
        break;
    case 2:
        Console.WriteLine($"La multiplicacion es; {resta(param1, param2)}");
        break;
    case 3:
        Console.WriteLine($"La multiplicacion es; {division(param1, param2)}");
        break;
    case 4:
        Console.WriteLine($"La multiplicacion es; {multiplicacion(param1, param2)}");
        break;

    default: Console.WriteLine("Numero invalido"); break;
}
