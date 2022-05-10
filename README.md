# Anotações Postgre
Para criar um banco de dados aperte em Databases com o botão direito depois create > database..

Para criar uma tabela aperte com o botão direito do mouse no banco de dados e selecione a opção Query Tool

### Explicando linhas passo a passo
Esse código serve para criar a tabela
~~~sql
create table nomedatabela(

)
~~~
Dentro dele você vai especificar quais vão ser os nomes das colunas, os tipos, quantidade de caractere máximo ou mínimo e se o campo pode ser vázio ou não  
~~~sql
create table nomedatabela(
     id serial primary key,
     descricao varchar(100) not null
)
~~~
Nome da coluna = descricao, tipo = varchar (significa cadeia de caracteres), (100) é o tamanho máximo de caracteres que podem oculpar um campo dessa coluna e not null = o campo é obrigatório
