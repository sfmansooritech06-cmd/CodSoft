import java.util.Scanner;

public class StudentGrade {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("Enter English marks: ");
        int marks1 = sc.nextInt();

        System.out.println("Enter Hindi marks: ");
        int marks2 = sc.nextInt();

        System.out.println("Enter Science marks: ");
        int marks3 = sc.nextInt();

        System.out.println("Enter Mathematics marks: ");
        int marks4 = sc.nextInt();

        System.out.println("Enter SST marks: ");
        int marks5 = sc.nextInt();

        int average = (marks1 + marks2 + marks3 + marks4 + marks5) / 5;
        float percentage = ((marks1 + marks2 + marks3 + marks4 + marks5) / 5);

        System.out.println("Avearge marks :" + average);
        System.out.println("Student Percentage: " + percentage);

        if (percentage < 33) {
            System.out.println("Grade FAIL");
        } else if (percentage >= 33 && percentage <= 40) {
            System.out.println("Grade D");
        } else if (percentage >= 41 && percentage <= 60) {
            System.out.println("Grade C");
        } else if (percentage >= 61 && percentage <= 80) {
            System.out.println("Grade B");
        } else if (percentage >= 80 && percentage <= 100) {
            System.out.println("Grade A");
        }
    }
}
