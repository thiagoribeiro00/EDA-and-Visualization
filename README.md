# Análise e Visualização de Dados de Veículos Elétricos por Condado

Este projeto realiza a análise de dados históricos de veículos elétricos em diferentes condados dos Estados Unidos. Através da leitura de um arquivo CSV, o projeto organiza, limpa e visualiza os dados para melhor compreensão das tendências e da penetração de veículos elétricos em comparação aos veículos não elétricos.

## Estrutura do Projeto

### 1. Importação de Bibliotecas

As bibliotecas utilizadas no projeto incluem:
- `numpy` e `pandas` para manipulação de dados
- `plotly.express`, `plotly.graph_objs`, `seaborn` e `matplotlib.pyplot` para visualizações interativas e estáticas.

### 2. Carregamento dos Dados

O dataset é carregado de um arquivo CSV chamado `Electric_Vehicle_Population_Size_History_By_County_.csv`. Cada registro contém informações sobre:
- Data
- Condado
- Estado
- Uso Primário do Veículo
- Quantidade de Veículos Elétricos a Bateria (BEVs) e Veículos Híbridos Plug-in (PHEVs)
- Percentual de Veículos Elétricos

### 3. Limpeza e Preparação dos Dados

Para análise mais detalhada, o projeto faz:
- Separação das colunas de data em `Ano`, `Mês` e `Dia`
- Conversão de colunas específicas com números representados com vírgulas para o formato numérico
- Substituição de valores nulos e tratamento de tipos de dados inconsistentes

### 4. Análise Exploratória

Realiza-se uma análise estatística básica, incluindo:
- Contagem, média, desvio padrão, e valores máximos e mínimos para as principais colunas numéricas
- Agrupamento de dados por condado para calcular a proporção de veículos elétricos em relação ao total de veículos

### 5. Visualizações

Visualizações são geradas para melhor compreensão dos dados, como:
- Gráficos de dispersão de `plotly` para comparar a proporção de veículos elétricos por condado
- Histogramas e gráficos de linha de `matplotlib` e `seaborn` para análise temporal
