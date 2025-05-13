Relatório: Manipulação de Dados Estruturados com Pandas

## Introdução
O Pandas é uma biblioteca Python essencial para análise e manipulação de dados estruturados. Este relatório demonstra sua aplicação na criação de `Series` e `DataFrames`, extração de informações e filtragem de dados, destacando sua eficiência no tratamento de dados tabulares.

---

## Procedimentos

### 1. **Criação de Series**
- **Objetivo**: Armazenar dados unidimensionais com rótulos.
- **Método**: 
  ```python
  serie = pd.Series([100, 200, 300, 400], index=['A', 'B', 'C', 'D'])
Resultado: Uma Series com valores associados a índices alfabéticos.

2. Criação de DataFrames
Objetivo: Estruturar dados em formato tabular.

Métodos:

Dicionário de listas:

python
pd.DataFrame({'Nome': ['Ana', 'Bruno'], 'Idade': [22, 35]})
Lista de listas:

python
pd.DataFrame([['Lucas', 28], ['Mariana', 32]], columns=['Nome', 'Idade'])
Resultado: DataFrames com colunas definidas e dados organizados.

3. Extraindo Informações
Objetivo: Analisar estrutura e estatísticas dos dados.

Métodos:

df.info(): Mostra tipos de dados e valores não nulos.

df.describe(): Estatísticas descritivas para colunas numéricas.

df.head(): Exibe as primeiras linhas.

Seleções com loc e filtros (ex: df[df['Idade'] > 25]).

Resultados
Series: Permitiram acesso rápido a valores via índices (ex: serie['B'] retornou 200).

DataFrames:

Dados foram organizados de forma intuitiva, com colunas nomeadas.

Filtros como Idade > 25 isolaram registros específicos (ex: Bruno, 35 anos).

Análise Descritiva: Métodos como describe() revelaram médias e distribuições (ex: idade média de 28.7 anos).

Conclusão
O Pandas mostrou-se uma ferramenta poderosa para:

Estruturação de dados: Transformação de listas/dicionários em tabelas.

Consulta eficiente: Seleção de linhas/colunas com sintaxe intuitiva.

Análise rápida: Cálculo de estatísticas e filtros com poucas linhas de código.

Aprendizado-chave: A combinação de Series e DataFrames com métodos de análise integrados acelera significativamente o fluxo de trabalho com dados.

Bibliografia
McKinney, W. Python for Data Analysis. O'Reilly, 2022.

Documentação oficial do Pandas: pandas.pydata.org

Data Science Handbook – Jake VanderPlas (O'Reilly, 2016).
