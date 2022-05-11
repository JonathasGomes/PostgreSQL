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
Nome da coluna = descricao, tipo = varchar (significa cadeia de caracteres), (100) é o tamanho máximo de caracteres que podem ocupar um campo dessa coluna e not null = o campo é obrigatório

Depois de ter digitado o código aperte no botão de Execute (F5) para a tabela e as colunas serem criadas, para acessar a tabela vá em Database > nome do banco de dados que você colocou > Schemas > Tables > nomedatabela, botão direito do mouse na tabela View/Edit Data > All Rows 

## Editar Tabela e Colunas
Browser > nomedatabela, botão direito do mouse na tabela > Properties
Nessa janela você consegue editar tabela e as colunas
## Editar Campos

## Créditos
