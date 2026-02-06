# Student Grade Manager 🎓

O **Student Grade Manager** é uma API minimalista construída para o gerenciamento de notas de alunos. Este projeto destaca-se por utilizar puramente o módulo nativo do Node.js para a criação do servidor e manipulação de rotas, sem a dependência de frameworks externos como o Express.

## 🚀 Tecnologias

Este projeto foi desenvolvido utilizando:
- **[Node.js](https://nodejs.org)**: Ambiente de execução JavaScript (configurado com ES Modules).
- **[UUID](https://www.npmjs.com)**: Utilizado para a geração de IDs únicos para cada registro de nota.
- **HTTP Native Module**: Utilizado para gerenciar requisições e respostas do servidor.

## 🛠️ Como Instalar e Rodar

1. **Clone o repositório:**
   git clone https://github.com

2. **Instale as dependências:**
   npm install

3. **Inicie o servidor:**
   node index.js

O servidor estará ativo em http://localhost:3000.

## 📌 Rotas da API

Abaixo estão os endpoints disponíveis para gerenciar as notas. Você pode utilizar ferramentas como [Postman](https://www.postman.com) ou [Insomnia](https://insomnia.rest) para realizar os testes.

| Método | Endpoint | Descrição |
| :--- | :--- | :--- |
| GET | /grades | Retorna a lista completa de notas. |
| POST | /grades | Cadastra uma nova nota no sistema. |
| PUT | /grades/:id | Atualiza os dados de uma nota específica via ID. |
| DELETE | /grades/:id | Remove permanentemente uma nota via ID. |

### Exemplo de Corpo da Requisição (JSON):
Para as operações de POST e PUT, utilize o seguinte formato no corpo da requisição:

{
  "studentName": "João Silva",
  "subject": "Matemática",
  "grade": 9.5
}

## 📂 Estrutura do Projeto

O projeto é focado em simplicidade, contendo apenas os arquivos essenciais:
- index.js: Contém toda a lógica do servidor, roteamento e armazenamento em memória.
- package.json: Manifesto do projeto com a dependência uuid e configurações de execução.

## 📝 Licença
Este projeto está licenciado sob a [ISC License](https://opensource.org).
