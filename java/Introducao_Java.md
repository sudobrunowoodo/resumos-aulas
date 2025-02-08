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
    b.  Inteiros: int, byte, short, long. Mais comum sendo int
    c.  Fracionários: float, double.