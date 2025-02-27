Estruturas Condicionais
====================================

Possibilita a escolha de um grupo de ações e comportamentos a serem executados quando determinadas condições são ou não satisfeitas. Se dividem em Condicionais Simples e Compostas.

Condicionais Simples
------------------------------------

Quando ocorre uma validação de execução de fluxo somente quando a condição é positiva, consideramos uma estrutura simples.

Ex:
``` java
public class CondicionalSimples {
public static void checarSaldo (double saldo , double valorSolicitado){
    if (valorSolicitado < saldo) {
        saldo = (saldo - valorSolicitado);
        System.out.println(saldo);
        }
    }
    
public static void main(String[] args) throws Exception {
    CondicionalSimples.checarSaldo(25,17);
        }
}
``` 

Condicionais Compostas
---------------------------

Algumas vezes o nosso programa deverá seguir mais de uma jornada de excução condicionada a uma regra de negócio, este cenário é denominado Estrutura Condicional Composta.

Ex:
``` java
public class CondicionalComposta {
    public static void verificarNota(double nota){
        if (nota >= 7 ) {
            System.out.println("Aprovado!");
        }
        else
            System.out.println("Reprovado!");
    }
    public static void main(String[] args) {
        verificarNota(8);
    }
}
```

Condicionais Encadeadas
----------------------

Em um controle de fluxo condicional, nem sempre nos limitamos ao se(if) e senão(else), poderemos ter uma terceira, quarta e ou inúmeras condições.

Ex:
``` java
public class CondicionalEncadeada {
    public static void verificarNota(double nota){
        if (nota >= 7 ) {
            System.out.println("Aprovado!");
        }
        else if (nota >= 5 && nota < 7){
            System.out.println("Recuperação!");
        }
        else
            System.out.println("Reprovado!");
    }
    public static void main(String[] args) {
        verificarNota (4);
    }
}
``` 

Condição Ternária
----------------------

Como vimos em operadores, podemos abreviar nosso algorítmico condicional refatorando com o conceito de operador ternário.

Ex (Otimizando os exemplos anteriores):
``` java
public class CondicaoTernaria {
    public static void verificarNota(double nota){
    String resultado = nota >= 7 ? "Aprovado!" : nota >= 5 && nota < 7 ? "Recuperação!" : "Reprovado!";
    System.out.println(resultado);
    }
    public static void main(String[] args) {
        verificarNota(6);
    }
}
```

"?" mostra o resultado para se (if) ":" para senão (else) ": + condição + ?" elif.

Switch Case
-----------------------

A estrutura switch compara o valor de cada caso com o da variável sequencialmente, e sempre que encontra um valor correnspondente, executa o código associado ao caso. Para evitar que as comparações continuem a ser executadas após um caso correspondente ter sido encontrado, acrescentamos o comando break no final de cada bloco de códigos. O comando break, quando executado, encerra a execução da estrutura onde ele se encontra. 

Ex:
``` java
public class SwitchCase {
    public static void verificarPlano(String plano) {
        switch (plano) {
            case "T":{
                System.out.println("5Gb de Youtube");
            }
            case "M":{
                System.out.println("Whats e Instagram grátis");
            }
            case "B":{
                System.out.println("100 minutos de ligação");
            }   
        }
    }
    public static void main(String[] args) {
        verificarPlano("M"); // Plano Midia "M" Plano Basic "B" Plano Turbo "T"
    }
}

```