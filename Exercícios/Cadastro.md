# Cadastro de funcionários
O exercício a seguir pede ao usuário informações sobre um funcionário e imprime suas informações no trabalho: empregado/aposentado, salario alto/baixo.
```java
import java.util.Scanner;

public class Main5 {
    public static void main(String[] args) {
        String nome;
        int idade;
        float salario;
        Scanner sc = new Scanner(System.in);

        System.out.println("Digite o nome do funcionário: ");
        nome = sc.nextLine();

        System.out.println("Digite a idade do funcionário: ");
        idade = sc.nextInt();

        if (idade > 60) {
            System.out.println("Funcionário aposentado.");
        } else {
            System.out.println("Digite o salário do funcionário: ");
            salario = sc.nextFloat();

            if (salario > 5000) {
                System.out.println("Salário alto.");
            } else {
                System.out.println("Salário baixo");
            }
        }
    }
}
```
