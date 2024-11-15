# 🕹️ DSList - Catálogo de Jogos

Este projeto consiste em uma API para gerenciar uma lista de jogos, permitindo organizar e visualizar informações sobre os games de forma prática e eficiente.

---

## 🚀 Funcionalidades

- Listar jogos disponíveis.
- Ordenar e categorizar jogos em diferentes listas.
- Reorganizar a posição dos jogos em listas.
- Visualizar detalhes de um jogo específico.

---

## 🛠️ Tecnologias Utilizadas

Este projeto foi desenvolvido utilizando o seguinte stack de tecnologias:

- **Java 21**
- **Spring Boot** 4.x (Framework principal)
- **JPA/Hibernate** (Persistência de dados)
- **H2 Database** (Banco de dados em memória para testes)
- **PostgreSQL** (Banco de dados em produção)
- **Swagger UI** (Documentação da API)
- **Maven** (Gerenciamento de dependências)

---

## 🗂️ Estrutura do Projeto

O projeto está dividido nos seguintes módulos principais:

- **Controller**: Define os endpoints REST da aplicação.
- **Service**: Contém a lógica de negócios.
- **Repository**: Responsável pela interação com o banco de dados.
- **Model**: Representação das entidades do domínio.
- **DTO**: Classes para transferência de dados.

---

## 🔧 Como Executar o Projeto Localmente

1. **Pré-requisitos**:
   - Java 17 ou superior.
   - Maven instalado.
   - IDE de sua preferência (Eclipse, IntelliJ, etc.).

2. **Clonar o repositório**:
   ```bash
   git clone https://github.com/eduardomoraesduarte/dslist.git
   cd dslist
   
3. Executar o projeto
   - Importe o projeto como um projeto Maven.
   - Execute a classe principal DslistApplication.

     
🖥️ Endpoints da API

📋 Listar todos os jogos
GET /games

📋 Detalhar um jogo específico
GET /games/{id}

📋 Listar jogos de uma lista específica
GET /lists/{listId}/games

📋 Mover posição de um jogo em uma lista
POST /lists/{listId}/replacement
Esse endpoint realiza a movimentação de um elemento dentro de uma lista.

---

📜 Licença

Este projeto foi desenvolvido de forma autoral, com base nos conceitos e orientações apresentados durante um programa conduzido pelo professor Nélio Alves.
