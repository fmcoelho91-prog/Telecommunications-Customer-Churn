# 📉 Telecommunications Customer Churn & Revenue Risk Analysis

## Resumo do Projeto

Este projeto foi desenvolvido com o objetivo de analisar o abandono de clientes, habitualmente designado por *customer churn*, numa empresa do setor das telecomunicações.

A análise foi realizada sobre uma base de dados com **7.043 clientes**, permitindo identificar os principais fatores associados ao churn, quantificar a faturação mensal relacionada com os clientes perdidos e determinar os grupos que devem receber maior prioridade nas estratégias de retenção.

O projeto combina uma Análise Exploratória de Dados em **Python** com um dashboard interativo desenvolvido em **Power BI**, orientado para a análise de clientes, proteção da receita e apoio à tomada de decisão.

---

#  Objetivos do Projeto

Os principais objetivos desta análise são:

* Calcular a taxa global de churn.
* Quantificar a faturação mensal associada aos clientes perdidos.
* Identificar os tipos de contrato com maior risco de abandono.
* Analisar a relação entre apoio técnico e retenção.
* Avaliar o comportamento dos clientes de acordo com o tempo de permanência.
* Comparar as taxas de churn entre diferentes métodos de pagamento.
* Segmentar os clientes de acordo com o valor da mensalidade.
* Identificar grupos que combinam elevado risco e elevado impacto financeiro.
* Desenvolver recomendações estratégicas orientadas para a retenção.

---

#  Questões de Negócio

O projeto procura responder às seguintes questões:

* Qual é a taxa global de churn da empresa?
* Qual é a faturação mensal associada aos clientes que abandonaram?
* Que tipos de contrato apresentam maior risco de churn?
* Qual é a relação entre apoio técnico e retenção de clientes?
* Em que fase da relação com a empresa ocorre maior abandono?
* Que métodos de pagamento apresentam taxas de churn mais elevadas?
* Que segmentos de valor apresentam maior risco financeiro?
* Que grupos devem ser prioritários nas campanhas de retenção?

---

#  Tecnologias Utilizadas

* Python
* Pandas
* Power BI
* Jupyter Notebook
* Google Colab

---

#  Processo de Análise

## 1. Auditoria Inicial dos Dados

Foi realizada uma avaliação inicial da estrutura e qualidade do dataset, incluindo:

* Verificação da dimensão da base de dados.
* Análise dos tipos de dados.
* Identificação de valores em falta.
* Verificação de registos duplicados.
* Verificação de identificadores de clientes repetidos.
* Análise das principais estatísticas descritivas.

## 2. Limpeza e Validação

O processo de limpeza incluiu:

* Tratamento dos valores em falta em `Total Charges`.
* Substituição dos valores não aplicáveis em `Churn Reason`.
* Validação das principais variáveis numéricas.
* Verificação das categorias utilizadas nas variáveis principais.
* Remoção de variáveis sintéticas criadas numa versão anterior da análise.

Após a limpeza, o dataset manteve os **7.043 clientes**, sem valores em falta ou registos duplicados.

## 3. Engenharia de Atributos

Foram criadas novas variáveis para apoiar a análise:

* `Churn_Numero`: transformação do churn numa variável numérica.
* `Grupo_Tenure`: agrupamento dos clientes por tempo de permanência.
* `Segmento_Valor`: segmentação dos clientes de acordo com o valor da mensalidade.

A segmentação por valor foi definida da seguinte forma:

* **Baixo Valor:** mensalidade inferior a 40 €.
* **Valor Médio:** mensalidade entre 40 € e 80 €.
* **Alto Valor:** mensalidade superior a 80 €.

Estes segmentos foram criados exclusivamente para fins analíticos e não representam planos comerciais reais da empresa.

## 4. Análise Exploratória

Foram analisadas as seguintes dimensões:

* Churn global.
* Impacto financeiro.
* Tipo de contrato.
* Apoio técnico.
* Tempo de permanência.
* Método de pagamento.
* Valor da mensalidade.
* Segmentação de clientes.

---

# 📊 Dashboard Interativo

Os resultados da análise foram apresentados num dashboard desenvolvido em **Power BI**, dividido em três páginas complementares.

## Executive Overview

Visão executiva dos principais indicadores de negócio, incluindo:

* Total de clientes.
* Clientes perdidos.
* Taxa global de churn.
* Receita mensal associada ao churn.
* Impacto anualizado estimado.
* Distribuição dos clientes por situação.

![Executive Overview](Dashboard%201.png)

---

## Customer Segmentation

Análise dos grupos com maior risco de abandono através do cruzamento de:

* Tipo de contrato.
* Apoio técnico.
* Método de pagamento.
* Tempo de permanência.
* Segmento de valor.

![Customer Segmentation](Dashboard%202.png)

---

## Financial Impact & Recommendations

Quantificação do impacto financeiro do churn e apresentação de recomendações estratégicas orientadas para a retenção de clientes e proteção da receita.

![Financial Impact and Recommendations](Dashboard%203.png)

---

#  Principais Descobertas

##  Taxa Global de Churn

A empresa apresenta uma taxa global de churn de **26,54%**.

Dos 7.043 clientes analisados:

* **5.174** permanecem ativos.
* **1.869** abandonaram o serviço.

Isto significa que aproximadamente um em cada quatro clientes presentes no dataset abandonou a empresa.

---

##  Impacto Financeiro

Os clientes que abandonaram representavam **139.130,85 € em faturação mensal**.

Este valor corresponde a um impacto anualizado estimado de aproximadamente **1,67 milhões de euros**, caso o nível de faturação mensal se mantivesse constante durante 12 meses.

O valor anualizado representa uma estimativa e não uma perda anual diretamente observada no dataset.

---

##  Tipo de Contrato

Os clientes com contratos `Month-to-month` apresentam a maior taxa de churn:

| Tipo de contrato | Taxa de churn |
| ---------------- | ------------: |
| Month-to-month   |        42,71% |
| One year         |        11,27% |
| Two year         |         2,83% |

Os contratos mensais concentram:

* **1.655 clientes perdidos**.
* **120.847,10 € de faturação mensal associada ao churn**.
* Aproximadamente **87% da faturação mensal perdida**.

Os clientes com contratos mensais representam, por isso, um dos principais grupos de risco.

---

##  Impacto do Apoio Técnico

A análise global demonstra que os clientes sem `Tech Support` apresentam uma taxa de churn superior à dos clientes com este serviço.

Para realizar uma comparação mais adequada, foram analisados separadamente os clientes com contratos `Month-to-month`.

Dentro deste grupo:

| Apoio técnico    | Taxa de churn |
| ---------------- | ------------: |
| Sem Tech Support |        50,37% |
| Com Tech Support |        30,70% |

A presença de apoio técnico está associada a uma redução de **19,67 pontos percentuais** na taxa de churn dos clientes com contratos mensais.

Esta relação representa uma associação e não permite concluir, isoladamente, que o apoio técnico seja a causa direta da redução do churn.

---

##  Tempo de Permanência

Os clientes que abandonaram apresentam um tempo médio e mediano de permanência inferior ao dos clientes ativos.

A análise por grupos demonstra que o churn é mais elevado durante as fases iniciais da relação com a empresa, sobretudo entre clientes com até 12 meses de permanência.

Este resultado sugere que o primeiro ano representa um período particularmente importante para:

* integração dos novos clientes;
* acompanhamento da experiência inicial;
* resolução de dificuldades técnicas;
* identificação de sinais de insatisfação.

---

##  Método de Pagamento

O método `Electronic check` apresenta a maior taxa de churn:

| Método de pagamento       | Taxa de churn |
| ------------------------- | ------------: |
| Electronic check          |        45,29% |
| Mailed check              |        19,11% |
| Bank transfer — automatic |        16,71% |
| Credit card — automatic   |        15,24% |

No grupo `Electronic check`, **1.071 dos 2.365 clientes** abandonaram o serviço.

Os métodos de pagamento automático apresentam as taxas de churn mais baixas.

Contudo, o método de pagamento deve ser interpretado em conjunto com outras variáveis, como o tipo de contrato e o tempo de permanência.

---

##  Segmentação por Valor

Os clientes foram agrupados de acordo com o valor da mensalidade.

| Segmento    | Taxa de churn | Clientes perdidos | Faturação mensal perdida |
| ----------- | ------------: | ----------------: | -----------------------: |
| Alto Valor  |        33,98% |               906 |              85.349,35 € |
| Valor Médio |        29,53% |               750 |              48.438,30 € |
| Baixo Valor |        11,59% |               213 |               5.343,20 € |

O segmento **Alto Valor**, composto por clientes com mensalidades superiores a 80 €, apresenta:

* a maior taxa de churn;
* o maior número de clientes perdidos;
* aproximadamente **61% da faturação mensal associada ao churn**.

Este grupo combina elevado risco de abandono com elevado impacto financeiro.

---

#  Recomendações Estratégicas

## 1. Priorizar Clientes com Contratos Mensais

Desenvolver campanhas de retenção dirigidas aos clientes com contratos `Month-to-month`.

Possíveis incentivos:

* descontos temporários;
* preços fixos durante o período contratual;
* serviços adicionais incluídos;
* benefícios de fidelização;
* condições especiais para migração para contratos anuais.

## 2. Reforçar o Apoio Técnico

Promover a adesão ao serviço de `Tech Support`, principalmente entre clientes com contratos mensais e menor tempo de permanência.

A empresa deve também facilitar o contacto com o apoio técnico e identificar rapidamente problemas de utilização ou insatisfação.

## 3. Melhorar o Acompanhamento Inicial

Reforçar o acompanhamento dos clientes durante os primeiros 12 meses através de:

* contactos após a adesão;
* questionários de satisfação;
* comunicações educativas;
* acompanhamento de problemas técnicos;
* ofertas personalizadas;
* contacto preventivo perante sinais de insatisfação.

## 4. Incentivar Métodos de Pagamento Automáticos

Facilitar e incentivar a adesão à transferência bancária automática ou ao pagamento automático por cartão.

Antes da implementação, deve ser analisada a relação entre o método de pagamento, o tipo de contrato e o perfil dos clientes.

## 5. Proteger os Clientes de Alto Valor

Criar ações específicas para clientes com mensalidades superiores a 80 €, como:

* atendimento prioritário;
* revisão periódica do plano;
* ofertas personalizadas;
* benefícios de fidelização;
* contacto preventivo;
* acompanhamento de satisfação.

## 6. Desenvolver um Modelo Preditivo

Utilizar os resultados desta análise como base para um futuro modelo de Machine Learning capaz de identificar clientes em risco antes do cancelamento.

O modelo poderá considerar variáveis como:

* tipo de contrato;
* tempo de permanência;
* apoio técnico;
* método de pagamento;
* mensalidade;
* serviços contratados.

---

#  Limitações da Análise

Esta análise apresenta algumas limitações:

* O dataset representa uma fotografia dos clientes num determinado momento.
* Não existe um histórico mensal da evolução dos clientes.
* Não estão disponíveis datas específicas de cancelamento.
* O impacto anualizado foi estimado através da multiplicação da faturação mensal por 12.
* A análise identifica associações, mas não permite provar relações de causa e efeito.
* A segmentação por valor foi criada especificamente para este projeto.
* Não foram considerados custos de aquisição, margens, descontos ou custos operacionais.
* Não existe informação detalhada sobre reclamações ou interações com o apoio ao cliente.
* Não foi desenvolvido um modelo preditivo nesta fase do projeto.

---

#  Ficheiros do Projeto

O repositório inclui:

* `telco_churn.ipynb` — notebook com a preparação, limpeza e análise dos dados.
* `telco_customer_churn_original.csv` — dataset utilizado como ponto de partida.
* `telco_churn_limpo.csv` — dataset tratado e enriquecido para utilização no Power BI.
* `telco_churn_dashboard.pbix` — dashboard interativo desenvolvido em Power BI.
* Imagens das três páginas do dashboard.

---

#  Competências Demonstradas

## Análise de Dados

* Data Cleaning
* Data Validation
* Exploratory Data Analysis
* Feature Engineering
* Customer Analytics
* Churn Analysis
* Customer Segmentation
* Financial Analysis

## Business Intelligence

* Power BI
* Data Modelling
* KPI Development
* Dashboard Design
* Business Analytics
* Data Storytelling

## Tecnologias

* Python
* Pandas
* Jupyter Notebook
* Google Colab
* Power BI

---

#  Conclusão

Este projeto permitiu transformar dados de clientes numa análise orientada para a retenção e proteção da receita.

Os resultados demonstram que o churn está particularmente associado a contratos mensais, ausência de apoio técnico, menor tempo de permanência, utilização de cheque eletrónico e mensalidades mais elevadas.

A análise permitiu identificar grupos prioritários para ações de retenção, quantificar o impacto financeiro do churn e preparar uma base de dados limpa e enriquecida para utilização num dashboard interativo em Power BI.

