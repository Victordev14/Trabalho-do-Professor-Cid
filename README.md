# Projeto de Banco de Dados — Modelagem Conceitual

## 1. Caracterização da Organização
*(vale 7,5% — Dimensão Conceitual)*

- **Nome e natureza da organização:** O DER representa uma ótica/comércio de produtos ópticos, com processos de atendimento, vendas, pagamentos, receitas, produtos, fornecedores e compras. O nome específico da organização não está informado no DER.
- **Contexto e porte:** O modelo representa uma operação comercial que realiza atendimentos a clientes, registra receitas, realiza vendas, recebe pagamentos, mantém produtos em estoque, possui fornecedores e realiza compras.
- **Problemas e necessidades identificados:** O DER demonstra a necessidade de organizar e controlar informações relacionadas a clientes, atendimentos, funcionários, receitas, vendas, pagamentos, produtos, fornecedores e compras.
- **Justificativa da escolha:** A organização apresenta diversos processos relacionados entre si, permitindo a aplicação de um banco de dados para centralizar informações de clientes, atendimentos, vendas, produtos, fornecedores, pagamentos e compras.
- **Evidências da organização:** O DER fornecido comprova a existência de uma estrutura de dados voltada para uma operação de ótica/comércio óptico. Nome, endereço, telefone, site, responsável e demais evidências físicas da organização devem ser preenchidos pelo grupo com os dados reais obtidos na pesquisa de campo.

---

## 2. Processos de Negócio
*(vale 10% — Dimensão Procedimental)*

### Principais processos mapeados

- Cadastro e controle de clientes;
- Registro de atendimentos;
- Associação do atendimento a um funcionário;
- Geração de receitas;
- Realização de vendas;
- Registro de pagamentos;
- Controle de produtos;
- Relação entre produtos e fornecedores;
- Registro de compras;
- Atendimento de compras por fornecedores;
- Controle da quantidade disponível dos produtos.

### Fluxos principais

```text
Atendimento → Funcionário → Receita/Venda → Pagamento → Produto

Fornecedor → Compra

Fornecedor ↔ Produto
