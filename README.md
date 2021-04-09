<h2>Desenvolvimento de testes unitários para validar uma API REST de gerenciamento de estoques de cerveja.</h2>
Desenvolvimento de testes unitários para validar o nosso sistema de gerenciamento de estoques de cerveja. Testes unitários com JUnit e Mockito. 


Para executar o projeto no terminal, digite o seguinte comando:

```shell script
mvn spring-boot:run 
```
Para iniciar banco de dados Docker digite o comando
```shell script
docker-compose up 
```

Para executar a suíte de testes desenvolvida durante a live coding, basta executar o seguinte comando:

```shell script
mvn clean test
```

Após executar o comando acima, basta apenas abrir o seguinte endereço e visualizar a execução do projeto:

```
http://localhost:8080/api/v1/beers
```

São necessários os seguintes pré-requisitos para a execução do projeto:

* Java 14 ou versões superiores.
* Docker-compose 
* Maven 3.6.3 ou versões superiores.
* Controle de versão GIT instalado na sua máquina.


Para criar as tabelas, execute o comando abaixo no gerenciados de Banco de Dados:
```
CREATE TABLE beer (
    ID bigint NOT NULL AUTO_INCREMENT,
    name varchar(255) NOT NULL,
    brand varchar(255),
    max int,
    quantity int,
    type varchar(255),
    PRIMARY KEY (id)
);
```

