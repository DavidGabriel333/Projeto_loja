Sistema de Loja de Suplementos

 Descrição do Projeto

Este projeto consiste em um sistema completo de gerenciamento de uma loja de suplementos, desenvolvido em **Java** com integração a banco de dados **PostgreSQL**.

O sistema simula um ambiente real de e-commerce, permitindo:

* Cadastro e gerenciamento de produtos
* Controle de estoque
* Realização de pedidos
* Cálculo automático de valores
* Separação de acesso entre cliente e gerente

 Tecnologias Utilizadas

Java (Swing) - Interface gráfica
PostgreSQL - Banco de dados
JDBC - Conexão com banco
Maven - Gerenciamento de dependências

 Tipos de Usuário (Login)

O sistema possui dois tipos de acesso:

 Cliente

* Visualiza produtos
* Adiciona ao carrinho
* Escolhe quantidade
* Finaliza pedidos
* Visualiza valor total da compra

Gerente

* Cadastra produtos
* Define preço e estoque
* Exclui produtos
* Visualiza vendas realizadas
* Acompanha faturamento total

Dados de Login 

Você pode inserir manualmente no banco ou usar:


INSERT INTO cliente(nome, email, senha)
VALUES ('Cliente', 'cliente@email.com', '123');


 Login Cliente:

 Email: cliente@email.com
 Senha: 123

 Login Gerente:
Email: admin@email.com
 Senha: 123

 Banco de Dados

O sistema utiliza as seguintes tabelas:

cliente
produto
pedido
item_pedido

Relacionamentos:

Cliente - Pedido (1:N)
Pedido - Item_Pedido (1:N)
 Produto - Item_Pedido (1:N)

## 👨‍💻 Autor

Desenvolvido por: David Gabriel

 Conclusão

Este projeto demonstra a construção de um sistema completo, integrando:

* Interface gráfica
* Banco de dados relacional
* Regras de negócio reais

Servindo como base para aplicações maiores e mais complexas.
