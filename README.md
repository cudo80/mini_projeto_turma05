# Repositório contendo o Mini-projeto Avaliativo da turma 05 de Análise de Dados com Python
# Mini Projeto Turma 05

Projeto de análise exploratória de dados em Python, focado em uma base de varejo. O objetivo é explorar, limpar e interpretar os dados para identificar padrões de compra, comportamento dos clientes e relações entre categorias de produtos e classes econômicas.

## Descrição do projeto

Este notebook realiza uma análise inicial de uma base de dados de compras de varejo, com foco em:

- leitura e validação da base de dados
- limpeza de colunas e registros inconsistentes
- conversão de datas para o tipo datetime
- renomeação de colunas para facilitar a leitura
- análise descritiva de clientes, produtos e comportamento de compra
- identificação de padrões em relação ao número de filhos e categoria de produto

## Objetivo

Entender melhor a base de clientes e compras, respondendo perguntas como:

- Quantos clientes possuem filhos?
- Qual categoria de produto é mais frequente?
- Existe relação entre classe econômica e quantidade de filhos?
- Como os dados estão distribuídos em termos de qualidade e consistência?

## Base de dados

A base de dados utilizada foi obtida no Kaggle:

- https://www.kaggle.com/datasets/namespaiva/base-varejo/data

Recomenda-se baixar o arquivo `base-varejo.zip` e extrair o conteúdo na pasta raiz do projeto.

O arquivo esperado no projeto é:

- `Base Varejo.csv`

## Requisitos

Antes de executar o notebook, é necessário ter instalado:

- Python 3.x
- Pandas
- NumPy
- IPython

### Instalação

```bash
python -m pip install pandas numpy ipython
```

### Imports utilizados no notebook

```python
import pandas as pd
import numpy as np
import os
from IPython.display import display
```

## Como executar

1. Faça o download do arquivo `base-varejo.zip`
2. Extraia o conteúdo na pasta raiz do projeto
3. Verifique se o arquivo `Base Varejo.csv` está presente
4. Abra o arquivo `mini_projeto_turma05.ipynb`
5. Execute as células em ordem

## Estrutura do projeto

```text
mini_projeto_turma05/
├── mini_projeto_turma05.ipynb
├── Base Varejo.csv
├── README.md
└── .gitignore
```

## Etapas realizadas no notebook

- carregamento do arquivo CSV
- validação da existência do arquivo
- verificação de duplicatas e valores nulos
- conversão da coluna `DATA` para `datetime`
- remoção de colunas vazias
- limpeza de valores inconsistentes como `#N/D`
- renomeação das colunas para nomes mais claros
- análise de clientes com e sem filhos
- agrupamento por classe econômica e categoria de produto

## Bibliotecas utilizadas

- `pandas`
- `numpy`
- `os`
- `IPython.display`

## Observações importantes

- O notebook usa um caminho absoluto para o arquivo CSV, o que pode dificultar a execução em outros computadores.
- Para melhorar a portabilidade, o ideal é usar caminhos relativos ou a biblioteca `pathlib`.
- A base contém alguns registros com valores inválidos, que foram tratados durante a limpeza dos dados.

## Possíveis melhorias futuras

- tornar o caminho do arquivo mais dinâmico
- adicionar visualizações com `matplotlib` e `seaborn`
- criar métricas de faturamento e ticket médio
- segmentar clientes por perfil
- gerar indicadores de desempenho e conclusões finais

## Autor

Projeto desenvolvido para a turma 05, com foco em análise de dados com Python.

## Licença

Este projeto é destinado ao uso acadêmico e didático.