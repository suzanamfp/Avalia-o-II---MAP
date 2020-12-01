# Avaliacao-II---MAP

# Padrão DAO

## Centro Universitário UNIESP

### Professora: Drª Alana Morais ([alanamm.prof@gmail.com](mailto:alanamm.prof@gmail.com))

### Aluno: Suzana Maria de Freitas Pereira

## Nome
O acrônimo do inglês DAO (Data Access Object) que quer dizer objeto de acesso a dados, é um padrão de projeto utilizado em aplicações com persistência de dados, que necessitem separar as regras de negócio das regras de acesso a banco de dados, implementado com programação orientada a objetos e arquitetura MVC (Model - View - Controller). 

## Problema
A DAO é responsável pela troca de informações com o SGBD, fornecem operações de bancos de dados conhecidas como CRUD (Create, Update e Delete), devem ser capazes também de realizar a busca de objetos ou listas de objetos no banco de dados, convertendo em instruções SQL e manda para o banco de dados. Toda interação com a base de dados se dará através destas classes (DAO), nunca das classes de negócio, e nem por meio de formulários. 

## Solução
O DAO normalmente é implementada por meio de uma interface comum de acesso aos dados onde se define os métodos que o objeto de acesso irá prover, uma classe que implementa os métodos e suas responsabilidades para realizar o acesso aos dados. A camada de negócio acessará os dados persistidos sem saber quais tipos de dados estão no banco, podendo ser um XML, um arquivo Txt. O padrão manterá em sigilo detalhes da execução da origem dos dados, abstrai e encapsula o acesso a fonte de dados.

## Consequências
 Podemos citar algumas vantagens do padrão DAO como:
- Transparência no acesso aos dados, os objetos de negócio irão acessar a fonte de dados, sem saber como esse acesso foi implementado, ou seja torna o caminho mais limpo, mais transparente.
- Facilidade na migração de um banco de dados para outro, a migração envolverá mudanças apenas na camada DAO.
- Simplicidade de código, tornando a classe de negócio e a DAO com suas devidas responsabilidades, reduzindo a complexidade do código com regras misturadas, ajudando na legibilidade do código e facilitando a sua manutenção.
- Facilidade no gerenciamento, a DAO centraliza o local de acesso aos dados, em uma camada mais isolada para fazer as operações necessárias.

Desvantagens:
A necessidade de desenvolver códigos básicos das operações.

## Referencias

https://www.devmedia.com.br/dao-pattern-persistencia-de-dados-utilizando-o-padrao-dao/30999
https://pt.stackoverflow.com/questions/113840/como-funciona-o-padr%C3%A3o-dao
http://ppgcc.propesp.ufpa.br/Disserta%C3%A7%C3%B5es_2011/Amanda%20Monteiro%20Sizo%20Lino_Disserta%C3%A7%C3%A3o.pdf
