import java.util.Scanner;

/*
   *  3 números inteiros, imprimir o menor e o maior
   * Método que executa o programa
   * public = É visto em qualquer lugar da aplicação. É o modificador de acesso
   * static = é iniciado automaticamente pela JVM, sem precisar de uma instância
   * void = Método sem retorno (retorno vazio)
   * main = Nome do método, que é obrigatório ser este. Recebe como parâmetro um array de String.
   * String[] args = Array de argumentos que podem ser repassados na chamada do programa.
*/

public class MenorMaior {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n1, n2, n3;

        System.out.print("Informe  o primeiro número: ");
        n1 = sc.nextInt();
        System.out.print("Informe  o segundo número: ");
        n2 = sc.nextInt();
        System.out.print("Informe o terceiro número: ");
        n3 = sc.nextInt();
        if (n1 > n2) {
            if (n1 > n3) {
                if (n2 < n3) {
                    System.out.println("O menor numero: " + n2);
                } else {
                    System.out.println("O menor numero: " + n3);
                }
                System.out.println("O maior numero: " + n1);
            } else {
                if (n1 < n2) {
                    System.out.println("O menor numero: " + n1);
                } else {
                    System.out.println("O menor numero: " + n2);
                }
                System.out.println("O maior numero: " + n3);
            }
        } else {
            if (n2 > n3) {
                if (n1 < n3) {
                    System.out.println("O menor numero: " + n1);
                } else {
                    System.out.println("O menor numero: " + n3);
                }
                System.out.println("O maior numero: " + n2);
            } else {
                if (n1 < n2) {
                    System.out.println("O menor numero: " + n1);
                } else {
                    System.out.println("O menor numero: " + n2);
                }
                System.out.println("O maior numero: " + n3);
            }
        }
    }
}
