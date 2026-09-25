1. Caracterização da Organização

(vale 7,5% — Dimensão Conceitual)

Nome e natureza da organização: A organização escolhida é a Ótica Kadosh, do segmento óptico.

Contexto e porte: A Ótica Kadosh possui 3 pessoas trabalhando. Segundo as informações levantadas na entrevista, são atendidos aproximadamente 50 clientes por semana. Também foram informados aproximadamente 200 vendas e 400 atendimentos no período mencionado durante a entrevista. Entre as atividades e produtos mencionados estão exame de vista, lentes, armações, óculos de sol, lentes de contato, laboratório e montagem.

Problemas e necessidades identificados: Os registros de informações são realizados em papel, o que pode ocasionar informações incorretas e rasuras. O controle dos produtos que estão faltando também é realizado manualmente, por meio de contagem. Foi identificada a necessidade de voltar a utilizar um sistema e possuir um banco de dados para organizar as informações.

Justificativa da escolha: A Ótica Kadosh foi escolhida por apresentar diferentes processos relacionados ao atendimento de clientes, receitas, produtos, vendas, pagamentos, fornecedores e compras, possibilitando a aplicação dos conceitos de modelagem conceitual de dados.

Evidências da organização: A pesquisa foi realizada por meio de entrevista e pesquisa de campo na Ótica Kadosh. As fotos da visita serão adicionadas posteriormente pelo grupo como evidência.

2. Processos de Negócio

(vale 10% — Dimensão Procedimental)

Principais processos mapeados: Atendimento ao cliente; identificação da necessidade do cliente; verificação de receita; realização de exame de vista quando não há receita; preenchimento da ficha; elaboração de orçamento; apresentação das informações ao cliente; venda de produtos; realização do pagamento; contagem dos produtos em falta; realização de compras e pedidos; relação com fornecedores; acompanhamento da ordem de serviço; montagem e finalização.

Fluxogramas: Os fluxogramas dos processos-chave serão anexados ao repositório, representando visualmente os fluxos identificados durante a pesquisa de campo.

3. Requisitos do Sistema

(esta seção e a Seção 4 "Regras de Negócio" DIVIDEM 7,5% na dimensão conceitual — juntas valem 7,5%, não 7,5% cada — + 4% exclusivos desta seção na organização/documentação)

3.1 Requisitos Funcionais

RF01 — O sistema deve permitir cadastrar clientes.

RF02 — O sistema deve permitir registrar nome, CPF, endereço, CEP e número do endereço do cliente.

RF03 — O sistema deve permitir cadastrar receitas dos clientes.

RF04 — O sistema deve permitir registrar data, grau, DNP e altura relacionados à receita.

RF05 — O sistema deve permitir registrar os atendimentos realizados.

RF06 — O sistema deve permitir registrar a data e o tipo de atendimento.

RF07 — O sistema deve permitir registrar informações relacionadas ao exame de vista e às receitas geradas a partir do atendimento.

RF08 — O sistema deve permitir cadastrar produtos.

RF09 — O sistema deve permitir consultar os produtos cadastrados.

RF10 — O sistema deve permitir registrar e consultar a quantidade disponível dos produtos.

RF11 — O sistema deve permitir registrar vendas, incluindo data, valor, número da nota e prazo de garantia.

RF12 — O sistema deve permitir registrar os pagamentos realizados.

RF13 — O sistema deve permitir registrar mais de uma forma de pagamento em uma venda.

RF14 — O sistema deve permitir registrar pagamentos parcelados.

RF15 — O sistema deve permitir cadastrar fornecedores.

RF16 — O sistema deve permitir registrar compras realizadas com fornecedores.

RF17 — O sistema deve permitir registrar informações da compra, incluindo data, valor total, status e tipo da compra.

3.2 Requisitos Não Funcionais

RNF01 — O sistema deve possuir uma interface simples e de fácil utilização.

RNF02 — O sistema deve proteger as informações pessoais dos clientes.

RNF03 — O sistema deve permitir acesso rápido às informações cadastradas.

RNF04 — O sistema deve possuir controle de acesso às informações administrativas.

RNF05 — O sistema deve manter os dados organizados e estruturados.

RNF06 — O sistema deve reduzir a dependência dos registros realizados em papel.

4. Regras de Negócio

(esta seção DIVIDE com a Seção 3 "Requisitos do Sistema" os mesmos 7,5% da dimensão conceitual — juntas valem 7,5%, não 7,5% cada — + 4% exclusivos desta seção na documentação. "Regras de negócio" é o termo técnico usado em modelagem de dados para as regras de funcionamento de qualquer organização, com ou sem fins lucrativos)

Regras operacionais: Um cliente pode realizar vários atendimentos e várias vendas; todo atendimento está associado a um cliente e a um funcionário; um atendimento pode gerar uma receita e uma ou mais vendas; uma venda recebe um ou mais pagamentos; uma venda possui um ou mais produtos; um produto pode estar relacionado a vários fornecedores e um fornecedor pode estar relacionado a vários produtos; um fornecedor pode atender várias compras; cada compra está associada a um fornecedor; os produtos possuem quantidade disponível controlada; uma venda pode utilizar diferentes formas de pagamento e parcelamento; existe garantia de 1 ano.

Restrições organizacionais: Parte dos registros é realizada em papel, podendo ocorrer rasuras e informações incorretas. O controle dos produtos faltantes também é realizado manualmente por contagem. A organização identificou a necessidade de voltar a utilizar um sistema e possuir um banco de dados para organizar e consultar suas informações.

5. Dicionário de Dados Conceitual (Preliminar)

(vale 10% — Dimensão Procedimental - Segue o modelo do arquivo 02-03g_Exemplo_Dicionario_Dados.pdf)
Para cada entidade identificada, liste:

Cliente

AtributoDescriçãoRegra de negócio associada





id_cliente

Identificador conceitual do cliente

Utilizado para identificar o cliente no modelo

cpf

CPF do cliente

Informação cadastral

endereco

Endereço do cliente

Informação cadastral

nome

Nome do cliente

Informação cadastral

data_nasc

Data de nascimento do cliente

Informação cadastral

Atendimento

AtributoDescriçãoRegra de negócio associada





id_atendimento

Identificador conceitual do atendimento

Utilizado para identificar o atendimento no modelo

tipo

Tipo do atendimento

Informação registrada no atendimento

observacao

Observação do atendimento

Registra observações relacionadas ao atendimento

data_hora

Data e hora do atendimento

Registra quando o atendimento ocorreu

Receita

AtributoDescriçãoRegra de negócio associada





id_receita

Identificador conceitual da receita

Utilizado para identificar a receita no modelo

altura

Altura registrada na receita

Informação da receita

dnp

DNP registrada na receita

Informação da receita

grau

Grau registrado na receita

Informação da receita

data

Data da receita

Registra a data da receita

Funcionario

AtributoDescriçãoRegra de negócio associada





id_funcionario

Identificador conceitual do funcionário

Utilizado para identificar o funcionário no modelo

telefone

Telefone do funcionário

Informação cadastral

funcao

Função do funcionário

Informação funcional

nome

Nome do funcionário

Informação cadastral

data_emissao

Data de emissão registrada no modelo

Informação registrada no DER

Venda

AtributoDescriçãoRegra de negócio associada





id_venda

Identificador conceitual da venda

Utilizado para identificar a venda no modelo

numero_nota

Número da nota da venda

Informação da venda

valor_total

Valor total da venda

Deve ser registrado

data

Data da venda

Registra quando a venda ocorreu

prazo_garantia

Prazo de garantia da venda

Informação de garantia

Pagamento

AtributoDescriçãoRegra de negócio associada





id_pagamento

Identificador conceitual do pagamento

Utilizado para identificar o pagamento no modelo

forma

Forma de pagamento

Informação registrada no pagamento

num_parcelas

Número de parcelas

Registra o parcelamento do pagamento

valor

Valor do pagamento

Registra o valor pago

Produto

AtributoDescriçãoRegra de negócio associada





id_produto

Identificador conceitual do produto

Utilizado para identificar o produto no modelo

tipo

Tipo de produto

Informação do produto

referencia

Referência do produto

Informação utilizada para identificação

marca

Marca do produto

Informação do produto

material

Material do produto

Informação do produto

tipo_montagem

Tipo de montagem

Informação do produto

tratamento

Tratamento

Informação do produto

medida

Medida

Informação do produto

grau

Grau

Informação do produto

bloco

Bloco

Informação do produto

indice

Índice

Informação do produto

quantidade_disponivel

Quantidade disponível do produto

Registra a quantidade disponível

Fornecedor

AtributoDescriçãoRegra de negócio associada





id_fornecimento

Identificador conceitual do fornecedor

Utilizado para identificar o fornecedor no modelo

localizacao

Localização do fornecedor

Informação cadastral

telefone

Telefone do fornecedor

Informação cadastral

cnpj

CNPJ do fornecedor

Informação cadastral

nome

Nome do fornecedor

Informação cadastral

Compra

AtributoDescriçãoRegra de negócio associada





id_compra

Identificador conceitual da compra

Utilizado para identificar a compra no modelo

data_compra

Data da compra

Registra quando a compra ocorreu

valor_total

Valor total da compra

Informação da compra

status_compra

Status da compra

Permite registrar a situação da compra

tipo_compra

Tipo da compra

Informação da compra

Mantenha o dicionário organizado e padronizado (mesmo formato de tabela para todas as entidades).
Atenção à privacidade: se forem usados exemplos de valores para ilustrar os atributos, esses exemplos devem ser fictícios — não utilize dados reais de clientes, fiéis, beneficiários, doadores ou funcionários da organização (nomes, CPFs, contatos etc.), mesmo que tenham sido observados durante a pesquisa de campo. Os exemplos devem apenas ser coerentes com as operações reais observadas.

6. Modelagem Conceitual (Entidades, Atributos, Relacionamentos)

(vale 7,5% na dimensão conceitual)

Entidades reconhecidas: Cliente, Atendimento, Receita, Funcionário, Venda, Pagamento, Produto, Fornecedor e Compra. Essas entidades correspondem às entidades representadas no DER atualizado.

Atributos e classificações: Cliente possui id_cliente, CPF, endereço, nome e data de nascimento. Atendimento possui id_atendimento, tipo, observação e data/hora. Receita possui id_receita, altura, DNP, grau e data. Funcionário possui id_funcionario, telefone, função, nome e data de emissão. Venda possui id_venda, número da nota, valor total, data e prazo de garantia. Pagamento possui id_pagamento, forma, número de parcelas e valor. Produto possui id_produto, tipo, referência, marca, material, tipo de montagem, tratamento, medida, grau, bloco, índice e quantidade disponível. Fornecedor possui id_fornecimento, localização, telefone, CNPJ e nome. Compra possui id_compra, data da compra, valor total, status da compra e tipo da compra.

Relacionamentos pertinentes: Cliente REALIZA Atendimento e Venda. Atendimento se relaciona com Funcionário por REALIZA, com Receita por GERA e com Venda por GERA. Venda se relaciona com Pagamento por RECEBE e com Produto por POSSUI. Produto se relaciona com Fornecedor por FORNECE. Fornecedor se relaciona com Compra por ATENDE.

Restrições e políticas organizacionais aplicadas ao modelo: O modelo considera o uso de registros em papel, o controle manual dos produtos faltantes, a possibilidade de múltiplas receitas por cliente, as diferentes formas de pagamento, o parcelamento, o registro das compras com fornecedores e a garantia de 1 ano.

Cardinalidades representadas no DER

Cliente (0,n) — REALIZA — (1,1) Atendimento.

Atendimento (1,1) — REALIZA — (0,n) Funcionário.

Atendimento (0,1) — GERA — (1,1) Receita.

Cliente (0,n) — REALIZA — (1,1) Venda.

Atendimento (0,m) — GERA — (1,n) Venda.

Pagamento (1,1) — RECEBE — (1,n) Venda.

Venda (1,n) — POSSUI — (1,1) Produto.

Produto (0,n) — FORNECE — (0,n) Fornecedor.

Fornecedor (0,n) — ATENDE — (1,1) Compra.

7. Diagrama Entidade-Relacionamento (DER)

(vale 20% — é o item de maior peso da entrega)

Anexe o DER (em imagem).

O diagrama deve representar corretamente:

Entidades

Atributos

Relacionamentos

Cardinalidades

O modelo deve ser consistente e já demonstrar potencial de escalabilidade e integração (pensando nas próximas etapas do projeto).

8. Justificativa Técnica

(vale 7,5% — sozinho, é o subcritério de maior peso dentro da Dimensão Conceitual)

A modelagem foi organizada a partir dos processos e informações levantados na Ótica Kadosh e representados no DER atualizado. A entidade Cliente concentra as informações cadastrais e se relaciona com Atendimento e Venda.
A entidade Atendimento representa o registro do atendimento e se relaciona com Cliente, Funcionário, Receita e Venda, conforme representado no DER. A relação com Receita permite representar que um atendimento pode gerar uma receita, enquanto a relação com Venda representa a geração da venda a partir do atendimento.
A entidade Funcionário participa do relacionamento com Atendimento e possui os atributos representados no diagrama. A entidade Venda registra os dados da venda e se relaciona com Cliente, Atendimento, Pagamento e Produto.
A entidade Pagamento foi separada de Venda porque o modelo registra forma de pagamento, valor e parcelamento. A entidade Produto concentra as características dos produtos e sua quantidade disponível, além de se relacionar com Fornecedor.
As entidades Fornecedor e Compra representam os processos relacionados ao fornecimento e às compras. Fornecedor se relaciona com Produto por meio de FORNECE e com Compra por meio de ATENDE.
As cardinalidades foram mantidas exatamente conforme representadas no DER enviado, sem acrescentar entidades, atributos ou relacionamentos que não estejam presentes no diagrama.

9. Uso de Inteligência Artificial

(documentação obrigatória — não é opcional se o grupo usou IA em qualquer etapa: pesquisa, escrita, organização de ideias ou revisão de texto)
Se o grupo usou alguma ferramenta de IA (ChatGPT, Claude, Gemini, Perplexity etc.) em qualquer parte do trabalho, registre para cada uso relevante:

ItemO que registrar



Ferramenta e etapa

ChatGPT — utilizado na organização das informações da entrevista, elaboração e revisão dos requisitos, regras de negócio, dicionário de dados, modelagem conceitual e revisão do README.

Motivação

Auxiliar na organização das informações obtidas na entrevista e na estruturação e revisão da documentação da atividade.

Prompt(s) utilizados

Prompts solicitando a organização e revisão das informações da entrevista da Ótica Kadosh conforme a estrutura do modelo fornecido pelo professor.

Resposta recebida

A IA auxiliou na organização das informações da entrevista em caracterização da organização, processos, requisitos, regras de negócio, dicionário de dados e modelagem conceitual.

Fontes consultadas e verificadas

As informações foram comparadas com as respostas obtidas na entrevista, com as observações realizadas durante a pesquisa de campo e com o DER definido pelo grupo.

Trechos rejeitados ou corrigidos

Foram rejeitadas ou corrigidas informações que não estavam confirmadas na entrevista, além de entidades, atributos e relacionamentos que não estavam representados no DER.

Justificativa da escolha final

O grupo utilizou a IA como ferramenta de apoio, mantendo a entrevista, a pesquisa de campo e o DER como base para as decisões do projeto.

Reflexão crítica

A IA pode interpretar incorretamente informações ambíguas ou sugerir elementos não levantados na pesquisa. Por isso, suas respostas foram analisadas criticamente e revisadas pelo grupo antes da utilização no projeto.

Critérios Atitudinais (20%)

Estes critérios NÃO constam explicitamente como item de entrega no README. Eles são avaliados por meio de Avaliação 360º entre os integrantes do grupo (cada membro avalia os colegas de equipe) e, no caso da Colaboração, também pela colaboração equilibrada no histórico de commits do repositório GitHub — não pela leitura do restante do repositório nem pela apresentação:

Participação (5%): envolvimento nas discussões técnicas e nas decisões do grupo.

Comprometimento (5%): cumprimento de prazos e responsabilidades assumidas.

Colaboração (5%): respeito às contribuições dos colegas, cooperação na construção do projeto e colaboração equilibrada no histórico de commits do repositório GitHub.

Autonomia (5%): busca independente de soluções e proposta de melhorias.

Resumo dos Pesos

DimensãoPeso total



Conceitual (contexto, requisitos/regras, modelagem, justificativa técnica)

30%

Procedimental (requisitos, fluxogramas, dicionário de dados, DER)

50%

Atitudinal (participação, comprometimento, colaboração, autonomia)

20%
