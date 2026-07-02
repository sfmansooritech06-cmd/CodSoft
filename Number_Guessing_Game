import java.util.Scanner;
import java.util.Random;

public class NumberGuessingGame {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Random rand = new Random();

        int lowerBound = 1;
        int UpperBound = 100;
        int maxAttempts = 7;
        int score = 0;
        int round = 1;
        boolean playAgain = true;

        System.out.println("Welcome to the Number Guesing Game");

        while (playAgain) {
            int numberToGuess = rand.nextInt(UpperBound - lowerBound + 1) + lowerBound;
            int attempts = 0;
            boolean guessedCorrectly = false;

            System.out.println("\n--- Round" + round + "---");
            System.out.println("Guess the number between" + lowerBound + "and" + UpperBound + ".");
            System.out.println("You have " + maxAttempts + " attempts.");

            while (attempts < maxAttempts) {
                System.out.println("Attempt" + (attempts + 1) + ":");
                int guess;

                if (sc.hasNextInt()) {
                    guess = sc.nextInt();
                    attempts++;

                    if (guess == numberToGuess) {
                        System.out.println("Correct! you guess the number in " + attempts + "attempts.");
                        score++;
                        guessedCorrectly = true;
                        break;
                    } else if (guess < numberToGuess) {
                        System.out.println("Too low");
                    } else {
                        System.out.println("Too High!");
                    }
                } else {
                    System.out.println("Invalid input! plz enter a number.");
                    sc.next();
                }
            }
            if (!guessedCorrectly) {
                System.out.println("Sorry,you used all attempts. The number was " + numberToGuess + ".");
            }
            System.out.println("Do you want to play another round? (y/n): ");
            String response = sc.next();
            if (!response.equalsIgnoreCase("y")) {
                playAgain = false;
            }

            round++;

        }
        System.out.println("\n Game over! your total score:" + score + "round(s) won.");
        sc.close();
    }
}
