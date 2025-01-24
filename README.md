# 🎮 Projeto DSList - Intensivão Java Spring 🚀

## Sobre o projeto
O DSList é uma aplicação backend para gerenciamento de uma lista de jogos, desenvolvida como parte do Intensivão Java Spring. O projeto utiliza tecnologias modernas como Spring Boot, JPA/Hibernate e SQL para criar uma API RESTful funcional e escalável.

A ideia central é permitir que os usuários organizem seus jogos em listas personalizadas, podendo criar, visualizar e atualizar com a organização baseada em rankings.

## 🗂️ Modelo de Domínio
O modelo de domínio da aplicação é representado no diagrama abaixo, que detalha as entidades principais do sistema:
- 🎮 **Game:** Representa os jogos cadastrados.
- 📋 **GameList:** Representa listas personalizadas de jogos criadas pelos usuários.
- 🔗 **Belonging:** Representa a relação entre jogos e listas, armazenando informações adicionais como a posição do jogo na lista.

![Modelo de domínio DSList](https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/dslist-model.png)

## 🛠️ Tecnologias utilizadas
- ☕ **Java 21**
- 🌱 **Spring Boot 3**
- 🗃️ **JPA / Hibernate**
- 🧩 **Maven**
- 🗄️ **Banco de dados H2 (em memória)**
- 🐳 **PostgreSQL** (local em homologação utilizando Docker e em nuvem para simular um ambiente de produção)
- 📫 **Postman** (para testes de API)

## 📡 Endpoints principais
A aplicação expõe os seguintes endpoints RESTful:

- **GET /games:** Lista todos os jogos.
- **GET /games/{id}:** Busca detalhes de um jogo específico.
- **GET /lists:** Lista todas as listas de jogos.
- **GET /lists/{id}/games:** Lista os jogos pertencentes a uma lista.
- **POST /lists/{idList}/replacement:** Atualiza a ordem dos jogos em uma lista específica.

## 🚀 Como executar o projeto
1. Clone o repositório:
   ```bash
   git clone https://github.com/MarcoTamassia01/dslist.git
   ```

2. Navegue até a pasta do projeto:
   ```bash
   cd dslist
   ```

3. Execute o projeto em sua IDE ou com o Maven:
   ```bash
   mvn spring-boot:run
   ```

4. Acesse o banco de dados H2 pelo navegador, caso necessário:
   ```
   http://localhost:8080/h2-console
   ```

5. Utilize uma ferramenta como Postman para testar os endpoints da API.

## 💡 Agradecimento especial
Um agradecimento especial ao professor Nélio Alves pelo conhecimento compartilhado e pela excelente abordagem didática durante o desenvolvimento das aulas! 🙌🎓  
