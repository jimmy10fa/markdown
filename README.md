# Project 1:WH10


## Source Code
```
package Jimmy;
import java.util.Scanner;

public class LoopsAndMethodsAdditonGame {
	public static void main(String[] args) {
		//System.out.println("Hello class.");
		
		//Call the addition game method.
		AdditonGameMethod();
	}
	public static void AdditonGameMethod() {
		//System.out.println("Inside the addition game method.");
		
		int hardness = 5;
		int hardnessStep = 2;
		int score = 0;
		
		// Set up my for loop to go through the number of rounds
		int numberOfRounds = 3;
		for(int roundNumber = 1; 
		roundNumber <= numberOfRounds;  
		roundNumber = roundNumber + 1){
			//System.out.println("Inside the for loop. Round: " + roundNumber);
			System.out.print("Round " + roundNumber + " of " + numberOfRounds + ". ");
			boolean isAnswerCorrect = getAndCheckStudentAnswer(hardness);
			if(isAnswerCorrect){
				System.out.print("Your score was " + score + " and is now ");
				score = score + hardness;
				System.out.print(score + ". ");
				
				if(roundNumber<numberOfRounds){
					System.out.print("Your hardness was " + hardness + " and is now ");
					hardness = hardness * hardnessStep;
					System.out.println(hardness + ".");
				}
			}else{
				System.out.print("Your score is " + score + ". ");
				if(roundNumber<numberOfRounds){
					System.out.print("Your hardness was " + hardness + " and is now ");
					if(hardness>5){
						hardness = hardness / hardnessStep;
					}
					System.out.println(hardness + ".");
					
				}
				
			}
		}
		System.out.print("\nThe game is complete. ");
		System.out.println("Your final score was " + score );
	}
	
	public static boolean getAndCheckStudentAnswer(int hardness) {
		//System.out.println("Inside get and check student answer method.");
		int number1 = (int)(Math.random()*hardness);
		int number2 = (int)(Math.random()*hardness);
		System.out.print("Add " + number1 + " and " + number2 +": ");
		//Scanner input = new Scanner(System.in);
		//int studentAnswer = input.nextInt();
		Scanner get = new Scanner(System.in);
		int studentAnswer = get.nextInt();
		if(studentAnswer == (number1 + number2)){
			System.out.print("Correct. ");
			return true;
		}else{
			System.out.println("Nice try, but the correct answer was " 
					+ (number1 + number2) + ".");
			return false;
		}
	}
}
```

## Console Output
```
Round 1 of 3. Add 4 and 1: 5
Correct. Your score was 0 and is now 5. Your hardness was 5 and is now 10.
Round 2 of 3. Add 5 and 0: 5
Correct. Your score was 5 and is now 15. Your hardness was 10 and is now 20.
Round 3 of 3. Add 10 and 5: 15
Correct. Your score was 15 and is now 35. 
The game is complete. Your final score was 35


```


## console history using git.
I didn't understand the purpose of this consol so I'll try my best,

git push: add the changes to gir
git pull: to retrev the information from git
git add: to add the information to git
