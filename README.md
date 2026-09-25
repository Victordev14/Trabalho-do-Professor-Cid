1. Caracterização da Organização

(vale 7,5% — Dimensão Conceitual)

Nome e natureza da organização: A organização escolhida é a Ótica Kadosh, do segmento óptico.

Contexto e porte: A Ótica Kadosh possui 3 pessoas trabalhando. Segundo as informações levantadas na entrevista, são atendidos aproximadamente 50 clientes por semana. Também foram informados aproximadamente 200 vendas e 400 atendimentos no período mencionado durante a entrevista. Entre as atividades e produtos mencionados estão exame de vista, lentes, armações, óculos de sol, lentes de contato, laboratório e montagem.

Problemas e necessidades identificados: Os registros de informações são realizados em papel, o que pode ocasionar informações incorretas e rasuras. O controle dos produtos que estão faltando também é realizado manualmente, por meio de contagem. Foi identificada a necessidade de voltar a utilizar um sistema e possuir um banco de dados para organizar as informações.

Justificativa da escolha: A Ótica Kadosh foi escolhida por apresentar diferentes processos relacionados ao atendimento de clientes, receitas, produtos, vendas, pagamentos, controle de produtos, fornecedores, compras e acompanhamento de serviços, possibilitando a aplicação dos conceitos de modelagem conceitual de dados.

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

RF17 — O sistema deve permitir registrar itens das compras e acompanhar o status da compra.

RF18 — O sistema deve permitir registrar e acompanhar ordens de serviço, incluindo status, previsão e entrega.

RF19 — O sistema deve permitir consultar as vendas realizadas por cada funcionário.

3.2 Requisitos Não Funcionais

RNF01 — O sistema deve possuir uma interface simples e de fácil utilização.

RNF02 — O sistema deve proteger as informações pessoais dos clientes.

RNF03 — O sistema deve permitir acesso rápido às informações cadastradas.

RNF04 — O sistema deve possuir controle de acesso às informações administrativas.

RNF05 — O sistema deve manter os dados organizados e estruturados.

RNF06 — O sistema deve reduzir a dependência dos registros realizados em papel.

4. Regras de Negócio

(esta seção DIVIDE com a Seção 3 "Requisitos do Sistema" os mesmos 7,5% da dimensão conceitual — juntas valem 7,5%, não 7,5% cada — + 4% exclusivos desta seção na documentação. "Regras de negócio" é o termo técnico usado em modelagem de dados para as regras de funcionamento de qualquer organização, com ou sem fins lucrativos)

Regras operacionais: Um cliente pode possuir mais de uma receita; cada receita registra grau, DNP e altura; um atendimento pode ou não gerar uma receita; todo atendimento pertence a um cliente e é realizado por um funcionário; uma venda pertence a um cliente e é efetuada por um funcionário; uma venda contém um ou mais itens; uma venda pode receber um ou mais pagamentos; uma venda pode ser acompanhada por uma ordem de serviço; uma receita pode estar relacionada a itens de venda; cada item de venda referencia um produto; um fornecedor pode fornecer vários produtos; uma compra deve estar relacionada a um fornecedor e conter um ou mais itens; cada item de compra referencia um produto; os produtos possuem quantidade disponível controlada; uma venda pode utilizar cartão de crédito, PIX ou dinheiro, podendo combinar formas de pagamento e utilizar parcelamento; existe garantia de 1 ano.

Restrições organizacionais: Parte dos registros é realizada em papel, podendo ocorrer rasuras e informações incorretas. O controle dos produtos faltantes também é realizado manualmente por contagem. A organização identificou a necessidade de voltar a utilizar um sistema e possuir um banco de dados para organizar e consultar suas informações.

5. Dicionário de Dados Conceitual (Preliminar)

(vale 10% — Dimensão Procedimental)

O dicionário abaixo foi ajustado para corresponder aos elementos que aparecem no DER fornecido.

Cliente

Atributo

Descrição

Regra de negócio associada

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

Atributo

Descrição

Regra de negócio associada

id_atendimento

Identificador conceitual do atendimento

Utilizado para identificar o atendimento no modelo

tipo

Tipo do atendimento

Pode representar exame, venda ou ajuste, conforme indicado no DER

observacao

Observação do atendimento

Registra observações relacionadas ao atendimento

data_hora

Data e hora do atendimento

Registra quando o atendimento ocorreu

Receita

Atributo

Descrição

Regra de negócio associada

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

Atributo

Descrição

Regra de negócio associada

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

Atributo

Descrição

Regra de negócio associada

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

Atributo

Descrição

Regra de negócio associada

id_pagamento

Identificador conceitual do pagamento

Utilizado para identificar o pagamento no modelo

forma

Forma de pagamento

Pode representar dinheiro, PIX, débito ou crédito, conforme indicado no DER

num_parcelas

Número de parcelas

Registra o parcelamento do pagamento

valor

Valor do pagamento

Registra o valor pago

Produto

Atributo

Descrição

Regra de negócio associada

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

Atributo

Descrição

Regra de negócio associada

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

Atributo

Descrição

Regra de negócio associada

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

Observação: não foram incluídas as entidades Item_Venda, Item_Compra e Ordem_Servico, nem atributos que não aparecem no DER fornecido. O dicionário deve permanecer limitado ao que está efetivamente representado no diagrama.

6. Modelagem Conceitual (Entidades, Atributos, Relacionamentos)

(vale 7,5% na dimensão conceitual)

Entidades reconhecidas

Cliente, Atendimento, Receita, Funcionário, Venda, Pagamento, Produto, Fornecedor e Compra.

Atributos

Cliente: id_cliente, cpf, endereco, nome, data_nasc.

Atendimento: id_atendimento, tipo, observacao, data_hora.

Receita: id_receita, altura, dnp, grau, data.

Funcionário: id_funcionario, telefone, funcao, nome, data_emissao.

Venda: id_venda, numero_nota, valor_total, data, prazo_garantia.

Pagamento: id_pagamento, forma, num_parcelas, valor.

Produto: id_produto, tipo, referencia, marca, material, tipo_montagem, tratamento, medida, grau, bloco, indice, quantidade_disponivel.

Fornecedor: id_fornecimento, localizacao, telefone, cnpj, nome.

Compra: id_compra, data_compra, valor_total, status_compra, tipo_compra.

Relacionamentos e cardinalidades

Cliente (0,n) — REALIZA — Atendimento (1,1).

Atendimento (1,1) — REALIZA — Funcionário (0,n).

Atendimento (0,1) — GERA — Receita (1,1).

Cliente (0,n) — REALIZA — Venda (1,1).

Atendimento (0,n) — GERA — Venda (1,n).

Venda (1,n) — RECEBE — Pagamento (1,1).

Venda (1,n) — POSSUI — Produto (1,1).

Produto (0,n) — FORNECE — Fornecedor (0,n).

Fornecedor (0,n) — ATENDE — Compra (1,1).

Observação de consistência

As entidades, atributos, relacionamentos e cardinalidades acima foram transcritos de acordo com o DER fornecido. Não foram acrescentadas entidades ou relacionamentos que não estejam representados no diagrama.

7. Diagrama Entidade-Relacionamento (DER)

(vale 20% — é o item de maior peso da entrega)



O diagrama representa corretamente:

Entidades

Atributos

Relacionamentos

Cardinalidades

O modelo deve ser consistente com as informações apresentadas neste README e com o DER anexado.

8. Justificativa Técnica

(vale 7,5% — sozinho, é o subcritério de maior peso dentro da Dimensão Conceitual)

A modelagem foi organizada a partir dos processos e informações levantados na Ótica Kadosh e representados no DER. A entidade Cliente concentra informações cadastrais e se relaciona com Atendimento e Venda, além de possuir relação com Receita por meio do modelo representado.

A entidade Atendimento registra o atendimento realizado e possui os atributos id_atendimento, tipo, observacao e data_hora. O atendimento se relaciona com Funcionário, Receita e Venda conforme as cardinalidades representadas no DER.

A entidade Funcionário possui os atributos apresentados no diagrama e participa do relacionamento REALIZA com Atendimento. Não foi acrescentada uma relação entre Funcionário e Venda, pois essa relação não aparece no DER fornecido.

A entidade Venda registra id_venda, numero_nota, valor_total, data e prazo_garantia. A venda se relaciona com Cliente, Atendimento, Pagamento e Produto, seguindo as cardinalidades apresentadas no diagrama.

A entidade Pagamento foi mantida separada de Venda e possui os atributos id_pagamento, forma, num_parcelas e valor. O relacionamento RECEBE representa a associação entre Venda e Pagamento conforme o DER.

A entidade Produto concentra suas características e a quantidade disponível. No DER fornecido, Produto se relaciona diretamente com Venda por meio de POSSUI e com Fornecedor por meio de FORNECE.

As entidades Fornecedor e Compra representam a parte relacionada aos fornecedores e às compras. Fornecedor possui relação ATENDE com Compra e relação FORNECE com Produto, conforme representado no diagrama.

Importante: não foram criadas ou descritas as entidades Item_Venda, Item_Compra e Ordem_Servico, pois elas não aparecem no DER fornecido.

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

As informações foram comparadas com as respostas obtidas na entrevista e com as observações realizadas durante a pesquisa de campo.

Trechos rejeitados ou corrigidos

Foram rejeitadas ou corrigidas informações que não estavam confirmadas na entrevista, além de atributos, entidades e relacionamentos que não estavam suficientemente sustentados pelo levantamento.

Justificativa da escolha final

O grupo utilizou a IA como ferramenta de apoio, mantendo a entrevista e a pesquisa de campo como base principal para as decisões do projeto.

Reflexão crítica

A IA pode interpretar incorretamente informações ambíguas ou sugerir elementos não levantados na pesquisa. Por isso, suas respostas foram analisadas criticamente e revisadas pelo grupo antes da utilização no projeto.

Se o grupo não usou nenhuma ferramenta de IA, declare isso explicitamente nesta seção.

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
