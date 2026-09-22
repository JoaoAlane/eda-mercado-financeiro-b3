# 📊 Análise de Risco de Ações da B3

> 💼 Projeto de portfólio desenvolvido para demonstrar habilidades em análise de dados com Python. Faz parte dos meus estudos em Ciência e Análise de Dados.

Análise exploratória dos retornos diários de quatro ações da B3 (PETR4, VALE3, ITUB4, MGLU3) comparadas ao Ibovespa (^BVSP), com foco em risco, volatilidade e relação entre os ativos.

## 🎯 Objetivo

Entender como diferentes ações brasileiras se comportam em termos de risco e retorno no período de 2019 a 2024, e como cada uma se relaciona com o índice de mercado (Ibovespa).

## 🔍 O que foi feito

- 📥 Coleta de dados históricos de preços via Yahoo Finance
- 🧮 Cálculo dos retornos diários (variação percentual)
- 📈 Estatísticas descritivas: média, mediana, volatilidade (diária e anualizada), amplitude interquartil
- 🔔 Assimetria e curtose, para entender o formato da distribuição dos retornos
- ⚖️ Índice de Sharpe anualizado (com taxa livre de risco), para medir retorno ajustado ao risco
- 📊 Visualizações: histogramas, boxplot comparativo e heatmap de correlação
- 🔗 Matriz de correlação e covariância entre os ativos

## 🛠️ Tecnologias utilizadas

- Python
- Pandas
- NumPy
- yfinance
- Matplotlib
- Seaborn
- Jupyter Notebook

## 💡 Principais insights

- Ações individuais são bem mais voláteis e têm mais risco de dias extremos do que o Ibovespa, já que o índice diversifica esse risco entre várias empresas.
- MGLU3 apresentou a maior volatilidade do grupo.
- Ativos com menor correlação entre si (como MGLU3 e VALE3) são mais interessantes para diversificação de carteira.
- Os retornos não seguem uma distribuição normal perfeita, em parte por causa de eventos extremos no período analisado — como a crise da Covid-19 em 2020, que gerou dias de variação muito acima do normal.

## ▶️ Como executar

1. Clone o repositório
2. Instale as dependências: `pip install yfinance pandas numpy matplotlib seaborn`
3. Abra o notebook `financial_data_analysis.ipynb` no Jupyter e execute as células em ordem
