import java.util.Scanner;
import java.util.Random;
public class RockPaperScissorsGame{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        Random random = new Random();
        String choices[] = {"rock","scissors","paper"};
        String UserChoice;
        String ComputerChoice;
        int count = 0;
        String PlayAgain = "yes";

        do {
            System.out.print("Enter Your Move(rock,scissors,paper): ");
            UserChoice = sc.nextLine().toLowerCase();
            if (!UserChoice.equals("rock") && !UserChoice.equals("scissors") && !UserChoice.equals("paper")) {
                System.out.println("Invalid Move");
                continue;
            }
            ComputerChoice = choices[random.nextInt(3)];
            System.out.println("Compueter choice is: " + ComputerChoice);

            if (UserChoice.equals(ComputerChoice)) {
                System.out.println("It is tie");
            } else if ((UserChoice.equals("paper") && ComputerChoice.equals("rock")) ||
                    (UserChoice.equals("scissors") && ComputerChoice.equals("paper") ||
                            UserChoice.equals("rock") && ComputerChoice.equals("scissors"))) {
                System.out.println("You Won!");
                count++;
            } else {
                System.out.println("You Lost");
            }
            System.out.println("Number of points: " + count);
            System.out.println("yes/no");
            PlayAgain = sc.nextLine().toLowerCase();
        }while(PlayAgain.equals("yes"));
        System.out.println("Total Points You Scored : "+ count);
        System.out.println("Thanks For Playing");

    }
}
