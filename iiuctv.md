import java.util.Scanner;

public class iiuctv {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int x = scanner.nextInt(); 
        int n = 6; 

        if (x >= n) {
            System.out.println("Able to buy subscription");
        } else {
            System.out.println("NOT able to buy subscription");
        }

        int minimum_cost = x / n;
        System.out.println("Minimum cost division result: " + minimum_cost);

        scanner.close();
    }
}
