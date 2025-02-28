__Loops__
================================

Laços de iteração ou simplesmente loops, são comandos que permitem iteração de código, ou seja, que comandos presentes no bloco se repitam quantas vezes forem necessárias.

* Estruturas:
    * For (para);
    * While (enquanto);
    * Do While (faça enquanto);

__For__
----------------

Permite que uma variável contadora seja testada e incrementada em cada iteração, sendo essas informações definidas na chamada de comando. O comando *for* recebe como entrada uma variável contadora, a condição e o valor da incrementação.

Ex:
``` java
    package repeticao;
public class ForAula {
    public static void main(String[] args) {
        for (int k = 1; k <= 20; k++){
            System.out.println("Contagem numérica " + k);
        }    
    }
}
```

__Arrays__:
``` java
package repeticao;

public class ForArray {
    public static void main(String[] args) {
        String usuarios [] = {"FELIPE", "JONAS", "JULIA", "MARCOS"};
        for (int cont = 0; cont<=usuarios.length ; cont++){
            int posicao = cont + 1;
            System.out.println("O usuário " + usuarios[cont] + " é o número " + posicao + " da fila.");
        }
    }
}
```

__For Each__ : O uso do for / each está fortemente relacionado com um cenário onde contenha um array ou coleção, e assim, a iteração é baseada aos elementos da coleção.

Ex:
``` java
package repeticao;

public class ForEach{
    public static void main(String[] args) {
        String usuarios [] = {"FELIPE", "JONAS", "JULIA", "MARCOS"};
        for(String usuario : usuarios){
            System.out.println("Nome do usuário é " + usuario);
        }
    }
}
```

**Break Continue**
-------------

_Break_ siginifica quebrar, parar, interromper, e essa é exatamente sua função. _Continue_, continua o laço. _Break_ interrompe o laço, já _continue_ interrompe somente a iteração atual.

__While e Do While__
-------------------

O laço _while_ (enquanto) determina que enquanto uma condição for válida, o bloco de código será executado. O laço _while_ testa a condição antes de executar o código, logo se a condição for inválida o bloco não será executado.

Ex:
``` java
package repeticao;
import java.util.concurrent.ThreadLocalRandom;
public class WhileAula {
    public static void main(String[] args) {
        double mesada = 50.0;
        int doceTotal = 0;
        while (mesada>0){
            Double valorDoce = valorAleatorio();
            if (valorDoce>mesada){
                valorDoce = mesada;
            }
            System.out.println("Doce do valor: " + valorDoce + " adicionado no carrinho.");
            mesada = mesada - valorDoce;
            doceTotal++;
        }
        System.out.println("Mesada: " + mesada);
        System.out.println("Joaozinho gastou toda sua mesada em doces e comrpou " + doceTotal + " doces.");
    }
    private static double valorAleatorio(){
        return ThreadLocalRandom.current().nextDouble(2,8);
    }
}
```

O laço _do / while_ (faça... enquanto), considera que enquanto uma determinada condição for válida o bloco de código será executado como no laço _while_ a diferença sendo que nessa estrutura se testa após executar o bloco código independente de a condição ser inválida o bloco será executado no mínimo uma vez.

Ex:
```java
package repeticao;
import java.util.Random;
public class DoWhileAula {
    public static void main(String[] args) {
        System.out.println("Discando... ");
        do { 
            System.out.println("Telefone tocando... ");
        } while (ringing());
        System.out.println("Alô!");
    }
    private static boolean ringing(){
        boolean pickup = new Random().nextInt(3)==1;
        System.out.println("Atendeu? " + pickup);
        return ! pickup; // Exclamação = negar na booleana
    }
}
```