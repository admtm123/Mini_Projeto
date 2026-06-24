# MiniProjeto DataView
 
## Sobre o projeto
**MiniProjeto DataView** O objetivo do projeto é criar um fluxo completo de análise de dados que leia, limpe, transforme, analise e visualize um dataset de vendas, gerando insights relevantes e um relatório exportável.

## O que o projeto analisa
- Como as vendas se comportam ao longo do tempo (por mês, por trimestre);
- Quais produtos e categorias geram mais receita;
- Quais regiões têm melhor desempenho;
- Quais clientes são mais valiosos (segmentação simples: Bronze, Prata, Ouro)
- Comparação entre os dados com e sem tratamento de outliers (v1 e v2)
- Exportação de relatórios em CSV e JSON

## Objetivo
Praticar os principais conceitos:
- Lógica de programação com Python
- Variáveis, tipos de dados e operadores
- Condicionais (if, elif, else) e repetição (for, while)
- Funções com parâmetros, retorno e funções lambda
- Funções reutilizáveis
- Leitura e escrita de arquivos CSV e JSON
- Módulo datetime para manipulação de datas
- Expressões regulares com o módulo re
- Pandas: DataFrames, limpeza, groupby, filtros e transformações
- NumPy: arrays, operações vetorizadas, broadcasting
- Detecção e tratamento de outliers (IQR ou z-score)
- Matplotlib e Seaborn: gráficos, customização e exportação em PNG
- Uso básico do GitHub


## Estrutura do projeto
```
Mini_Projeto/
|-- data/
|   |-- raw/                       # vendas.csv
|   |-- processed/
|   |   |-- v1_com_outliers/       # limpeza, outliers mantidos 
|   |   |-- v2_outliers_tratado/   # limpeza + outliers tratados
|   |-- final/                     # versao escolhida (v2) 
|-- notebooks/                     # Dataset escolhido para uso futuro 
|   |-- dataview.ipynb             # notebook principal de EDA
|-- outputs/
|   |-- metricas_por_mes.csv
|   |-- segmentacao_clientes.csv
|   |-- estatisticas_gerais.json
|   |-- graficos/                  # Gráficos exportados
|-- README.md
```

## Como executar
### Localmente com VS Code
1. Instale o Python 3.10+ e o VS Code.
2. Instale as dependências:
   pip install pandas numpy matplotlib seaborn

## Decisão de versão (dados)
A análise final usa a versão **v2** (outliers tratados). 
Motivo: Outliers (valores extremos) distorcem as estatísticas e métricas.
Além disso, outliers podem ser:
 - Erros de entrada de dados;
 - Casos muito especiais que não refletem o padrão;
 - Ruído que mascara tendências genuínas;
Então, v2 é a escolha mais segura para análises descritivas e segmentação de clientes.

A v1 (com outliers) fica preservada em `data/processed/` para consulta futura.

## Ferramentas utilizadas
- Python 3.10+
- Bibliotecas: pandas, numpy, matplotlib, seaborn
- VS Code
- GitHub para versionamento

## Vídeo de demonstração
https://drive.google.com/drive/folders/1ckjQk9gMGSy10Hg40hjRegLrGIDGg9cK?usp=drive_link
