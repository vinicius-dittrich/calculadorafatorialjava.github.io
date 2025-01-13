# calculadorafatorialjava.github.io
Calculadora de Fatorial em Java
import java.util.Scanner;

public class CalculadoraFatorial {
    public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Digite um número positivo e inteiro: ");
            int numero = scanner.nextInt();
            
            if (numero < 0) {
                System.out.println("O número deve ser positivo e inteiro.");
            } else {
                long fatorial = 1;
                for (int i = 1; i <= numero; i++) {
                    fatorial *= i;
                }
                System.out.println("O fatorial de " + numero + " é: " + fatorial);
            }
        }
    }
}
