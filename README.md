class program
{
static void Main()
{
Console.Write("enter a number");
int number = Convert.ToInt32(Console.ReadLine());
Console.WriteLine("جمله {number} دنباله فیبوناچی: {Fib(number)}");
}

static int Fib(int n)
{
int a = 0;
int b = 1;
for (int i = 2; i <= n; i++)
{
int temp = a;
a = b;
b = temp + b;
}
return n > 0 ? b : a;
}
}
