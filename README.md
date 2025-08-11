# 🍔 Hamburgueria XTudo - Sistema de Pedidos

Sistema desenvolvido em **Progress OpenEdge/ABL** para gerenciamento de pedidos, clientes, produtos e cidades, com foco em integridade referencial e facilidade de uso.

## 📋 Funcionalidades

- **Cadastro de Cidades**
  - Inclusão, alteração e exclusão com validação de vínculos (não permite excluir cidade com clientes vinculados).
  
- **Cadastro de Clientes**
  - Inclusão, alteração e exclusão.
  - Validação de vínculos (bloqueio de exclusão se houver pedidos) ou exclusão em cascata (opcional).
  
- **Cadastro de Produtos**
  - Inclusão, alteração e exclusão.
  - Bloqueio de exclusão se o produto estiver vinculado a itens de pedidos.
  
- **Pedidos**
  - Inclusão, alteração e exclusão de pedidos.
  - Adição e remoção de itens do pedido.
  - Recalcula automaticamente o valor total do pedido.
  - Bloqueio de exclusão se houver vínculos, com opção de exclusão em cascata para itens.
  
- **Navegação Fácil**
  - Botões para ir ao primeiro, anterior, próximo e último registro.
  - Botões para adicionar, modificar, eliminar, salvar, cancelar e exportar.
  
## 🛡️ Validações Implementadas

- **Integridade Referencial** manual em código:
  - Cidade ↔ Clientes
  - Cliente ↔ Pedidos
  - Produto ↔ Itens
- Bloqueio de exclusão de registros com vínculos.
- Validação de campos obrigatórios (cliente, produto, data).
- Mensagens amigáveis de erro para o usuário.

## 🖼️ Telas Principais

- **Cadastro de Cidades**
- **Cadastro de Clientes**
- **Cadastro de Produtos**
- **Pedidos com Itens**

> As telas foram desenvolvidas com interface simples e objetiva, permitindo uso rápido em ambiente de produção.

## ⚙️ Tecnologias Utilizadas

- **Linguagem:** Progress OpenEdge/ABL
- **Banco de Dados:** Progress
- **Interface:** Frames e Browses nativos ABL

## 🚀 Como Executar

1. Abra o projeto no **Progress Developer Studio** ou no editor ABL.
2. Compile todos os arquivos `.p`.
3. Execute o programa principal (menu ou módulo desejado).
4. Utilize os botões de navegação e CRUD conforme necessário.

## 🧩 Estrutura de Arquivos

