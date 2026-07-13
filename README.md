
# 📉 B2B SaaS Customer Churn Analysis

##  Project Overview

Este projeto foi desenvolvido com o objetivo de analisar o abandono de clientes (*Customer Churn*) numa empresa B2B do setor das telecomunicações/SaaS.

Através de uma análise exploratória de dados (EDA), foram identificados os principais fatores associados ao churn, quantificado o impacto financeiro da perda de clientes e propostas recomendações para melhorar a retenção.

---

#  Business Questions

O projeto procurou responder às seguintes questões:

- Qual é a taxa global de churn da empresa?
- Qual o impacto financeiro do abandono de clientes?
- Que segmentos apresentam maior risco de cancelamento?
- Que serviços estão associados a uma maior retenção?
- Quais as oportunidades para reduzir o churn?

---

#  Ferramentas Utilizadas

- Python
- Pandas
- NumPy
- Power BI
- Jupyter Notebook

---

#  Processo de Análise

### Preparação dos Dados

- Limpeza e validação dos dados
- Tratamento de valores inconsistentes
- Criação de novas variáveis (Feature Engineering)
- Segmentação de clientes por nível de faturação

### Análise Exploratória

Foram analisadas diversas variáveis para identificar padrões de abandono:

- Tipo de contrato
- Serviços contratados
- Apoio Técnico
- Tempo de permanência
- Receita mensal
- Segmentação de clientes

### Dashboard

Os resultados foram apresentados através de um dashboard interativo em Power BI para facilitar a análise dos principais indicadores de negócio.

---

#  Principais Descobertas

##  Taxa Global de Churn

A empresa apresenta uma taxa global de abandono de **26,5%**, indicando uma oportunidade significativa para melhorar a retenção de clientes.

---

##  Impacto Financeiro

Os clientes que abandonaram o serviço representam uma perda estimada de **139.130,85 € de receita recorrente mensal (MRR)**, equivalente a mais de **1,6 milhões de euros por ano**.

---

##  Segmentos de Maior Risco

O segmento **Enterprise** apresenta a maior taxa de abandono (**33%**), comprometendo uma parte significativa da receita da empresa.

Por outro lado, o segmento **Starter** demonstrou uma taxa de churn bastante inferior (**11%**).

---

##  O impacto do Apoio Técnico

Os clientes com contratos mensais (*Month-to-Month*) e sem serviço de **Tech Support** apresentam uma taxa de churn superior a **50%**.

Quando existe Apoio Técnico, essa taxa reduz-se para aproximadamente **15%**, evidenciando a importância deste serviço na retenção de clientes.

---

#  Recomendações

Com base na análise realizada, foram propostas as seguintes ações:

- Reforçar estratégias de retenção para clientes Enterprise.
- Promover a adesão ao serviço de Tech Support nos primeiros meses de contrato.
- Desenvolver campanhas direcionadas para clientes com contratos Month-to-Month.
- Monitorizar regularmente os indicadores de churn através de dashboards.

---

# Competências Demonstradas

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Customer Analytics
- Churn Analysis
- Financial Analysis
- Business Intelligence
- Python
- Pandas
- NumPy
- Power BI

---

# 📂 Estrutura do Repositório

```text
📁 data/
    customer_churn.csv

📁 notebooks/
    Churn_Analysis.ipynb

📁 powerbi/
    Churn_Dashboard.pbix

📁 images/
    dashboard.png

📄 README.md
```
