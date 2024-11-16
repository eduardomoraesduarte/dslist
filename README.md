# 🕹️ DSList - Catálogo de Jogos

Este projeto consiste em uma API para gerenciar uma lista de jogos, permitindo organizar e visualizar informações sobre os games de forma prática e eficiente.

---

## 💡 Objetivo

- Esse projeto tem como objetivo principal desenvolver e aprimorar habilidades no back-end, com ênfase em Spring Boot, Java e APIs REST, aplicando boas práticas de organização, modelagem de dados e design de sistemas robustos.

---

## 🚀 Funcionalidades

- 📋 Listar jogos disponíveis: Acesse uma lista com todos os jogos cadastrados.
- 🗂️ Ordenar e categorizar jogos: Organize os jogos em diferentes listas.
- 🔄 Reorganizar posições: Altere a ordem dos jogos em uma lista específica.
- 🔍 Visualizar detalhes: Obtenha informações detalhadas de um jogo específico.

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

## 📚 Modelo Conceitual de Entidades:
O projeto foi estruturado com base em um modelo conceitual claro e eficiente, representando as entidades essenciais:

![dslist-model](https://github.com/user-attachments/assets/eb0f16f1-8833-47f0-96d1-7ad913fa045d)

- **Game** (Jogo): Inclui atributos como título, gênero, ano de lançamento e pontuação.
- **GameList** (Lista Jogo): Representa categorias organizadas pelo usuário.
- **Belonging** (Relação Jogo-Lista): Garante a flexibilidade na organização e no posicionamento dos jogos.

---

## 🗂️ Estrutura do Projeto

O projeto está dividido nos seguintes módulos principais:

- **Controller**: Define os endpoints REST da aplicação.
- **Service**: Contém a lógica de negócios.
- **Repository**: Responsável pela interação com o banco de dados.
- **Model**: Representação das entidades do domínio.
- **DTO**: Classes para transferência de dados.

![Padrao camadas](https://github.com/user-attachments/assets/85b3db3d-3030-4d9c-9b76-eccf1f11e0a5)

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

---

## 🌐 Front-End (não incluso)

Este projeto tem seu foco exclusivamente no back-end. No entanto, o front-end pode ser facilmente integrado, utilizando tecnologias modernas para consumir os endpoints da API.

Aqui estão algumas sugestões para um possível front-end:

 - React.js ou Angular: Para criar uma interface web responsiva e interativa.
 - Bootstrap ou Material-UI: Para estilização rápida e consistente.
 - Fetch API ou Axios: Para consumir os endpoints REST da API.

Exemplo:

   - Lista
![List](https://github.com/user-attachments/assets/b942c3bb-0153-4017-8457-68340e9b7a81)
   - Listas de Games
![List 1 Game](https://github.com/user-attachments/assets/f728a062-ddcc-4c5f-99c3-9dc0c5b42c82)
![List 2 Game](https://github.com/user-attachments/assets/a50250c6-c4fc-47c8-ba5c-ddb11cd12861)

---

📜 Licença

Este projeto foi desenvolvido de forma autoral, com base em estudos e práticas adquiridos ao longo da minha trajetória. A construção foi guiada por conceitos sólidos e orientações aprendidas em um curso que serviu como base para estruturar a aplicação.
