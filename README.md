# Fibonacci

public class Fibonacci {

    public static void main(String[] args) {
        int n = 10; // Jumlah bilangan Fibonacci yang ingin dihasilkan
        toastNumber(n);
    }

    public static void toastNumber(int n) {
        int first = 1;
        int second = 1;

        System.out.print("Bilangan Fibonacci (" + n + " angka pertama): ");

        if (n >= 1) {
            System.out.print(first + " ");
        }
        if (n >= 2) {
            System.out.print(second + " ");
        }

        for (int i = 3; i <= n; i++) {
            int next = first + second;
            System.out.print(next + " ");
            first = second;
            second = next;
        }

        System.out.println();
    }
}
