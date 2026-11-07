# 🐍 Capacitação Prática de Python para Ciência de Dados — Case Campe Supply

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Cleaning-150458?logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-Data%20Viz-4C72B0)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-brightgreen)

Bem-vindo(a) ao repositório oficial da nossa **Capacitação de Python para Ciência de Dados**! 

Este treinamento de **5 horas (5 módulos práticos)** foi desenhado para ensinar o fluxo real de um projeto de dados: desde a recepção de uma planilha corporativa completamente corrompida até a limpeza avançada, validação matemática, análise exploratória (EDA) e construção de gráficos executivos.

---

## 🎯 O Desafio: Case "Campe Supply"

A **Campe Supply** é uma distribuidora que atua nas regiões Sul, Sudeste e Nordeste atendendo os canais de *Atacado*, *Atacarejo* e *Varejo*. A diretoria precisa de respostas estratégicas sobre o desempenho comercial, mas a base de dados bruta (`Campe_Supply_Corrompido.xlsx`, com 1.690 linhas e 13 colunas) apresenta problemas reais de qualidade:

* **Colunas de lixo e duplicatas ocultas:** Colunas com hashes aleatórios (`UNNAMED: 0`, `coluna_inutil_0`, `coluna_inutil_1`) que mascaram vendas duplicadas.
* **Erros de digitação em textos:** Mais de 140 variações incorretas de nomes (ex: `"Cvrnes"`, `"Vacessa"`, `"Attcarejo"`).
* **Números corrompidos como texto:** Valores financeiros com letras infiltradas (ex: `"60b.72"`, `"0.a6"`).
* **Outliers e inconsistências matemáticas:** Linhas onde a regra $\text{Lucro} = \text{Faturamento} \times \text{Margem}$ foi violada (incluindo lucros irreais na casa dos milhões).

---

## 📚 Cronograma das Aulas (5 Módulos de 1h)

| Aula | Arquivo (`.ipynb`) | Tema Principal | O que você vai aprender |
| :--- | :--- | :--- | :--- |
| **01** | `Aula_01_Setup_e_Diagnostico.ipynb` | **Setup, Importação e Diagnóstico** | Leitura com `pandas`, inspeção de tipos (`info`, `isna`), padronização de colunas (*snake_case*) e remoção de colunas inúteis e duplicatas primárias. |
| **02** | `Aula_02_Limpeza_Textos_e_Funcoes.ipynb` | **Limpeza de Texto e Funções** | Criação de funções (`def` + `.apply()`) com `difflib` para corrigir erros de digitação automaticamente e cruzamento lógico (`.map()` + `.fillna()`) para recuperar setores e regiões vazias. |
| **03** | `Aula_03_Limpeza_Numerica_e_Outliers.ipynb` | **Limpeza Numérica e Outliers** | Conversão com `pd.to_numeric()`, caça e correção de 5 outliers graves usando regras de negócio, recuperação matemática de `NaN` e eliminação da 2ª onda de duplicatas. |
| **04** | `Aula_04_Analise_Exploratoria_Negocio.ipynb` | **Análise Exploratória (EDA)** | Cálculo de KPIs gerais, ranking de vendedores e produtos com `.groupby()` e `.agg()`, matrizes com `pd.pivot_table()` e filtros avançados com `.query()`. |
| **05** | `Aula_05_Visualizacao_e_Storytelling.ipynb` | **Visualização e Storytelling** | Criação de gráficos executivos com `matplotlib` e `seaborn`: sazonalidade mensal (*lineplot*), ranking comercial (*barplot*), distribuição (*boxplot*) e mapa de calor (*heatmap*). |
