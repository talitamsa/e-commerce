# Documentação da Aplicação de E-commerce

## Visão Geral

### Descrição do Projeto: 
A aplicação é um e-commerce que permite aos usuários comprar produtos eletrônicos. Ela incluirá recursos como registro de usuário, login, navegação de produtos, adição ao carrinho, checkout e rastreamento de pedidos.


# Tecnologias Utilizadas

### Backend:

1. Linguagem de programação: Java
2. Framework: Spring Boot
3. Banco de dados: H2 (para testes), MySQL (em produção)
4. Maven para gerenciamento de dependências

### Frontend:

1. Angular
2. Angular Material

### Arquitetura:
A aplicação segue uma arquitetura de três camadas com frontend, backend e banco de dados. O frontend se comunica com o backend por meio de uma API REST.

### Entidades do Banco de Dados:

Usuário:

Campos: ID, nome, email, senha
Exemplo de registro:

{
  "id": 1,
  "nome": "João",
  "email": "joao@email.com",
  "senha": "hashed_password"
}

Produto:

Campos: ID, nome, descrição, preço, quantidade em estoque
Exemplo de produto:

{
  "id": 1,
  "nome": "Smartphone",
  "descrição": "Um smartphone de última geração.",
  "preço": 599.99,
  "quantidade_estoque": 100
}

Pedido:

Campos: ID, ID do usuário, lista de itens do pedido, status do pedido
Exemplo de pedido:

{
  "id": 1,
  "id_usuario": 1,
  "itens_pedido": [
    {
      "produto_id": 1,
      "quantidade": 2
    }
  ],
  "status_pedido": "Em andamento"
}
