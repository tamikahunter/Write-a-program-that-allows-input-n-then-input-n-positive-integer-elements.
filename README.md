# Write-a-program-that-allows-input-n-then-input-n-positive-integer-elements.
Write a program that allows input n, then input n positive integer elements.
import java.util.Scanner;
public class BaiTapJavaCoBan12
{
    public static void main(String[] args)
    {
       int n;
       int[] soNguyen;
       int max = 0;
       Scanner sc = new Scanner(System.in);

       System.out.println("Enter n:");
       n = sc.nextInt();
       soNguyen = new int[n];
       for (int i = 0; i < n; i++)
       {
          System.out.println("Integer:");
          soNguyen[i] = sc.nextInt();
       }

       for (int i = 0; i < n; i++)
       {
          if(soNguyen[i] > max)
          max = soNguyen[i];
       }
      
       System.out.println("Maximum element is: " + max);
    }
}
