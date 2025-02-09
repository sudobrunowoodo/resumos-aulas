Classe
============= 

Definição: 
-------------
Arquivo, todo o código está dentro dela, public class nome da classe coerente

Ex:
``` java
        public class Aula1{ 

        }
```

Aula:
--------------
1. Convenções 
    a. Cada palavra das classes em letra maiúsculas;
    b. Todo arquivo .java;
    c. Variáveis com letra minúscula, palavra composta segunda com letra maiúscula, em nomes somente letras, _ , $ e números;
    d. Nome da variável inteiramente maiúscula Significa que é imutável;

2. Variáveis
    a. Tipo NomeBemDefinido = Atribuição de valor;
    b. Mesmo que mude o valor o tipo permanece; 

3. Criar Metódos
    a. TipoRetorno NomeObjetivoInfinitivo Parametro(s) {corpo};
        Ex:
    ``` java
            public static String nomeCompleto ( String primeiroNome, String segundoNome ) {
                return "Resultado do método " + primNome + " " + segNome;
            }
    ```
    b. Igual definir funções em Python;

4. Identação
    a. Forma de tabular o código a nível de escopo;
    b. Melhorar visualização;

5. Organinzando Arquivos (Packages)
    a. Tipo de projeto.nome da empresa.nome do projeto.subfinalidades(se houver);
        Ex: 
            com.kaimancalçados.notification

6. Java Beans
    a. Convenções envolvendo legibilidade dos algoritmos;
    b. Variável clara, sem abreviação, definição sem sentido, sempre no singular a n ser q seja um array ou coleção, idioma único para as variáveis;
    c. Métodos nomeados como verbo, mistura de letras minúsculas e maiúsculas;

Hierarquia:
-------------------
Pacote/Classe/Método/Resto
{ } Corpo ( ) Parametros [ ] Arrays " " Strings

Tipos e Variáveis
===============

Ver tipos de dados e suas aplicabilidades.

Tipos de dados:
----------------
1.  Int, byte, short, long, float, double, boolean e char:
    a.  Tipos primitivos, representam valores brutos, armazenados diretamente na pilha de memória (Memory Stack);
    b.  Inteiros: int, byte, short, long. Mais comum sendo int;
    c.  long termina com L, float com F;
    d.  Fracionários: float, double.

2.  Variáveis/Constantes
    a.  final mantém constante os valores;
    b.  Convenção final Caixa Alta; 
         Ex:
```java
             final int idade = 45;
```

Operadores
==============

Apresentar e explicar simbolos especiais em Java.

Classificação
-----------

1.  Atribuição "="
    a.  Coloca valor inicial em uma variável.

2.  Aritméticos "+ - * /"
    a.  Realizar operações numéricas.
    b.  Adição usada em textos funciona para concatenar (juntar textos).

3.  Unários
    a.  Aplicados juntos a outros operadores, realizam trabalhos básicos como incrementar, decrementar, inverter valores numéricos e booleanos.
    b.  "+" valot positivo, "-" valor negativo, "++" incrementar valor 1 unidade, "--" decremento valor 1 unidade; (!) negação ou inversão do valor de uma expressão booleana.
    c.  Funcionam como prefixo e sufixo.

4.  Ternário
    a.  Forma resumida de condição.
    b.  Única linha.
    c. "?:" representação -> condição ? verdadeiro : falso.

5.  Relacionais
    a.  Checam a relação entre variáveis.
    b.  "==" igualdade, "!=" diferença, ">" maior q, ">=" maior ou igual q, "<" menor q, "<=" menor ou igual q.
    c. Vários tipos de comparação.
    d. equals() comparação de conteúdo. Melhor para objetos.
6.  Lógicos
    a. Recurso para criar expressões lógica maiores, junção de várias condições.
    b.  "&&" operador lógico e, || operador lógico ou.

Métodos
==========

Critérios para visualização de métodos, parametros e visibilidade.
Classe dividida por atributos e métodos. Atributos são variéveis ou tipos de valores, métodos sao funções ou sub-rotinas dentro das classes.

1.  Critérios de nomeação de métodos
    a.  Deve ser nomeado como verbos bem explicativos e de acordo com a proposta, seguir padrão camelCase.

2.  Critérios de definição de métodos
    a.  Qual a proposta principal do método?
    b.  Qual tipo de retorno esperado após executar o método?
    c.  Quais parâmetros necessários para execução do método?
    d.  O método possui risco de apresentar alguma exceção?
    e.  Qual a visibilidade do método? Toda aplicação, somente em pacotes, através da herança ou somente na propria classe.

Escopo
============

Identificar a localização mais conveniente para a escrita de algoritmos para o nosso programa, também pode ser entendido como o ambiente onde a variável pode ser acessada. Variáveis criadas dentro de metódos e de blocos só podem ser acessada dentro dos próprios locais.

Palavras Reservas
===========

Listagem de palavras reservadas, para classificação e usabilidade melhorada. Identificadores de uma liguagem que já possuem finalidade específica.

Lista por funções:
---------------
    a.  Controle de pacotes: import(pacotes ou classes), package(especifica o pacote no qual todas as classes de arquivos pertencem).
    b.  Modificadores de acesso: public(acesso a qualquer classe), private(acesso só dentro da classe), protected(acesso por classes no mesmo pacote e subclasses).
    c.  Primitivos: byte, boolean, char, double, float, short, int, long, void(nenhum valor/tipo).
    d.  Modificadores de classe: abstract(classe que não pode ser instanciada), class, extends(indica a superclasse que a subclasse está extendendo), final(variável imutável), implements(indica as interfaces que uma classe irá implementar), interface, native, new(cria novo objeto), static(Recurso que determina que não é preciso criar um objeto para usufruin dos seus recursos), stricttfp, synchronizaed(manter a integridade de execuções multi-threading), transient(impede serialização de campos), volatile(variável pode ser alterada durante uso de threads).
    e.  Controle de fluxo dentro de um bloco de código: break(sai do bloco de codigo em que está), case(executa um bloco de código dependendo do teste do switch), continue(pula execução do código que viria após essa linha e vao para a próxima passagem de loop), default, do, else, for, if, instanceof, return, switch, while.
    f.  Tratamento de erros: assert, catch, finally, throw, throws, try.
    g.  Variáveis de referência: super, this.
    h.  Palavras reservada não utilizadas: const, goto.
    j.  Literais reservado: null, true, false.

Java Doc
=================

Ficar revisando para melhor entendimento [Java_documentação](https://docs.oracle.com/javase/7/docs/api/overview-summary.html)

Tags
---------------

/**
h1> Definição da classe /h1>
Descrição
p> 
b>Note:/b> Mais notas
@author
@version
@since
*/
/**
*Documentação
*@param explicação dos parâmetros
*@return explicação dos resultados
*/

ex:
```java
    /**
    * <h1>Calculadora</h1>
    * A Calculadora realiza operações matemáticas entre números inteiros
    * <p>
    * <b>Note:</b> Leia atentamente a documentação desta classes
    * para desfrutar dos recursos oferecidos pelo autor
    *
    * @author  Gleyson Sampaio
    * @version 1.0
    * @since   01/01/2022
    */
    public class Calculadora {
        /**
        * Este método é utilizado para somar dois números inteiros
        * @param numeroUm este é o primeiro parâmetro do método
        * @param numeroDois este é o segundo parâmetro do método
        * @return int o resultado deste método é a soma dos dois números.
        */
    public int somar(int numeroUm, int numeroDois) {
        return  numeroUm + numeroDois;
    }
    }
```
Tipos de comentários:
--------------

1.  One line;
    Ex: // Comentário única linha
2.  Mult line;
    Ex: /*Comentário
         *mais
         *de
         *uma
         *linha
        */
3.  Documentation;
    Ex: /**
         * Documentação
         *
         * 
         */

Javadoc
----------------

É um gerador de documentação para documentar a API dos progrmas em Java, a partir do código-fonte

No terminal execute o comando abaixo
javadoc -encoding UTF-8 -docencoding ISO-8859-1  -d ../docs  src/*.java

Terminal e Argumentos
===============

Quando executamos uma classe que contenha o método main, o mesmo permite que passemos um array [] de argumentos do tipo String. Logo podemos após a definição da classe a ser executada informar estes parâmetros.
    EX:
```java
public class AboutMe {
    public static void main(String[] args) {
        //os argumentos começam com indice 0
        String nome = args [0];
        String sobrenome = args [1];
        int idade = Integer.valueOf(args[2]); //vamos falar sobre Wrappers
        double altura = Double.valueOf(args[3]);

        System.out.println("Ola, me chamo " + nome + " " + sobrenome);
        System.out.println("Tenho " + idade + " anos ");
        System.out.println("Minha altura é " + altura + "cm ");
    }
}
```