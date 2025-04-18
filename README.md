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

![Image](https://github.com/user-attachments/assets/b1458cc7-81f3-476e-b952-144984957a93)

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

![Image](https://github.com/user-attachments/assets/47b0503d-e145-414b-8173-5d6fa576238d)

---

![Image](https://github.com/user-attachments/assets/28161cea-84ec-4c4d-ae74-b9edd5293651)

---

![Image](https://github.com/user-attachments/assets/2515e591-4db4-4ac7-b8f1-5ddf45dba3ac)

---

![Image](https://github.com/user-attachments/assets/d58d2656-8fca-42dd-8975-6928b1407ad8)

---

![Image](https://github.com/user-attachments/assets/5dad5645-b897-4458-9809-c3ad25a8b109)

---

![Image](https://github.com/user-attachments/assets/1c918fa0-4af9-4c34-9c1f-9b7ac9f2128c)

---

![Image](https://github.com/user-attachments/assets/84089056-fac2-42e3-a2b1-8851a198a1ea)
