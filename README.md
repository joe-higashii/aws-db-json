# **Projeto: Banco de Dados Simulado com JSON Server**

## **Descrição**
Este projeto consiste em:
- Modelagem de um banco de dados no [dbdiagram.io](https://dbdiagram.io).
- Conversão do modelo para JSON com dados mockados.
- Configuração de uma API Fake utilizando o `json-server`.
- Publicação do projeto no GitHub com a imagem do diagrama incluída no README.

A API fake permite simular operações CRUD (Create, Read, Update, Delete) nos dados mockados.

---

## **Diagrama do Banco de Dados**
Abaixo está o diagrama do banco de dados modelado:

![Image](https://github.com/user-attachments/assets/a124e53e-d381-41c7-8fb4-7c61b5c013e0)

---

## **Tecnologias Utilizadas**
- [dbdiagram.io](https://dbdiagram.io) para modelagem do banco de dados.
- [Node.js](https://nodejs.org/) e [JSON Server](https://github.com/typicode/json-server) para simulação da API.
- Git e GitHub para versionamento e compartilhamento do projeto.

---

## **Como Configurar e Executar o Projeto**

### **Pré-requisitos**
Certifique-se de ter as seguintes ferramentas instaladas em sua máquina:
- Node.js (versão 16 ou superior)
- npm (gerenciador de pacotes do Node.js)

### **Passo a Passo**

1. **Clone o repositório**
   No terminal, execute:
   ```bash
   git clone 
   cd 
   ```

2. **Instale o JSON Server**
   Caso ainda não tenha o `json-server` instalado, execute:
   ```bash
   npm install -g json-server
   ```

3. **Inicie o servidor**
   Execute o comando abaixo para iniciar a API Fake:
   ```bash
   json-server --watch db.json
   ```
   O servidor será iniciado em `http://localhost:3000`.

4. **Acesse os endpoints no navegador ou via ferramentas como Postman**
   Exemplos de endpoints disponíveis:
   - Listar todos os usuários:
     ```
     http://localhost:3000/users
     ```
   - Listar todos os produtos:
     ```
     http://localhost:3000/products
     ```
   - Listar pedidos:
     ```
     http://localhost:3000/orders
     ```

---

## **Testando no Navegador**

1. Após iniciar o servidor com `json-server --watch db.json`, abra seu navegador.
2. Acesse os seguintes links para visualizar os dados mockados:
   - Usuários: [http://localhost:3000/users](http://localhost:3000/users)
   - Produtos: [http://localhost:3000/products](http://localhost:3000/products)
   - Pedidos: [http://localhost:3000/orders](http://localhost:3000/orders)

3. Você também pode usar ferramentas como [Postman](https://www.postman.com/) ou [Insomnia](https://insomnia.rest/) para testar requisições GET, POST, PUT e DELETE nos endpoints.

---

## **Estrutura do Projeto**

```
aws-db-json/
│
├── db.json          # Arquivo JSON com os dados mockados
├── diagram.png      # Imagem do diagrama do banco de dados
├── README.md        # Documentação do projeto
```

---

## **Exemplo de Dados Mockados (`db.json`)**

```json
{
  "users": [
    { "id": 1, "name": "Alice", "email": "alice@example.com", "password": "123456" },
    { "id": 2, "name": "Bob", "email": "bob@example.com", "password": "abcdef" }
  ],
  "products": [
    { "id": 1, "name": "Laptop", "price": 1500 },
    { "id": 2, "name": "Mouse", "price": 50 }
  ],
  "orders": [
    { "id": 1, "user_id": 1, "order_date": "2025-04-01T10:00:00" }
  ],
  "order_items": [
    { "id": 1, "order_id": 1, "product_id": 1, "quantity": 1 },
    { "id": 2, "order_id": 1, "product_id": 2, "quantity": 2 }
  ]
}
```

---

## **Contribuição**
Sinta-se à vontade para contribuir com melhorias neste projeto. Basta abrir um pull request ou relatar problemas na aba Issues.

---

## **Licença**
Este projeto é apenas para fins educacionais e não possui uma licença específica.

## **Screenshots**

![Image](https://github.com/user-attachments/assets/0428ec3f-fcb7-4ffc-a37e-d28a7655ceb1)

---
![Image](https://github.com/user-attachments/assets/0dd69420-4fd9-4c29-bbf8-9c558f7aa04a)

---
![Image](https://github.com/user-attachments/assets/b129a178-ef9c-4abc-a146-c30bfbf861ce)

---
![Image](https://github.com/user-attachments/assets/84ec5e67-2f99-4ea1-b5d6-80d4757ff7bf)

---
![Image](https://github.com/user-attachments/assets/cfd08ad6-fe0a-4e8c-88b8-66973f8098cb)

---
![Image](https://github.com/user-attachments/assets/eccf6992-0b22-4802-a1a8-6d272b466c54)

---
![Image](https://github.com/user-attachments/assets/9121cdfb-d868-471c-97ee-3a0baab8b6d6)