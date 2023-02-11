// Напишите программу, которая принимает на вход число и выдаёт сумму цифр в числе.
//452 -> 11
//82 -> 10
//9012 -> 12

void SumNum(int[] a, int n)

{

    int sum = 0;
    
    for (int i =0; i<n; i++)
    
    {
      sum = sum + a[i];
    }
    
    Console.WriteLine(sum);   
    
}

Console.WriteLine("Введите количество цифр в числе: ");

int n = Convert.ToInt32(Console.ReadLine());

Console.WriteLine("Введите цифры по одной: ");

int[] a = new int[n];

for (int i=0; i<n; i++)

{
    a[i] = Convert.ToInt32(Console.ReadLine());
}

SumNum(a,n);
