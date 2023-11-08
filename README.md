# PDV Frente de Caixa
# 🧑‍🏫 Sobre
- O projeto "PDV Frente de Caixa" é uma API RESTful desenvolvida para atender as necessidades de um ponto de venda (PDV). Esta API disponibiliza um conjunto de 16 rotas (GET, PUT, POST, DELETE) que permitem aos usuários realizar a gestão de categorias, clientes, produtos, pedidos e usuários. Além disso, o projeto suporta o envio de imagens e emails.

- A API foi estruturada seguindo as melhores práticas de desenvolvimento e oferece funcionalidades como cadastro, edição, listagem e exclusão de registros em diferentes entidades. Além disso, ela permite a autenticação de usuários por meio de tokens de acesso e aplica validações para garantir a integridade dos dados.


- Portanto, o PDV Frente de Caixa é uma solução flexível e escalável que pode ser usada como base para o desenvolvimento de sistemas de PDV e controle de estoque. Sinta-se à vontade para explorar as rotas e recursos disponíveis nesta API e contribuir com o seu desenvolvimento e aprimoramento.

---
#  💁‍♂️ Instruções para Executar o Projeto

Este guia fornece instruções gerais para configurar e executar o projeto PDV. Certifique-se de adaptar as etapas conforme necessário para sua configuração específica.

### Pré-requisitos

- Node.js instalado
- Banco de Dados PostgreSQL configurado e acessível

### Configuração Inicial

1. Clone este repositório para o seu ambiente local.

2. Navegue até o diretório do projeto:

```bash
cd seu-diretorio-do-projeto
```
2. Instale as dependências usando o npm:

```bash
npm install ou npm i
```
3. Configure as variáveis de ambiente:
- Crie um arquivo .env na raiz do projeto e defina as variáveis necessárias. Consulte o arquivo .env.example para obter um exemplo das variáveis que podem ser necessárias, como credenciais do banco de dados, segredos para JWT, etc.

4. Execute as migrações do banco de dados para criar as tabelas:
- Arquivo: DB.sql

5. Popule o banco de dados com dados iniciais (se necessário):

### Executando o Projeto

Para iniciar o servidor:

```bash
npm run dev
```
O servidor estará em execução e pronto para aceitar solicitações.
___
# 🛣️ Rotas

### Usuários
- Cadastro de Usuário
    **POST /usuario**
    Cadastra um novo usuário no sistema.
- Login de Usuário
    **POST /login**
    Permite que um usuário cadastrado realize o login e recebe um token de autenticação.
- Detalhes do Perfil do Usuário
    **GET /usuario**
    Retorna os dados do perfil do usuário logado.
- Editar Perfil do Usuário
    **PUT /usuario**
    Permite ao usuário logado atualizar as informações do seu perfil.
### Categorias
- Listar Categorias
    **GET /categoria**
    Retorna a lista de categorias disponíveis.
### Produtos
- Cadastro de Produto
    **POST /produto**
    Permite ao usuário logado cadastrar um novo produto no sistema.
- Editar Dados do Produto
    **PUT /produto/:id**
    Permite ao usuário logado atualizar as informações de um produto cadastrado.
- Listar Produtos
    **GET /produto**
    Retorna a lista de produtos cadastrados. Pode filtrar por categoria.
- Detalhes do Produto
    **GET /produto/:id**
    Retorna os detalhes de um produto específico.
- Excluir Produto por ID
    **DELETE /produto/:id**
    Permite ao usuário logado excluir um produto específico.
    
### Clientes
- Cadastro de Cliente
    **POST /cliente**
    Permite ao usuário logado cadastrar um novo cliente no sistema.
- Editar Dados do Cliente
    **PUT /cliente/:id**
    Permite ao usuário atualizar as informações de um cliente cadastrado.
- Listar Clientes
    **GET /cliente**
    Retorna a lista de clientes cadastrados.
- Detalhes do Cliente
    **GET /cliente/:id**
    Retorna os detalhes de um cliente específico.

### Pedidos
- Cadastro de Pedido
    **POST /pedido**
    Permite cadastrar um novo pedido no sistema, com produtos vinculados.
- Listar Pedidos
    **GET /pedido**
    Retorna a lista de pedidos cadastrados. Pode filtrar por cliente.

---
### 👨‍💻 Tecnologias:
- **Linguagem:** JavaScript | NODE.JS
- **Banco De Dados:** PostgreSQL
- **Bibliotecas:** express - aws-sdk - bcrypt - cors - cpf - dotenv - handlebars - joi - jsonwebtoken - knex - multer - nodemailer - pg
- **Deploys e envio de email:** elephant - ciclic - sendGrid - balckblaze
---
## 📧 Contato 
- Email: everton.junio132@gmail.com
- Linkedin: https://www.linkedin.com/in/everton-junio-dev
