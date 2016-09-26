# 09-26-16
	/* Programmer:Collin Palmer
	* Date:09/26/16
	* COSC 111 mw 2:00
 	* khaled mansour
 	* purpose: if else if statement
	*/
import java.util.Scanner;
	public class work 
{
	

	public static void main(String[] args) 
	{
		
		Scanner k= new Scanner(System.in);
		int points=0,angl=0,angl2=0,angl3=0;
		char grade = ' ';
		String tritype="";
		
		//input
		System.out.println("Enter points:");
		points= k.nextInt();
		System.out.println("Enter three angles");
		angl=k.nextInt();
		angl2=k.nextInt();
		angl3=k.nextInt();
		
		if(angl==angl2 && angl2==angl3)
			tritype="equilateral";
			else if (angl==90||angl2==90||angl3==90)
			tritype="Right";
		else
			tritype="isoceles";
		if (points>=90 && points <=100)
		     grade='A';
		  
		else if (points>=80 && points<=89)
			grade='B';
		else if (points>=70 && points<=79)
		    grade='C';
		else if (points>= 60 && points<=69)
			grade='D';
		else if (points >=0 && points <=59)
			grade='F';
		else 
			grade='?';
		
      System.out.println("your grade is "+grade);
      System.out.println("your triangle type is "+tritype);
	}
  
}
