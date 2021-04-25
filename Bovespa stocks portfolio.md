# Carteira de ações da Bovespa

**Objetivos:** Elaborar um portfólio de ações com base em dados históricos.


## Obtendo os dados

Existem cadernos de notas *Notebook Jupyter* separados que explicam como fazer o download e preparar os conjuntos de dados.

*Os textos principais estão em português, mas os códigos / comentários estão em inglês.*

**Preparação de dados**

 - Obtenção do *Yahoo! Finanças* citações históricas
   - [Notebook Jupyter: baixando ações da Bovespa] (https://github.com/devscie/PythonBovespa/blob/main/bovespa_tickers_download.ipynb)
 - Limpeza de dados
   - pré-processamento [Notebook Jupyter: pré-processamento] (https://github.com/devscie/PythonBovespa/blob/main/bovespa_tickers_portfolio.ipynb)

## Portfólio via otimização convexa do índice de Sharpe esperado

O objetivo é elaborar uma carteira com bom desempenho utilizando um número reduzido de ações da lista disponível.

Para cada mês, é elaborada uma carteira de ações com base no índice de retorno de log de Sharpe dos meses anteriores. O desempenho do portfólio é comparado com três benchmarks:
- iBovespa: o índice oficial da Bovespa (composto por +60 ações)
- Média BVSP: média simples de todas as ações disponíveis da iBovespa
- Dolar: O valor atual dos dólares americanos em reais


**Resultados esperados:**

- Melhor desempenho (médio) a longo prazo
- Alta volatilidade devido ao pequeno número de ações que compõem a carteira


**Veja o [Notebook Jupyter] (https://github.com/devscie/PythonBovespa/blob/main/bovespa_tickers_download_portfolio.ipynb) apresentando todo o procedimento e resultados.**