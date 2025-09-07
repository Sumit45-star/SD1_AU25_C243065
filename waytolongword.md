import java.util.Scanner;

public class WayTooLongWords {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
      
        int n = scanner.nextInt();
        scanner.nextLine(); 
                for (int i = 0; i < n; i++) {
            String word = scanner.nextLine();
            System.out.println(abbreviate(word));
        }
        
        scanner.close();
    }
    
        private static String abbreviate(String word) {
        if (word.length() <= 10) {
            return word; 
        }
        
         int count = word.length() - 2;
        return word.charAt(0) + Integer.toString(count) + word.charAt(word.length() - 1);
    }
}