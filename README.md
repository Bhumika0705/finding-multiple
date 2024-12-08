# finding-multiple
This code will give you multiple of  any number
import java.util.Scanner;

public class multiple {
    public multiple() {
    }

    static void go(int n, int k, int i) {
        if (k != 0) {
            System.out.println(n * i + " ");
            go(n, k - 1, i + 1);
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int k = sc.nextInt();
        go(n, k, 1);
    }
}
