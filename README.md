using System;
//ROBLES-BSCS302
public class ComputeAverageProgram
{
    public static void Main(string[] args)
    {
        double sum = 0;
        Console.WriteLine("PLEASE ENTER THE 5 GRADES SEPARATED BY NEW LINE:");

        for (int i = 0; i < 5; i++)
        {
            Console.Write($"GRADE NUMBER {i + 1}: ");
            sum += Convert.ToDouble(Console.ReadLine());
        }

        double average = sum / 5;
        int rounded = (int)Math.Round(average);

        Console.WriteLine($"\nTHE AVERAGE IS {average} AND ROUND OFF TO {rounded}");
        Console.Write("\nPRESS ANY KEY TO EXIT...");
        Console.ReadKey();
    }
}
