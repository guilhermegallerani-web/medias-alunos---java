# medias-alunos---java 

/**
* Programa que calcula a média das notas de um aluno
 * e informa se ele foi aprovado, ficou de recuperação ou foi reprovado.
 *
 * Autor: Guilherme Gallerani Simões
/*

 
 
 
 public class CalculadoraMediaAlunos {
blic static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
 
        System.out.println("=== CALCULADORA DE MÉDIA DE ALUNOS ===");
 
        // Pede o nome do aluno
        System.out.print("Digite o nome do aluno: ");
        String nome = scanner.nextLine();
 
        // Pede quantas notas serão lançadas
        System.out.print("Quantas notas o aluno terá? ");
        int quantidadeNotas = scanner.nextInt();
  double somaNotas = 0;
 
        // Loop para ler cada nota digitada
        for (int i = 1; i <= quantidadeNotas; i++) {
            System.out.print("Digite a nota " + i + ": ");
            double nota = scanner.nextDouble();
            somaNotas += nota;
        }
 
        // Calcula a média simples
        double media = somaNotas / quantidadeNotas;
 
        // Exibe o resultado formatado
        System.out.println("\n=== RESULTADO ===");
        System.out.println("Aluno: " + nome);
        System.out.printf("Média final: %.2f%n", media);
 
        // Verifica a situação do aluno com base na média
        if (media >= 7.0) {
            System.out.println("Situação: APROVADO");
        } else if (media >= 5.0) {
            System.out.println("Situação: RECUPERAÇÃO");
        } else {
            System.out.println("Situação: REPROVADO");
        }
 
        scanner.close();
    }
}  
 
