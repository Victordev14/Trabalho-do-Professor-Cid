Projeto de Banco de Dados — Modelagem Conceitual

1. Caracterização da Organização

(vale 7,5% — Dimensão Conceitual)

Nome e natureza da organização: A organização representada pelo DER é uma ótica, caracterizada como uma empresa comercial que trabalha com atendimento de clientes, realização de exames, ajustes, vendas de produtos ópticos, receitas, pagamentos, compras e fornecedores.

Contexto e porte: A organização possui uma operação voltada ao atendimento de clientes e à comercialização de produtos ópticos. O sistema contempla funcionários responsáveis pelos atendimentos, clientes, produtos, fornecedores, vendas, pagamentos, receitas e compras.

Problemas e necessidades identificados: A organização necessita de um sistema capaz de organizar e centralizar as informações relacionadas aos clientes, atendimentos, funcionários, receitas, vendas, pagamentos, produtos, fornecedores e compras. O controle dessas informações permite melhorar a organização dos dados e facilitar o acompanhamento das operações realizadas.

Justificativa da escolha: A organização foi escolhida por apresentar diversos processos que podem ser representados por meio de um banco de dados. O funcionamento envolve diferentes entidades e relacionamentos, como clientes realizando atendimentos, funcionários realizando atendimentos, atendimentos gerando receitas e vendas, vendas recebendo pagamentos, produtos sendo relacionados às vendas e fornecedores relacionados a produtos e compras.

Evidências da organização: O DER desenvolvido apresenta a estrutura de informações e processos relacionados à organização. As informações específicas como nome oficial da organização, endereço completo, telefone, e-mail, responsável e links de redes sociais ou Google Maps devem ser preenchidas pelo grupo de acordo com os dados obtidos durante a pesquisa de campo.

2. Processos de Negócio

(vale 10% — Dimensão Procedimental)

Principais processos mapeados: Os principais processos identificados no funcionamento da organização são:

Cadastro de clientes;

Registro de atendimentos;

Cadastro e controle de funcionários;

Registro de exames, vendas e ajustes;

Geração de receitas;

Realização de vendas;

Registro de pagamentos;

Cadastro e controle de produtos;

Controle da quantidade disponível dos produtos;

Cadastro de fornecedores;

Relação entre fornecedores e produtos;

Registro de compras;

Controle das informações das compras.

Processo de atendimento: O cliente realiza um atendimento na organização. O atendimento possui informações como tipo, data, hora e observação e está relacionado a um funcionário responsável.

Processo de receita: Um atendimento pode gerar uma receita. A receita possui informações como ID da receita, altura, DP, grau e data.

Processo de venda: O cliente realiza uma venda. A venda possui informações como ID da venda, número da nota, valor total, data e prazo de garantia.

Processo de pagamento: A venda recebe o pagamento. O pagamento registra informações como ID do pagamento, forma de pagamento, número de parcelas e valor.

Processo de produtos: A venda possui produtos. Cada produto possui informações próprias, como tipo, referência, marca, modelo, tipo de montagem, tratamento, medida, grau, bloco, índice e quantidade disponível.

Processo de fornecedores: Os fornecedores estão relacionados aos produtos comercializados pela organização. O fornecedor possui informações como localização, telefone, CNPJ, nome e ID de fornecimento.

Processo de compras: O fornecedor atende às compras realizadas pela organização. Cada compra possui ID da compra, data da compra, valor total, status da compra e tipo da compra.

Fluxo geral dos processos:

CLIENTE
   ↓
ATENDIMENTO
   ↓
FUNCIONÁRIO
   ↓
RECEITA / VENDA
   ↓
PAGAMENTO
   ↓
PRODUTO
   ↓
FORNECEDOR
   ↓
COMPRA

3. Requisitos do Sistema

(esta seção e a Seção 4 "Regras de Negócio" DIVIDEM 7,5% na dimensão conceitual — juntas valem 7,5%, não 7,5% cada — + 4% exclusivos desta seção na organização/documentação)

3.1 Requisitos Funcionais

O sistema deve:

Permitir cadastrar clientes.

Permitir consultar os dados dos clientes.

Permitir registrar CPF, ID do cliente, endereço, nome e data de nascimento.

Permitir registrar atendimentos.

Permitir consultar os atendimentos realizados.

Permitir registrar o tipo do atendimento.

Permitir registrar data, hora e observação do atendimento.

Permitir relacionar o atendimento ao cliente.

Permitir relacionar o atendimento ao funcionário responsável.

Permitir cadastrar funcionários.

Permitir consultar funcionários.

Permitir registrar ID, função, nome, telefone e data de emissão do funcionário.

Permitir registrar receitas.

Permitir relacionar uma receita ao atendimento.

Permitir registrar altura, DP, grau e data da receita.

Permitir cadastrar vendas.

Permitir relacionar a venda ao cliente.

Permitir registrar número da nota, valor total, data e prazo de garantia.

Permitir registrar pagamentos.

Permitir relacionar pagamentos às vendas.

Permitir registrar forma de pagamento, número de parcelas e valor.

Permitir cadastrar produtos.

Permitir consultar produtos.

Permitir registrar as características dos produtos.

Permitir controlar a quantidade disponível dos produtos.

Permitir cadastrar fornecedores.

Permitir consultar fornecedores.

Permitir registrar localização, telefone, CNPJ, nome e ID de fornecimento.

Permitir registrar compras.

Permitir relacionar compras aos fornecedores.

Permitir registrar data, valor total, status e tipo da compra.

Permitir relacionar produtos aos fornecedores.

3.2 Requisitos Não Funcionais

Segurança: o sistema deve proteger as informações armazenadas e restringir o acesso conforme as permissões definidas.

Integridade: os dados cadastrados devem permanecer consistentes entre as entidades e relacionamentos.

Usabilidade: o sistema deve apresentar as informações de maneira organizada e compreensível.

Desempenho: o sistema deve realizar consultas e registros de maneira eficiente.

Escalabilidade: o sistema deve permitir o crescimento da quantidade de clientes, produtos, vendas, compras e demais registros.

Disponibilidade: os dados devem estar disponíveis quando forem necessários para a realização dos processos da organização.

4. Regras de Negócio

(esta seção DIVIDE com a Seção 3 "Requisitos do Sistema" os mesmos 7,5% da dimensão conceitual — juntas valem 7,5%, não 7,5% cada — + 4% exclusivos desta seção na documentação)

Regras operacionais:

Todo atendimento deve estar relacionado a um cliente.

Todo atendimento deve estar relacionado a um funcionário.

Um atendimento pode gerar uma receita.

Um atendimento pode gerar uma venda.

Uma venda deve estar relacionada a um cliente.

Uma venda deve receber pagamento.

Uma venda pode possuir produtos.

Todo produto deve possuir um identificador próprio.

O produto deve possuir controle de quantidade disponível.

Um fornecedor pode fornecer diferentes produtos.

Um produto pode estar relacionado a diferentes fornecedores.

Um fornecedor pode atender diferentes compras.

Uma compra deve estar relacionada a um fornecedor.

Toda compra deve possuir data, valor total, status e tipo.

Os registros devem possuir identificadores para permitir sua diferenciação.

Restrições organizacionais:

Os identificadores devem ser utilizados para evitar registros duplicados dentro das entidades.

As cardinalidades definidas no DER devem ser respeitadas na implementação do banco de dados.

Os dados dos clientes, funcionários e fornecedores devem ser armazenados de maneira organizada.

A quantidade disponível dos produtos deve permitir o controle do estoque.

Os dados de venda devem estar relacionados aos respectivos pagamentos e produtos.

Os dados de compra devem estar relacionados aos respectivos fornecedores.

5. Dicionário de Dados Conceitual (Preliminar)

(vale 10% — Dimensão Procedimental - Segue o modelo do arquivo 02-03g_Exemplo_Dicionario_Dados.pdf)

Para cada entidade identificada:

CLIENTE

Atributo

Descrição

Regra de negócio associada

cpf

CPF utilizado para identificação do cliente

Deve identificar o cliente

id_cliente

Identificador único do cliente

Chave primária

endereço

Endereço do cliente

Informação cadastral

nome

Nome do cliente

Informação cadastral

data_nasc

Data de nascimento do cliente

Informação cadastral

ATENDIMENTO

Atributo

Descrição

Regra de negócio associada

id_atendimento

Identificador do atendimento

Chave primária

tipo

Tipo de atendimento realizado

Exame, venda ou ajuste

data

Data em que ocorreu o atendimento

Informação obrigatória do atendimento

hora

Horário do atendimento

Informação do atendimento

observação

Observações relacionadas ao atendimento

Informação complementar

FUNCIONARIO

Atributo

Descrição

Regra de negócio associada

id_funcionario

Identificador do funcionário

Chave primária

função

Função exercida pelo funcionário

Informação funcional

nome

Nome do funcionário

Informação cadastral

telefone

Telefone do funcionário

Informação cadastral

data_emissão

Data de emissão registrada

Informação cadastral

RECEITA

Atributo

Descrição

Regra de negócio associada

id_receita

Identificador da receita

Chave primária

altura

Informação de altura registrada na receita

Informação da receita

dp

Informação de DP registrada na receita

Informação da receita

grau

Grau registrado na receita

Informação da receita

data

Data da receita

Informação da receita

VENDA

Atributo

Descrição

Regra de negócio associada

id_venda

Identificador da venda

Chave primária

numero_nota

Número da nota fiscal da venda

Identificação da venda

valor_total

Valor total da venda

Informação financeira

data

Data da venda

Informação da venda

prazo_garantia

Prazo de garantia da venda

Informação de garantia

PAGAMENTO

Atributo

Descrição

Regra de negócio associada

id_pagamento

Identificador do pagamento

Chave primária

forma

Forma utilizada para realizar o pagamento

Dinheiro, PIX, débito ou crédito

num_parcelas

Número de parcelas do pagamento

Informação do pagamento

valor

Valor do pagamento

Informação financeira

PRODUTO

Atributo

Descrição

Regra de negócio associada

id_produto

Identificador do produto

Chave primária

tipo

Tipo do produto

Classificação do produto

referencia

Referência do produto

Identificação do produto

marca

Marca do produto

Informação do produto

modelo

Modelo do produto

Informação do produto

tipo_montagem

Tipo de montagem

Característica do produto

tratamento

Tratamento do produto

Característica do produto

medida

Medida do produto

Característica do produto

grau

Grau do produto

Característica do produto

bloco

Bloco do produto

Característica do produto

indice

Índice do produto

Característica do produto

quantidade_disponivel

Quantidade disponível do produto

Controle de estoque

FORNECEDOR

Atributo

Descrição

Regra de negócio associada

localização

Localização do fornecedor

Informação cadastral

telefone

Telefone do fornecedor

Informação cadastral

cnpj

CNPJ do fornecedor

Identificação do fornecedor

nome

Nome do fornecedor

Informação cadastral

id_fornecimento

Identificador do fornecimento

Identificação do registro

COMPRA

Atributo

Descrição

Regra de negócio associada

id_compra

Identificador da compra

Chave primária

data_compra

Data em que a compra foi realizada

Informação da compra

valor_total

Valor total da compra

Informação financeira

status_compra

Situação atual da compra

Controle do status

tipo_compra

Tipo da compra

Classificação da compra

6. Modelagem Conceitual (Entidades, Atributos, Relacionamentos)

(vale 7,5% na dimensão conceitual)

Entidades reconhecidas:

CLIENTE: representa os clientes atendidos pela organização.

ATENDIMENTO: representa os atendimentos realizados.

FUNCIONARIO: representa os funcionários responsáveis pelos atendimentos.

RECEITA: representa as receitas geradas nos atendimentos.

VENDA: representa as vendas realizadas.

PAGAMENTO: representa os pagamentos das vendas.

PRODUTO: representa os produtos comercializados.

FORNECEDOR: representa os fornecedores dos produtos.

COMPRA: representa as compras realizadas junto aos fornecedores.

Atributos e classificações:

Cada entidade possui seus próprios atributos para representar as informações necessárias ao funcionamento da organização. Os atributos identificadores, como id_cliente, id_atendimento, id_funcionario, id_receita, id_venda, id_pagamento, id_produto e id_compra, são utilizados para identificar os registros.

Relacionamentos pertinentes:

CLIENTE REALIZA ATENDIMENTO.

ATENDIMENTO REALIZA com FUNCIONARIO.

ATENDIMENTO GERA RECEITA.

ATENDIMENTO GERA VENDA.

CLIENTE REALIZA VENDA.

VENDA RECEBE PAGAMENTO.

VENDA POSSUI PRODUTO.

PRODUTO FORNECE FORNECEDOR.

FORNECEDOR ATENDE COMPRA.

Restrições e políticas organizacionais aplicadas ao modelo:

As cardinalidades apresentadas no DER devem ser respeitadas na implementação do banco de dados. Os relacionamentos representam as operações existentes entre clientes, atendimentos, funcionários, receitas, vendas, pagamentos, produtos, fornecedores e compras.

7. Diagrama Entidade-Relacionamento (DER)

(vale 20% — é o item de maior peso da entrega)

Anexe o DER (em imagem).

O DER apresenta as seguintes entidades:

CLIENTE

ATENDIMENTO

FUNCIONARIO

RECEITA

VENDA

PAGAMENTO

PRODUTO

FORNECEDOR

COMPRA

Os relacionamentos representados são:

CLIENTE — REALIZA — ATENDIMENTO

ATENDIMENTO — REALIZA — FUNCIONARIO

ATENDIMENTO — GERA — RECEITA

ATENDIMENTO — GERA — VENDA

CLIENTE — REALIZA — VENDA

VENDA — RECEBE — PAGAMENTO

VENDA — POSSUI — PRODUTO

PRODUTO — FORNECE — FORNECEDOR

FORNECEDOR — ATENDE — COMPRA

O modelo utiliza cardinalidades para representar a participação mínima e máxima das entidades em cada relacionamento.

O DER foi estruturado de forma a permitir uma futura implementação do banco de dados e possibilitar a expansão do sistema conforme o crescimento da organização.

8. Justificativa Técnica

(vale 7,5% — sozinho, é o subcritério de maior peso dentro da Dimensão Conceitual)

A modelagem conceitual foi desenvolvida com o objetivo de representar os principais processos da organização de maneira organizada e estruturada.

As entidades CLIENTE, ATENDIMENTO, FUNCIONARIO, RECEITA, VENDA, PAGAMENTO, PRODUTO, FORNECEDOR e COMPRA foram separadas porque representam diferentes elementos envolvidos no funcionamento da organização.

A entidade CLIENTE permite armazenar as informações cadastrais dos clientes. A entidade ATENDIMENTO registra as informações relacionadas aos atendimentos realizados, enquanto FUNCIONARIO permite identificar os funcionários envolvidos nesses atendimentos.

A entidade RECEITA foi separada para armazenar as informações específicas das receitas geradas a partir dos atendimentos.

A entidade VENDA representa a operação comercial e possui informações próprias, como número da nota, valor total, data e prazo de garantia.

A entidade PAGAMENTO foi separada da venda para permitir o armazenamento das informações financeiras relacionadas ao pagamento, como forma, número de parcelas e valor.

A entidade PRODUTO permite armazenar as características dos produtos comercializados e controlar a quantidade disponível.

A entidade FORNECEDOR representa os fornecedores e armazena suas informações cadastrais. A entidade COMPRA representa as operações de compra realizadas junto dos fornecedores.

Os relacionamentos foram definidos para representar como as entidades participam dos processos da organização. As cardinalidades demonstram a quantidade mínima e máxima de ocorrências permitidas em cada relacionamento.

A estrutura criada permite que o modelo seja posteriormente utilizado como base para a criação do modelo lógico e implementação do banco de dados.

9. Uso de Inteligência Artificial

(documentação obrigatória — não é opcional se o grupo usou IA em qualquer etapa: pesquisa, escrita, organização de ideias ou revisão de texto)

Item

O que registrar

Ferramenta e etapa

ChatGPT — utilizado na etapa de organização e documentação do projeto a partir do DER.

Motivação

A ferramenta foi utilizada para organizar as informações presentes no DER dentro do esqueleto fornecido pelo professor, mantendo a ordem e o formato solicitado.

Prompt(s) utilizados

“PEGA AS INFORMAÇÕES DO DER E COLOCA NO ESQUELETO NÃO MUDA O FORMATO SEGUE A ORDEM E O JEITO QUE TE MANDEI.”

Resposta recebida

A IA organizou as informações do DER nas seções do projeto, incluindo caracterização da organização, processos de negócio, requisitos, regras de negócio, dicionário de dados, modelagem conceitual, DER e justificativa técnica.

Fontes consultadas e verificadas

O DER fornecido pelo grupo foi utilizado como principal fonte para identificar as entidades, atributos e relacionamentos.

Trechos rejeitados ou corrigidos

Informações que não estavam presentes no DER, como nome oficial da organização, endereço, telefone, responsável e outras evidências da pesquisa de campo, não foram inventadas e devem ser preenchidas pelo grupo.

Justificativa da escolha final

O conteúdo foi organizado com base nas informações identificadas no DER e seguindo a estrutura apresentada no roteiro do trabalho.

Reflexão crítica

A IA foi utilizada como ferramenta de apoio à organização e documentação. As informações específicas da organização precisam ser verificadas e validadas pelo grupo por meio da pesquisa de campo.

Critérios Atitudinais (20%)

Estes critérios são avaliados por meio da participação dos integrantes do grupo durante o desenvolvimento do projeto:

Participação (5%): envolvimento nas discussões técnicas e decisões do grupo.

Comprometimento (5%): cumprimento dos prazos e responsabilidades assumidas.

Colaboração (5%): cooperação entre os integrantes e participação equilibrada no desenvolvimento do projeto e nos commits do GitHub.

Autonomia (5%): busca independente de soluções e proposta de melhorias para o projeto.

Resumo dos Pesos

Dimensão

Peso total

Conceitual (contexto, requisitos/regras, modelagem, justificativa técnica)

30%

Procedimental (requisitos, fluxogramas, dicionário de dados, DER)

50%

Atitudinal (participação, comprometimento, colaboração, autonomia)

20%
