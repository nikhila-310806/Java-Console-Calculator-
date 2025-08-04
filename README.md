# Java-Console-Calculator-
This Java console calculator is a simple, user-friendly application designed to perform basic arithmetic operations such as additthe, subtraction, multipladdition and division. Users can interact with the calculator through a command-line interface, selecting operations and inputting numbers to obtain results. 
import java.util.Scanner;

public class ConsoleCalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("---- Java Console Calculator ----");
        System.out.print("Enter first number: ");
        double num1 = scanner.nextDouble();
        System.out.print("Enter an operator (+, -, *, /): ");
        char operator = scanner.next().charAt(0);
        System.out.print("Enter second number: ");
        double num2 = scanner.nextDouble();
        double result;
        switch (operator) {
            case '+':
                result = num1 + num2;
                System.out.println("Result: " + result);
                break;
            case '-':
                result = num1 - num2;
System.out.println("Result: Result: " + result);
                break;
                case '*':
                result = num1 * num2;
                System.out.println("Result: " + result);
                break;
                case  '/':
                 if (num2 != 0) {
                    result = num1 / num2;
                    System.out.println("Result: " + result);
                } else {
                    System.out.println("Error: Division by zero!");
                }
                break;
              default:
                System.out.println("Invalid operator!");
        }
        scanner.close();
  }
}
        
   
            


        

        

        

    
