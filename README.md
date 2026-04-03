# Desafio: Modelo de Domínio e ORM

Projeto desenvolvido como parte do curso da DevSuperior (Prof. Nélio Alves), com foco em modelagem de domínio e mapeamento objeto-relacional (ORM) utilizando Spring Boot e JPA.

## 🚀 Tecnologias
- Java 17+
- Spring Boot
- Spring Data JPA
- H2 Database
- Maven

## 📚 Descrição do projeto

O sistema simula o gerenciamento de participantes em atividades de um evento acadêmico, como cursos e oficinas.

## 🧩 Funcionalidades modeladas
- Cadastro de participantes
- Cadastro de atividades
- Associação entre participantes e atividades (M)
- Organização de atividades por categoria
- Divisão das atividades em blocos de horário
- 
## 🗂️ Modelo de domínio

O sistema possui as seguintes entidades:

- Participante
- Atividade
- Categoria
- Bloco

## 🔗 Relacionamentos
- Participante ↔ Atividade → Muitos-para-muitos (M:N)
- Atividade → Categoria → Muitos-para-um (N:1)
- Atividade → Bloco → Um-para-muitos (1:N)

## 🌱 Seeding da base de dados

O banco de dados é automaticamente populado com dados iniciais através do arquivo:

- import.sql

Isso garante que, ao iniciar a aplicação, os dados já estejam disponíveis para teste.

## ⚙️ Como executar o projeto
### 📌 Pré-requisitos
- Java 17 ou superior 

## ▶️ Rodando a aplicação

No terminal, execute:
```bash
./mvnw spring-boot:run
```

## 🗄️ Acessando o banco H2

Após iniciar o projeto, acesse:

👉 http://localhost:8080/h2-console

🔑 Dados de conexão:
- JDBC URL: jdbc:h2:mem:testdb
- User: sa
- Password: (vazio)

## 📄 Licença

Este projeto está sob a licença MIT.

## 👩🏻‍💻 Autor

Alina Sobral