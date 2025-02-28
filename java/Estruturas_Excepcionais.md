Estruturas Excepcionais
==============

Exceções
---------------

Ao executar o código Java, diferentes erros podem acontecer: erros de codificação feitos pelo programador, erros devido a entrada errada ou outros imprevistos.

Ao ocorrer um erro, o Java para e gera uma mensagem de erro: Java lançará uma _exceção_ (Throws Exception).

De forma interpretativa em Java, um erro é algo irreparável, a aplicação trava ou é encerrada drasticamente. Já exceções é um fluxo inesperado da nossa aplicação, exemplo: Querer dividir um valor por zero, querer abrir um arquivo que não existe, abrir uma conexão de banco com usuários ou senha inválida. Todos estes cenários e os demais não são erros mas sim fluxos não previstos pela aplicação.

O tratamento de exceções é o realizado ao prever estas situações.

Exemplos de exceções:
|<center>Exceção|<center>Causa|
|:-----|:------|
|java.lang.NullPointerException|Quando tentamos obter alguma informação de uma variável nula.|
|java.lang.ArithmeticException	|Quando tentamos dividir um valor por zero.|
|java.sql.SQLException|Quando existe algum erro relacionado a interação com banco de dados.|
|java.io.FileNotFoundException|Quando tentamos ler ou escrever em um arquivo que não existe.|

Podemos usar as instruções _try_, _catch_ e _finally_ para tratar exceções.
_Try_: Permite que seja definido um bloco de código a ser testado por exceções enquanto é executado.
_Catch_: Permite definir um bloco de código a ser executado, caso uma exceção apareça no try.
_Finally_: Permite definir um bloco de código a ser executado independente de existirem erros ou não.
Como visto na definição do código abaixo.
``` java
try {
  //  bloco de código conforme esperado
}
catch(Exception e) {// precisamos saber qual exceção
  // bloco de código que captura as exceções que podem acontecer
  // em caso de um fluxo não previsto
}
```

Hierarquia de Exceções
------------------------------------

Dispõe de uma variedade de classes que representam exceções, e estas classes são organizadas em uma hierarquia demoninadas `Checked and Unchecked Exceptions` ou _Exceções Checadas e Não Checadas_.

