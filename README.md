import java.util.Scanner;

class Add{
	static int arr[] = new int[100];
	
	static float sum=0;
	static int flag=0;
	static Scanner input = new Scanner(System.in);
	public static void addarr()
	{
		System.out.println("Enter size of array:");
		int n = input.nextInt();
		int arr2[]=new int[arr.length];
		System.out.println("Enter "+ n +" elements of array");
		for(int i=0;i<n;i++)
		{
			arr[i] = input.nextInt();
		}
		for(int i=0;i<n;i++)
		{
			arr2[i]=arr[n-1-i];
		}
		System.out.println("reversed array is:");
		for(int i=0;i<n;i++)
		{
			System.out.println(arr2[i]);
		}
		
	}
}

public class Jala {

	public static void main(String[] args) {
		Add a = new Add();
		a.addarr();
	}
}
