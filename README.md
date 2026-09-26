## 1. Caracterização da Organização
*(vale 7,5% — Dimensão Conceitual)*

- **Nome e natureza da organização:** A organização representada pelo DER é uma **ótica**, caracterizada como uma empresa comercial que trabalha com atendimento de clientes, realização de exames, ajustes, vendas de produtos ópticos, receitas, pagamentos, compras e fornecedores.

- **Contexto e porte:** A organização possui uma operação voltada ao atendimento de clientes e à comercialização de produtos ópticos. O sistema contempla funcionários responsáveis pelos atendimentos, clientes, produtos, fornecedores, vendas, pagamentos, receitas e compras.

- **Problemas e necessidades identificados:** A organização necessita de um sistema capaz de organizar e centralizar as informações relacionadas aos clientes, atendimentos, funcionários, receitas, vendas, pagamentos, produtos, fornecedores e compras. O controle dessas informações permite melhorar a organização dos dados e facilitar o acompanhamento das operações realizadas.

- **Justificativa da escolha:** A organização foi escolhida por apresentar diversos processos que podem ser representados por meio de um banco de dados. O funcionamento envolve diferentes entidades e relacionamentos, como clientes realizando atendimentos, funcionários realizando atendimentos, atendimentos gerando receitas e vendas, vendas recebendo pagamentos, produtos sendo relacionados às vendas e fornecedores relacionados a produtos e compras.

- **Evidências da organização:** O DER desenvolvido apresenta a estrutura de informações e processos relacionados à organização. As informações específicas como nome oficial da organização, endereço completo, telefone, e-mail, responsável e links de redes sociais ou Google Maps devem ser preenchidas pelo grupo de acordo com os dados obtidos durante a pesquisa de campo.


---

## 2. Processos de Negócio
*(vale 10% — Dimensão Procedimental)*

- **Principais processos mapeados:** Os principais processos identificados no funcionamento da organização são o cadastro de clientes, registro de atendimentos, cadastro e controle de funcionários, registro de exames, vendas e ajustes, geração de receitas, realização de vendas, registro de pagamentos, cadastro e controle de produtos, controle da quantidade disponível dos produtos, cadastro de fornecedores, relação entre fornecedores e produtos e registro e controle de compras.

- **Processo de atendimento:** O cliente realiza um atendimento na organização. O atendimento possui informações como tipo, data, hora e observação e está relacionado a um funcionário responsável.

- **Processo de receita:** Um atendimento pode gerar uma receita. A receita possui informações como ID da receita, altura, DP, grau e data.

- **Processo de venda:** O cliente realiza uma venda. A venda possui informações como ID da venda, número da nota, valor total, data e prazo de garantia.

- **Processo de pagamento:** A venda recebe o pagamento. O pagamento registra informações como ID do pagamento, forma de pagamento, número de parcelas e valor.

- **Processo de produtos:** A venda possui produtos. Cada produto possui informações próprias, como tipo, referência, marca, modelo, tipo de montagem, tratamento, medida, grau, bloco, índice e quantidade disponível.

- **Processo de fornecedores:** Os fornecedores estão relacionados aos produtos comercializados pela organização. O fornecedor possui informações como localização, telefone, CNPJ, nome e ID de fornecimento.

- **Processo de compras:** O fornecedor atende às compras realizadas pela organização. Cada compra possui ID da compra, data da compra, valor total, status da compra e tipo da compra.

- **Fluxo geral dos processos:** O funcionamento geral pode ser representado pela sequência de atendimento do cliente, realização do atendimento, participação do funcionário, geração de receita ou venda, registro do pagamento, utilização dos produtos e relacionamento com fornecedores e compras.


---

## 3. Requisitos do Sistema
*(esta seção e a Seção 4 "Regras de Negócio" DIVIDEM 7,5% na dimensão conceitual — juntas valem 7,5%, não 7,5% cada — + 4% exclusivos desta seção na organização/documentação)*

### 3.1 Requisitos Funcionais

- **Cadastro de clientes:** O sistema deve permitir cadastrar e consultar os dados dos clientes, incluindo CPF, ID do cliente, endereço, nome e data de nascimento.

- **Registro de atendimentos:** O sistema deve permitir registrar e consultar os atendimentos realizados, armazenando tipo, data, hora e observações.

- **Relacionamento com funcionários:** O sistema deve permitir relacionar cada atendimento ao funcionário responsável e manter os dados dos funcionários, como ID, função, nome, telefone e data de emissão.

- **Registro de receitas:** O sistema deve permitir registrar receitas relacionadas aos atendimentos, armazenando informações como ID da receita, altura, DP, grau e data.

- **Registro de vendas:** O sistema deve permitir registrar vendas realizadas pelos clientes, contendo ID da venda, número da nota, valor total, data e prazo de garantia.

- **Registro de pagamentos:** O sistema deve permitir registrar os pagamentos relacionados às vendas, incluindo forma de pagamento, número de parcelas e valor.

- **Cadastro de produtos:** O sistema deve permitir cadastrar e consultar produtos, armazenando tipo, referência, marca, modelo, tipo de montagem, tratamento, medida, grau, bloco, índice e quantidade disponível.

- **Cadastro de fornecedores:** O sistema deve permitir cadastrar e consultar fornecedores, armazenando localização, telefone, CNPJ, nome e ID de fornecimento.

- **Registro de compras:** O sistema deve permitir registrar compras realizadas junto aos fornecedores, contendo ID da compra, data, valor total, status e tipo da compra.

### 3.2 Requisitos Não Funcionais

- **Segurança:** O sistema deve proteger as informações armazenadas e restringir o acesso conforme as permissões definidas.

- **Integridade:** Os dados cadastrados devem permanecer consistentes entre as entidades e seus respectivos relacionamentos.

- **Usabilidade:** O sistema deve apresentar as informações de forma organizada, clara e compreensível para os usuários.

- **Desempenho:** O sistema deve realizar consultas, registros e atualizações de forma eficiente.

- **Escalabilidade:** O sistema deve permitir o crescimento da quantidade de clientes, produtos, vendas, compras e demais registros.

- **Disponibilidade:** As informações devem estar disponíveis quando forem necessárias para a realização das atividades da organização.


---

## 4. Regras de Negócio
*(esta seção DIVIDE com a Seção 3 "Requisitos do Sistema" os mesmos 7,5% da dimensão conceitual — juntas valem 7,5%, não 7,5% cada — + 4% exclusivos desta seção na documentação)*

- **Relacionamento entre cliente e atendimento:** Todo atendimento deve estar relacionado a um cliente cadastrado no sistema.

- **Responsabilidade pelo atendimento:** Todo atendimento deve estar relacionado a um funcionário responsável.

- **Geração de receita:** Um atendimento pode gerar uma receita contendo as informações referentes ao exame ou prescrição.

- **Geração de venda:** Um atendimento pode gerar uma venda para o cliente.

- **Relacionamento da venda:** Toda venda deve estar relacionada a um cliente.

- **Pagamento da venda:** Toda venda deve possuir informações referentes ao seu pagamento.

- **Produtos da venda:** Uma venda pode possuir produtos comercializados pela organização.

- **Controle de produtos:** Todo produto deve possuir um identificador próprio e informações referentes à sua quantidade disponível.

- **Relacionamento com fornecedores:** Um fornecedor pode fornecer diferentes produtos e um produto pode estar relacionado a diferentes fornecedores.

- **Registro de compras:** Uma compra deve estar relacionada a um fornecedor e possuir informações sobre data, valor total, status e tipo.

- **Identificação dos registros:** As entidades devem possuir identificadores para permitir a diferenciação dos registros.

- **Integridade dos dados:** Os relacionamentos e cardinalidades definidos no DER devem ser respeitados durante a implementação do banco de dados.


---

## 5. Dicionário de Dados Conceitual (Preliminar)
*(vale 10% — Dimensão Procedimental - Segue o modelo do arquivo 02-03g_Exemplo_Dicionario_Dados.pdf)*

Para cada entidade identificada, foram definidos os atributos necessários para representar as informações da organização e as respectivas regras de negócio.

### CLIENTE

| Atributo | Descrição | Regra de negócio associada |
|----------|-----------|------------------------------|
| `cpf` | CPF utilizado para identificação do cliente | Deve identificar o cliente |
| `id_cliente` | Identificador único do cliente | Chave primária |
| `endereço` | Endereço do cliente | Informação cadastral |
| `nome` | Nome do cliente | Informação cadastral |
| `data_nasc` | Data de nascimento do cliente | Informação cadastral |

### ATENDIMENTO

| Atributo | Descrição | Regra de negócio associada |
|----------|-----------|------------------------------|
| `id_atendimento` | Identificador do atendimento | Chave primária |
| `tipo` | Tipo de atendimento realizado | Informação do atendimento |
| `data` | Data em que ocorreu o atendimento | Informação obrigatória |
| `hora` | Horário do atendimento | Informação do atendimento |
| `observação` | Observações relacionadas ao atendimento | Informação complementar |

### FUNCIONARIO

| Atributo | Descrição | Regra de negócio associada |
|----------|-----------|------------------------------|
| `id_funcionario` | Identificador do funcionário | Chave primária |
| `função` | Função exercida pelo funcionário | Informação funcional |
| `nome` | Nome do funcionário | Informação cadastral |
| `telefone` | Telefone do funcionário | Informação cadastral |
| `data_emissão` | Data de emissão registrada | Informação cadastral |

### RECEITA

| Atributo | Descrição | Regra de negócio associada |
|----------|-----------|------------------------------|
| `id_receita` | Identificador da receita | Chave primária |
| `altura` | Informação de altura registrada na receita | Informação da receita |
| `dp` | Informação de DP registrada na receita | Informação da receita |
| `grau` | Grau registrado na receita | Informação da receita |
| `data` | Data da receita | Informação da receita |

### VENDA

| Atributo | Descrição | Regra de negócio associada |
|----------|-----------|------------------------------|
| `id_venda` | Identificador da venda | Chave primária |
| `numero_nota` | Número da nota fiscal da venda | Identificação da venda |
| `valor_total` | Valor total da venda | Informação financeira |
| `data` | Data da venda | Informação da venda |
| `prazo_garantia` | Prazo de garantia da venda | Informação de garantia |

### PAGAMENTO

| Atributo | Descrição | Regra de negócio associada |
|----------|-----------|------------------------------|
| `id_pagamento` | Identificador do pagamento | Chave primária |
| `forma` | Forma utilizada para realizar o pagamento | Informação do pagamento |
| `num_parcelas` | Número de parcelas do pagamento | Informação do pagamento |
| `valor` | Valor do pagamento | Informação financeira |

### PRODUTO

| Atributo | Descrição | Regra de negócio associada |
|----------|-----------|------------------------------|
| `id_produto` | Identificador do produto | Chave primária |
| `tipo` | Tipo do produto | Classificação do produto |
| `referencia` | Referência do produto | Identificação do produto |
| `marca` | Marca do produto | Informação do produto |
| `modelo` | Modelo do produto | Informação do produto |
| `tipo_montagem` | Tipo de montagem | Característica do produto |
| `tratamento` | Tratamento do produto | Característica do produto |
| `medida` | Medida do produto | Característica do produto |
| `grau` | Grau do produto | Característica do produto |
| `bloco` | Bloco do produto | Característica do produto |
| `indice` | Índice do produto | Característica do produto |
| `quantidade_disponivel` | Quantidade disponível do produto | Controle de estoque |

### FORNECEDOR

| Atributo | Descrição | Regra de negócio associada |
|----------|-----------|------------------------------|
| `localização` | Localização do fornecedor | Informação cadastral |
| `telefone` | Telefone do fornecedor | Informação cadastral |
| `cnpj` | CNPJ do fornecedor | Identificação do fornecedor |
| `nome` | Nome do fornecedor | Informação cadastral |
| `id_fornecimento` | Identificador do fornecimento | Identificação do registro |

### COMPRA

| Atributo | Descrição | Regra de negócio associada |
|----------|-----------|------------------------------|
| `id_compra` | Identificador da compra | Chave primária |
| `data_compra` | Data em que a compra foi realizada | Informação da compra |
| `valor_total` | Valor total da compra | Informação financeira |
| `status_compra` | Situação atual da compra | Controle do status |
| `tipo_compra` | Tipo da compra | Classificação da compra |


---

## 6. Modelagem Conceitual (Entidades, Atributos, Relacionamentos)
*(vale 7,5% na dimensão conceitual)*

- **Entidades reconhecidas:** As principais entidades identificadas no DER são CLIENTE, ATENDIMENTO, FUNCIONARIO, RECEITA, VENDA, PAGAMENTO, PRODUTO, FORNECEDOR e COMPRA. Cada uma representa uma parte específica dos processos realizados pela organização.

- **CLIENTE:** Representa as pessoas que utilizam os serviços e realizam compras na organização.

- **ATENDIMENTO:** Representa os atendimentos realizados aos clientes.

- **FUNCIONARIO:** Representa os funcionários responsáveis pelos atendimentos e atividades da organização.

- **RECEITA:** Representa as receitas geradas a partir dos atendimentos realizados.

- **VENDA:** Representa as vendas realizadas para os clientes.

- **PAGAMENTO:** Representa os pagamentos relacionados às vendas.

- **PRODUTO:** Representa os produtos comercializados e controlados pela organização.

- **FORNECEDOR:** Representa as empresas ou responsáveis pelo fornecimento dos produtos.

- **COMPRA:** Representa as compras realizadas pela organização junto aos fornecedores.

- **Atributos e classificações:** Cada entidade possui atributos específicos responsáveis por armazenar suas informações. Os atributos identificadores, como `id_cliente`, `id_atendimento`, `id_funcionario`, `id_receita`, `id_venda`, `id_pagamento`, `id_produto` e `id_compra`, permitem identificar individualmente os registros.

- **Relacionamentos pertinentes:** As entidades estão relacionadas de acordo com os processos da organização. O cliente realiza atendimentos e vendas, os atendimentos estão relacionados aos funcionários e podem gerar receitas e vendas, as vendas recebem pagamentos e possuem produtos, enquanto fornecedores estão relacionados aos produtos e às compras.

- **Restrições e políticas organizacionais aplicadas ao modelo:** As cardinalidades e relacionamentos representados no DER devem ser respeitados na implementação do banco de dados para garantir a integridade das informações.


---

## 7. Diagrama Entidade-Relacionamento (DER)
*(vale 20% — é o item de maior peso da entrega)*

<img width="1243" height="948" alt="image" src="https://github.com/user-attachments/assets/453b1735-33d7-462a-ba8c-4c2915e364dc" />


## 8. Justificativa Técnica
*(vale 7,5% — sozinho, é o subcritério de maior peso dentro da Dimensão Conceitual)*

- **Escolha das entidades:** As entidades foram definidas a partir dos principais elementos envolvidos nos processos da organização. A separação entre clientes, atendimentos, funcionários, receitas, vendas, pagamentos, produtos, fornecedores e compras permite representar cada conjunto de informações de maneira organizada.

- **Escolha dos atributos:** Os atributos foram definidos de acordo com as informações necessárias para identificar e descrever cada entidade. Os identificadores foram utilizados para diferenciar os registros e facilitar os relacionamentos entre as entidades.

- **Escolha dos relacionamentos:** Os relacionamentos representam as operações realizadas pela organização. Dessa forma, é possível acompanhar desde o atendimento do cliente até processos relacionados a receitas, vendas, pagamentos, produtos, fornecedores e compras.

- **Escolha das cardinalidades:** As cardinalidades foram utilizadas para representar a quantidade de registros que podem participar de cada relacionamento, mantendo a estrutura compatível com os processos representados no DER.

- **Organização do modelo:** A divisão das informações em diferentes entidades evita a concentração de dados em uma única estrutura e facilita a futura implementação do banco de dados.

- **Escalabilidade:** A estrutura conceitual permite que o sistema seja ampliado posteriormente com novos clientes, funcionários, produtos, vendas, compras e demais registros.


---

## 9. Uso de Inteligência Artificial
*(documentação obrigatória — não é opcional se o grupo usou IA em qualquer etapa: pesquisa, escrita, organização de ideias ou revisão de texto)*

- **Ferramenta e etapa:** Foi utilizada a ferramenta **ChatGPT** na etapa de organização e documentação do projeto a partir das informações presentes no DER.

- **Motivação:** A ferramenta foi utilizada para auxiliar na organização das informações do DER dentro do esqueleto fornecido pelo professor, mantendo a ordem e o formato solicitado.

- **Prompt(s) utilizados:** O grupo solicitou que as informações do DER fossem colocadas no esqueleto fornecido, mantendo o formato, a ordem e a estrutura apresentados no roteiro.

- **Resposta recebida:** A IA organizou as informações identificadas no DER nas seções do projeto, incluindo caracterização da organização, processos de negócio, requisitos, regras de negócio, dicionário de dados, modelagem conceitual, DER e justificativa técnica.

- **Fontes consultadas e verificadas:** O DER fornecido pelo grupo foi utilizado como principal referência para identificar as entidades, atributos e relacionamentos.

- **Trechos rejeitados ou corrigidos:** Informações que não estavam presentes no DER, como nome oficial da organização, endereço, telefone, responsável e demais evidências da pesquisa de campo, devem ser verificadas e preenchidas pelo grupo.

- **Justificativa da escolha final:** O conteúdo foi mantido e organizado com base nas informações disponíveis no DER e na estrutura apresentada pelo professor.

- **Reflexão crítica:** A IA foi utilizada como ferramenta de apoio à organização e documentação. As informações específicas da organização devem ser verificadas pelo grupo por meio da pesquisa de campo, evitando a utilização de informações inventadas ou não confirmadas.


---

## Critérios Atitudinais (20%)

- **Participação (5%):** Envolvimento nas discussões técnicas e nas decisões realizadas pelo grupo durante o desenvolvimento do projeto.

- **Comprometimento (5%):** Cumprimento dos prazos e das responsabilidades assumidas pelos integrantes do grupo.

- **Colaboração (5%):** Cooperação entre os integrantes, respeito às contribuições dos colegas e participação equilibrada no desenvolvimento do projeto e no histórico de commits do GitHub.

- **Autonomia (5%):** Busca independente por soluções, participação nas decisões e proposta de melhorias para o projeto.


---

## Resumo dos Pesos

| Dimensão | Peso total |
|----------|-----------|
| Conceitual (contexto, requisitos/regras, modelagem, justificativa técnica) | 30% |
| Procedimental (requisitos, fluxogramas, dicionário de dados, DER) | 50% |
| Atitudinal (participação, comprometimento, colaboração, autonomia) | 20% |
