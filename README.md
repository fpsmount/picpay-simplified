## 📌 PicPay Simplificado

Este projeto foi desenvolvido como parte do desafio para a vaga de **Desenvolvedor Júnior** no PicPay.  
Trata-se de uma **API RESTful** que simula uma plataforma de pagamentos, permitindo transferências entre usuários e lojistas.  

---

## 🚀 Tecnologias Utilizadas
- ☕ **Java 17**
- 🌱 **Spring Boot**
- 🗄️ **Banco de Dados H2 (em memória)**
- 🛠️ **Maven**
- 🔗 **RESTful API**

---

## 🎯 Funcionalidades
✔️ Cadastro de usuários comuns e lojistas  
✔️ Transferência de valores entre usuários  
✔️ Restrições para lojistas (apenas recebem pagamentos)  
✔️ Validação de saldo antes da transferência  
✔️ Integração com serviço externo para autorização de transações  

---

## ⚡ Como Rodar o Projeto

### 📌 Pré-requisitos
- JDK 17+  
- Maven  

### ▶️ Executando o projeto  
1️⃣ Clone este repositório:  
   ```sh
   git clone https://github.com/fpsmount/picpay-simplified.git
   ```
2️⃣ Acesse o diretório do projeto:  
   ```sh
   cd picpay-simplified
   ```
3️⃣ Compile e execute o projeto com o Maven:  
   ```sh
   mvn spring-boot:run
   ```
4️⃣ A API estará disponível em:  
   ```sh
   http://localhost:8080
   ```

---

## 🗄️ Banco de Dados  

O projeto utiliza o **H2 Database** (banco em memória) para facilitar a execução sem configurações adicionais.  

- **Driver:** `org.h2.Driver`  
- **URL JDBC:** `jdbc:h2:mem:testdb`  
- **Usuário:** `sa`  
- **Senha:** *(vazio)*  

---

## 🔗 Endpoints Principais  

### 💰 Transferência entre usuários  
**POST /transfer**  
```json
{
  "value": 100.0,
  "sender": 4,
  "receiver": 15
}
```
Essa operação valida o saldo do usuário pagador, consulta um serviço externo de autorização e executa a transação caso seja aprovada.  

---

## 📌 Pontos de Melhoria  

🔹 Implementar **testes unitários** para validar as regras de negócio  
🔹 Melhorar o tratamento de erros e mensagens de resposta  
🔹 Utilizar um **banco de dados real** (PostgreSQL ou MySQL)  
🔹 Adicionar logs mais detalhados para facilitar o monitoramento  

---

## 📞 Contato  

📩 Caso tenha dúvidas ou sugestões, entre em contato pelo [LinkedIn](https://www.linkedin.com/in/dimitrimonteiro/).  

---

# 🌎 English Version  

## 📌 PicPay Simplified  

This project was developed as part of the **Junior Developer** challenge at PicPay.  
It is a **RESTful API** that simulates a payment platform, allowing money transfers between users and merchants.  

---

## 🚀 Technologies Used  
- ☕ **Java 17**  
- 🌱 **Spring Boot**  
- 🗄️ **H2 Database (in-memory)**  
- 🛠️ **Maven**  
- 🔗 **RESTful API**  

---

## 🎯 Features  
✔️ User and merchant registration  
✔️ Money transfers between users  
✔️ Merchants can only receive payments  
✔️ Balance validation before transactions  
✔️ Integration with an external authorization service  

---

## ⚡ How to Run the Project  

### 📌 Prerequisites  
- JDK 17+  
- Maven  

### ▶️ Running the Project  
1️⃣ Clone this repository:  
   ```sh
   git clone https://github.com/fpsmount/picpay-simplified.git
   ```
2️⃣ Navigate to the project directory:  
   ```sh
   cd picpay-simplified
   ```
3️⃣ Build and run the project using Maven:  
   ```sh
   mvn spring-boot:run
   ```
4️⃣ The API will be available at:  
   ```sh
   http://localhost:8080
   ```

---

## 🗄️ Database  

This project uses **H2 Database** (an in-memory database) to make execution easier without additional configuration.  

- **Driver:** `org.h2.Driver`  
- **JDBC URL:** `jdbc:h2:mem:testdb`  
- **User:** `sa`  
- **Password:** *(empty)*  

---

## 🔗 Main Endpoints  

### 💰 Money Transfer  
**POST /transfer**  
```json
{
  "value": 100.0,
  "sender": 4,
  "receiver": 15
}
```
This operation validates the sender's balance, calls an external authorization service, and processes the transaction if approved.  

---

## 📌 Possible Improvements  

🔹 Implement **unit tests** to validate business rules  
🔹 Improve error handling and response messages  
🔹 Use a **real database** (PostgreSQL or MySQL)  
🔹 Add detailed logs for better monitoring  

---

## 📞 Contact  

📩 Feel free to reach out via [LinkedIn](https://www.linkedin.com/in/dimitrimonteiro/) for any questions or suggestions.  
