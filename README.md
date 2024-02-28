import java.util.Random;
import java.util.Scanner;

public class Praveen {

	public Praveen() {
		//no argument constructor....
	}

	public static void main(String[] args) {
		 int answer,guess;
   	  final int MAX=100;
   	  Scanner sc=new Scanner(System.in);
   	  Random rand=new Random();
   	  answer=rand.nextInt(MAX)+1; 
   	  System.out.println("guess the number between 1 and 100:");
   	  guess=0; 
   	  int score=10;
   	while(guess!=answer && score>0) {
   		guess=sc.nextInt();
   	  if(guess==answer) {
 		System.out.println("The number was " +answer);  
       	System.out.println("GOOD JOB!!!");
   		System.out.println("Your Score is " +score);
   		
   		  
   	  }
   	  if(guess>answer) {
   		System.out.println("The Number was HIGH!! ");
   		score--;
   		System.out.println("************************");
   	  }
   	if(guess<answer) {
   		System.out.println("The Number was LOW!! ");
   		score--;
    	System.out.println("************************");
   	  }
   	  }
   	  if(score==0)
   	  System.out.println("Sorry Better Luck Next Time.... ");
	}
	}


