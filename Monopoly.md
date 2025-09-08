import java.util.Scanner;

public class Monopoly {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int T = sc.nextInt();  

        for (int i = 0; i < T; i++) {
            int P = sc.nextInt();
            int Q = sc.nextInt();
            int R = sc.nextInt();
            int S = sc.nextInt();

     
            int total = P + Q + R + S;

          
            if (P > total - P || Q > total - Q || R > total - R || S > total - S) {
                System.out.println("YES");
            } else {
                System.out.println("NO");
            }
        }

        sc.close();
    }
}
