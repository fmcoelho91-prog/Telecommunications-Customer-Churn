# B2B-SaaS-Churn-Analysis
Projeto de Análise Exploratória (EDA) em Python focado em retenção de clientes B2B.


#  B2B SaaS Customer Churn Analysis

##  O Problema de Negócio
Uma empresa B2B do setor das telecomunicações/SaaS está a enfrentar um problema grave de retenção de clientes, o objetivo deste projeto é analisar uma base de dados de +7.000 clientes, identificar os segmentos de maior risco e quantificar o impacto financeiro do abandono (Churn).

## Ferramentas Utilizadas
* **Python (Pandas, NumPy):** Limpeza de dados, feature engineering (criação de Tiers Financeiros e métricas comportamentais) e análise exploratória cruzada.
* **Power BI:** Criação de Dashboard interativo para apresentação à Administração *(Em desenvolvimento)*.

## Principais Descobertas (Insights Estratégicos)
Após a análise exploratória e cruzamento de variáveis, detetámos cenários críticos:

1. **Alerta Vermelho de Retenção:** A taxa de Churn global da empresa encontra-se nos **26.5%**.
2. **Impacto Financeiro:** Os clientes que abandonaram o serviço representam uma perda de receita mensal (MRR) de **139.130,85 €** (mais de 1.6 Milhões de euros anualizados).
3. **Churn de Receita vs Churn de Clientes:** O segmento que mais cancela o serviço é precisamente o **Enterprise (33%)**, que suporta o ARPU da empresa. O segmento Starter é o mais leal (11% de churn).
4. **O Cenário de Pesadelo:** O risco de abandono dispara para os **50.3%** quando um cliente tem um contrato sem fidelização (Month-to-month) e **não possui** serviço de Apoio Técnico (Tech Support). Em contrapartida, clientes com Apoio Técnico reduzem o risco de saída para apenas 15.2%.

## Recomendações Preliminares
* Reestruturação imediata da estratégia de *Customer Success* para a conta Enterprise.
* Criação de campanhas para oferecer/incluir o *Tech Support* nos primeiros meses de contrato, dada a sua correlação direta com o aumento drástico da taxa de retenção.

---
*Ficheiro de código e dataset limpo disponíveis neste repositório para consulta.*
