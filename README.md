# habit-tracker-java
A cute self-care habit tracker built in Java
// importing scanner so i can get input from the person using it
import java.util.Scanner;

public class HabitTracker {
    public static void main(String[] args) {
        //this lets me take input from the user
        Scanner input = new Scanner(System.in);

        System.out.println("🌸 Welcome to Vania's Self-Care Habit Tracker!! 🌸");
        //^cute into message

        System.out.println("Which habit did you achieve today?");
        System.out.println("1. Gym 🏋🏾‍♀️");
        System.out.println("2. Journal 🧘🏾‍♀️");
        System.out.println("3. Read 📚");
        System.out.println("4. Drink Water 💦");
        //^showing user the list of habits they can track 

        System.out.print("Enter the number (1–4): ");
        int choice = input.nextInt();
        input.nextLine(); // IMPORTANT: clears leftover input
        //asking user to pick (1-4)

        System.out.print("Did you complete it today? (yes/no): ");
        String didIt = input.nextLine(); // allows typing full input

        if (didIt.equalsIgnoreCase("yes")) {
            System.out.println("✨ I’m proud of you! You’re smashing it 💖");
        } else {
            System.out.println("💗 No worries! Tomorrow is a fresh start 🌸");
        }
        //giving cute response based on if they did it or not

        input.close();
    }
}
