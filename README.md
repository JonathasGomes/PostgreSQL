# Anotações Postgre
Eu frequentemente esqueço como usar algumas funções do banco de dados, então decidi criar esse guia para me ajudar a lembrar do que eu preciso de uma forma mais rápida e fácil 
## Criando Banco de Dados, Tabelas e Colunas
Para criar um banco de dados aperte em Databases com o botão direito depois create > database..<br>
Para criar uma tabela aperte com o botão direito do mouse no banco de dados e selecione a opção Query Tool
### Explicando linhas passo a passo
Esse código serve para criar a tabela
~~~sql
create table nomedatabela(

)
~~~
Dentro dele você vai especificar quais serão os nomes das colunas, os tipos, quantidade de caractere máximo e se o campo pode ser vázio ou não  
~~~sql
create table nomedatabela(
     id serial primary key,
     descricao varchar(100) not null
)
~~~
Nome da coluna = descricao, tipo = varchar (significa cadeia de caracteres), (100) é o tamanho máximo de caracteres que podem ocupar um campo dessa coluna e not null = o campo é obrigatório

Depois de ter digitado o código aperte no botão de Execute (F5) para a tabela e as colunas serem criadas, para acessar a tabela vá em Database > nome do banco de dados que você colocou > Schemas > Tables > nomedatabela, botão direito do mouse na tabela > View/Edit Data > All Rows 

## Editar Tabela e Colunas
Browser > nomedatabela, botão direito do mouse na tabela > Properties<br>
Nessa janela você consegue editar tabela e colunas
## Editar Campos
**Primeiro passo abra a Query Tool**
### Insert
Para inserir dados na tabela digite o código
~~~sql
insert into 
~~~
Depois digite o nome da tabela e entre parênteses digite o nome da coluna, em seguida digite values e o dado que deseja que seja inserido na coluna
~~~sql
insert into nomedatabela (descricao) values ('teste')
~~~
### Update
Para atualizar dados na tabela digite o código
~~~sql
update
~~~
Depois digite o nome da tabela mais set e o nome da coluna, entre aspas simples coloque o novo dado e especifique qual é o identificador do dado que você deseja alterar (where id = 1)  
~~~sql
update nomedatabela set descricao = 'teste2' where id = 1
~~~
### Delete
Para deletar dados na tabela digite o código
~~~sql
delete from
~~~
## Créditos
https://www.youtube.com/watch?v=k4wYRoMvBwE&list=PLWd_VnthxxLe660ABLFZH26CW3G-uQIv-&index=1
