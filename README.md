# Literalura: Um aplicativo Spring Boot para gerenciar dados de livros

Literalura é um aplicativo Java construído com Spring Boot que permite buscar e gerenciar informações sobre livros e autores. Ele utiliza a API pública Gutendex, uma fonte de dados sobre livros e autores, e armazena as informações em um banco de dados PostgreSQL. O aplicativo oferece uma interface de linha de comando amigável para interagir com suas funcionalidades.

## Funcionalidades

* Buscar livros por título usando a API Gutendex
* Visualizar uma lista de todos os livros registrados no banco de dados do aplicativo
* Visualizar uma lista de todos os autores registrados no banco de dados do aplicativo
* Encontrar autores que estavam vivos em um determinado ano
* Filtrar livros por idioma
* Buscar um autor por nome
* Ver uma lista dos 10 livros mais baixados
* Gerar estatísticas de downloads de livros

## Tecnologias Utilizadas

* **Java 17:** Linguagem de programação principal
* **Spring Boot:** Framework para desenvolvimento rápido de aplicativos
* **Spring Data JPA:** Simplifica a interação com o banco de dados PostgreSQL
* **PostgreSQL:** Banco de dados relacional para persistência de dados
* **Maven:** Gerencia as dependências e compilação do projeto
* **API Gutendex:** Fornece dados sobre livros e autores

## Pré-requisitos

Antes de executar o aplicativo, você precisará ter instalado:

* Java 17 ou superior
* Maven
* PostgreSQL
* Acesso à API Gutendex

## Configuração do Banco de Dados

Crie um banco de dados PostgreSQL e configure as credenciais no arquivo `application.properties`:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/literalura
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
spring.jpa.hibernate.ddl-auto=update
```

## Executando o Aplicativo

1. Clone este repositório

```bash
git clone https://github.com/thiagofelipedev/Challenge_literalura
cd Challenge_literalura
```

2. Compile o projeto

```bash
mvn clean install
```

3. Execute o aplicativo

```bash
mvn spring-boot:run
```

4. Interaja com as funcionalidades do aplicativo através do menu de linha de comando.

## Estrutura do Projeto

O projeto está organizado em vários componentes principais:

* Model: Representa as entidades de dados (livros e autores)
* Service: Contém a lógica principal do aplicativo
* Repository: Fornece uma interface para interagir com o banco de dados
* Principal: Lidar com a interação do usuário através da linha de comando


Este desafio foi proposto pela Alura em parceria com a Oracle no programa ONE, no cronograma das atividades dos cursos de Java/ Spring Framework da especialização Back-End.

