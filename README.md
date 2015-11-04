# markdown / addition game 

## Introduction 
Designing a math quiz that increases the difficulty as the user answers a question.

## Code
```
 import java.util.Random;
import java.util.Scanner;




public class Jimmy {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		System.out.println(" ---Welcome to Jameel's Math Challenge!--- ");
		System.out.println("You will be asked 5 question, Be ready user! ");
		Scanner in = new Scanner(System.in);
		Random rand = new Random();
		
		
					//Declaring variables
		 int QuesHard=10;
		 int points=0;
		 int num1=(int) (Math.random()* points);
		 int num2=(int) (Math.random()* points);
		 int  answer, checking;
		 
		 
		 
					//Code for the first round
		 num1 = rand.nextInt(10);
		num2 = rand.nextInt(10);
		answer = num1+num2;
		System.out.print(num1 +  " + " + num2 +" = " );
		
		
		
		
					//For checking the answer Round 1
			checking =in.nextInt();
			if (checking == answer){
				System.out.println("Awesome! You are brilliant");
				points+= QuesHard;
				System.out.println("Your points: " + points );
				System.out.println("The Hard Question Rate: " + QuesHard );
} 
				else
					System.out.println("Uh oh! Try again! ");
					System.out.println("Answer was: " + answer  );
					points+=0;
					if(QuesHard>10){
						QuesHard/=10;
					}
					
	System.out.println("End of Round 1 ");
	
	
	
	
	
 //Declaring
	int QuesHard1=10;
	int points1=0;
	 int num11=(int) (Math.random()* points1);
	 int num21=(int) (Math.random()* points1);
	 int  answer1, checking1;
	 
	 
	 
				//Code for the first second
	 num11 = rand.nextInt(10);
	num21 = rand.nextInt(10);
	answer1 = num11+num21;
	System.out.print(num11 +  " + " + num21 +" = " );
	
	
	
				//For checking the answer Round 2
		checking1 =in.nextInt();
		if (checking1 == answer1){
			System.out.println("Awesome! You are brilliant");
			points1+= QuesHard1*10;
			System.out.println("Your points: " + points1 );
			System.out.println("The Hard Question Rate: " + QuesHard );

} 

		else 
				System.out.println("Uh oh! Try again! ");
				System.out.println("Answer was: " + answer1  );
				points1+=0;
				if(QuesHard1>10){
					QuesHard1/=10;
				}
				System.out.println("End of Round 2 ");
				
				
				
				
				 //Declaring
				int QuesHard11=10;
				int points11=0;
				 int num111=(int) (Math.random()* points11);
				 int num211=(int) (Math.random()* points11);
				 int  answer11, checking11;
				 
				 
				 
							//Code for the first third
				 num111 = rand.nextInt(10);
				num211 = rand.nextInt(10);
				answer11 = num111+num211;
				System.out.print(num111 +  " + " + num211 +" = " );
				
				
				
							//For checking the answer Round 3
					checking11 =in.nextInt();
					if (checking11 == answer11){
						System.out.println("Awesome! You are brilliant");
						points11+= QuesHard11*100;
						System.out.println("Your points: " + points11 );
						System.out.println("The Hard Question Rate: " + QuesHard );

			} 

					else 
							System.out.println("Uh oh! Try again! ");
							System.out.println("Answer was: " + answer11  );
							points11+=0;
							if(QuesHard11>10){
								QuesHard11/=10;
							}
							System.out.println("End of Round 3 ");	
							
							
							
			 //Declaring
	    	int QuesHard111=10;
		    int points111=0;
		    int num1111=(int) (Math.random()* points111);
		    int num2111=(int) (Math.random()* points111);
		    int  answer111, checking111;
		    
		    
		    
							 
										//Code for the first fourth
							 num1111 = rand.nextInt(10);
							num2111 = rand.nextInt(10);
							answer111 = num1111+num2111;
							System.out.print(num1111 +  " + " + num2111 +" = " );
							
							
							
										//For checking the answer Round 4
								checking111 =in.nextInt();
								if (checking111 == answer111){
									System.out.println("Awesome! You are brilliant");
									points111+= QuesHard111;
									System.out.println("Your points: " + points111 );
									System.out.println("The Hard Question Rate: " + QuesHard );

						} 

								else 
										System.out.println("Uh oh! Try again! ");
										System.out.println("Answer was: " + answer111  );
										points111+=0;
										if(QuesHard111>10){
											QuesHard111/=10;
										}
										System.out.println("End of Round 4 ");
										
}}
```
## Console Output
```
---Welcome to Jameel's Math Challenge!--- 
You will be asked 5 question, Be ready user! 
3 + 5 = 8
Awesome! You are brilliant
Your points: 10
The Hard Question Rate: 10
Answer was: 8
End of Round 1 
7 + 5 = 12
Awesome! You are brilliant
Your points: 100
The Hard Question Rate: 10
Answer was: 12
End of Round 2 
5 + 9 = 0
Uh oh! Try again! 
Answer was: 14
End of Round 3 
1 + 4 = 0
Uh oh! Try again! 
Answer was: 5
End of Round 4 
Your total points are: 10

```
## Summary
Here we are trying to write a code that sorts the rounds and harden the questionability as the user answers the question. Using the if and else statement was the correct choice. I learned that Math.random was specified for picking a random number. After figuring the inputs and everything I finally got it to work with the exception of hardening the questions.

## Git commands
Git add; this command accesses the user to add file or modify a file.
Git commit: storing content that was changed.
Git push: sharing command.
Git Pull: bringing up a repository.

