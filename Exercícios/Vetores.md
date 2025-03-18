## Elementos de um vetor
 O código a seguir pede ao usuário a quantidade de elementos do vetor e imprime a posição e o valor do maior e menor elemento do vetor.
```java
import java.util.Scanner;

public class Main5 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("Digite a quantidade de elementos do vetor: ");
        int n = sc.nextInt();

        int[] vetor = new int[n];

        System.out.println("Digite os elementos do vetor: ");
        for (int i = 0; i < n; i++) {
            vetor[i] = sc.nextInt();
        }

        int maior = vetor[0];
        int menor = vetor[0];
        int posicaoM  = 0;
        int posicaoN = 0;

        for (int i = 1; i < n; i++) {
            if(vetor[i] > maior) {
                maior = vetor[i];
                posicaoM = i;
            }
            if(vetor[i] < menor) {
                menor = vetor[i];
                posicaoN = i;
            }
        }

        System.out.println("O maior elemento do vetor é " + maior + " na posição " + posicaoM + " e o menor é " + menor + " na posição " + posicaoN);
    }
}

```
