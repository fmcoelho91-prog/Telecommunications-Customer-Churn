# 📉 B2B SaaS Customer Churn Analysis Dashboard

## Resumo do Projecto

Este projeto foi desenvolvido com o objetivo de analisar o abandono de clientes (*Customer Churn*) numa empresa B2B do setor das telecomunicações/SaaS.

Através de uma análise exploratória de dados (EDA), foram identificados os principais fatores associados ao churn, quantificado o impacto financeiro da perda de clientes e desenvolvidas recomendações estratégicas para melhorar a retenção e proteger a receita recorrente da empresa.

---

# Questões de Negócio

O projeto procurou responder às seguintes questões:

- Qual é a taxa global de churn da empresa?
- Qual o impacto financeiro do abandono de clientes?
- Que segmentos apresentam maior risco de cancelamento?
- Que serviços estão associados a uma maior retenção?
- Quais as oportunidades para reduzir o churn?

---

#  Tecnologia Utilizada

- Python
- Pandas
- NumPy
- Power BI
- Jupyter Notebook

---

# Processo de Análise

## Preparação dos dados

- Limpeza e validação dos dados
- Tratamento de valores inconsistentes
- Feature Engineering
- Segmentação de clientes por nível de faturação

## Análise Exploratória

Foram analisadas diversas variáveis para identificar padrões de abandono:

- Tipo de contrato
- Serviços contratados
- Apoio Técnico
- Tempo de permanência (Tenure)
- Receita mensal
- Segmentação de clientes

---

# 📊 Dashboard Interactivo

Os resultados da análise foram apresentados através de um dashboard desenvolvido em **Power BI**, dividido em três páginas complementares.

## Executive Overview

Visão executiva dos principais indicadores de negócio, incluindo taxa de churn, receita em risco e distribuição dos clientes.

![Executive Overview](https://github.com/fmcoelho91-prog/B2B-SaaS-Churn-Analysis/blob/main/Dashboard%201.png)

---

## Customer Segmentation

Análise dos segmentos com maior risco de abandono através do cruzamento de contratos, serviços, métodos de pagamento e perfis de clientes.

![Customer Segmentation](https://github.com/fmcoelho91-prog/B2B-SaaS-Churn-Analysis/blob/main/Dashboard%202.png)

---

## Financial Impact & Recommendations

Quantificação do impacto financeiro do churn e apresentação de recomendações estratégicas orientadas para a retenção de clientes.

![Financial Impact](https://github.com/fmcoelho91-prog/B2B-SaaS-Churn-Analysis/blob/main/Dasboard%203.png)

---

# Principais Descobertas

## 📉 Global Churn Rate

A empresa apresenta uma taxa global de abandono de **26,5%**, evidenciando uma oportunidade significativa para melhorar a retenção de clientes.

---

##  Financial Impact

Os clientes que abandonaram o serviço representam uma perda estimada de **139.130,85 € de Receita Recorrente Mensal (MRR)**, equivalente a mais de **1,6 milhões de euros por ano**.

---

## Segmento de Maior Risco

O segmento **Enterprise** apresenta a maior taxa de churn (**33%**), comprometendo uma parte significativa da receita da empresa.

Em contrapartida, o segmento **Starter** demonstrou uma taxa de abandono bastante inferior (**11%**).

---

## Impacto do Apoio Tecnico

Os clientes com contratos **Month-to-Month** e sem serviço de **Tech Support** apresentam uma taxa de churn superior a **50%**.

Quando existe Apoio Técnico, essa taxa reduz-se para aproximadamente **15%**, demonstrando a forte correlação entre suporte ao cliente e retenção.

---

#  Recomendações Estratégicas

Com base na análise realizada, foram propostas as seguintes ações:

- Priorizar campanhas de retenção para clientes Enterprise.
- Promover a adesão ao serviço de Tech Support durante os primeiros meses de contrato.
- Incentivar a migração de contratos Month-to-Month para contratos anuais.
- Monitorizar continuamente os principais indicadores de churn através de dashboards.
- Desenvolver modelos preditivos para identificar clientes em risco antes do cancelamento.

---

#  Competências Demonstradas

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Customer Analytics
- Churn Analysis
- Financial Analysis
- Business Intelligence
- Business Analytics
- Data Storytelling
- Python
- Pandas
- NumPy
- Power BI

---

# 📂 Repository Structure

```text
📁 data/
    customer_churn.csv

📁 notebooks/
    Churn_Analysis.ipynb

📁 powerbi/
    Churn_Dashboard.pbix

📁 images/
    executive_overview.png
    customer_segmentation.png
    financial_impact.png

📄 README.md
```

---

##  About

Este projeto demonstra um fluxo completo de análise de dados, desde a preparação e exploração dos dados em Python até à criação de dashboards executivos em Power BI, convertendo informação analítica em recomendações de negócio orientadas para a redução do churn e aumento da retenção de clientes.
```
