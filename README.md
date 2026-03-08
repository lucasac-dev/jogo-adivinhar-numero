jogo simples aonde o jogador precisa acertar um número gerado aleatoriamente entre 1 e 100.

# características
- Geração de número aleatório
- Dicas (se o valor digitado é alto/baixo)

# Recursos
- Java
- Scanner
- Random
 




      package advinheonumero;
      import java.util.Random;
      import java.util.Scanner;

    
      public class Adivinheonumero {
    
    
      public static void main(String[] args) {
       
        
        Scanner scanner = new Scanner(System.in);
        Random random = new Random();
        
        int numeroSecreto = random.nextInt(100) + 1;
        int tentativa;
        
        System.out.println("Tente adivinhar o numero entre 1 e 100");
        
        do{
            System.out.print("Digite seu palpite: ");
            tentativa = scanner.nextInt();
            
        if (tentativa > numeroSecreto) {
            System.out.println("Muito alto");
                    
        }
        
        else if (tentativa < numeroSecreto) {
            System.out.println("Muito baixo");
        
        }
      
      }while (tentativa != numeroSecreto);
            System.out.println("Voce acertou");
        
    }
}a…]()



