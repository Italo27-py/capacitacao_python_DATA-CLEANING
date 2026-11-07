🐍 Capacitação Prática em Python para Ciência de Dados — Case Campe Supply
![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Cleaning-150458?logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-Data%20Viz-4C72B0)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)
Bem-vindo(a) ao repositório oficial da nossa Capacitação de Python para Ciência de Dados!
Este treinamento de 5 horas foi desenhado para ensinar análise e tratamento de dados na prática, simulando o fluxo real de um projeto: desde o recebimento de uma planilha bruta e cheia de problemas até a entrega de insights visuais para a tomada de decisão.
---
🎯 O Desafio: Case "Campe Supply"
A Campe Supply é uma distribuidora que atua nas regiões Sul, Sudeste e Nordeste atendendo clientes de Atacado, Atacarejo e Varejo. A diretoria precisa entender o desempenho de seus vendedores, setores e produtos ao longo do ano, mas a base de dados original (`Campe_Supply_Corrompido.xlsx`) possui diversas inconsistências reais:
Colunas inúteis que mascaram registros duplicados;
Erros de digitação em variáveis categóricas (ex: `"Cvrnes"`, `"Vacessa"`, `"Attcarejo"`);
Valores numéricos corrompidos com letras infiltradas (ex: `"60b.72"`);
Dados ausentes (`NaN`) e outliers extremos causados por erros de digitação financeira.
---
📚 Cronograma das Aulas (5 Módulos de 1h)
Aula	Notebook	Tema Principal	O que você vai aprender
01	`Aula_01_Setup_e_Diagnostico.ipynb`	Setup, Importação e Diagnóstico	Leitura de arquivos Excel (`read_excel`), inspeção estrutural (`info`, `shape`, `isna`), padronização de colunas (snake_case) e remoção de colunas inúteis e duplicatas (`drop`, `drop_duplicates`).
02	`Aula_02_Limpeza_Textos_e_Funcoes.ipynb`	Limpeza de Texto e Cruzamento Lógico	Inspeção com `value_counts`, criação de funções (`def`) com `difflib` e `.apply()` para corrigir erros de digitação automaticamente e recuperação de nulos com dicionários (`.map()` e `.fillna()`).
03	`Aula_03_Limpeza_Numerica_e_Outliers.ipynb`	Limpeza Numérica e Outliers	Conversão de tipos (`to_numeric`), detecção e correção de erros matemáticos ($\text{Lucro} = \text{Faturamento} \times \text{Margem}$), tratamento de outliers e extração de informações de datas (`dt.month`).
04	`Aula_04_Analise_Exploratoria_Negocio.ipynb`	Análise Exploratória (EDA) e KPIs	Estatística descritiva (`describe`), criação de indicadores de negócio, agrupamentos avançados (`groupby` + `.agg`), tabelas dinâmicas (`pivot_table`) e filtros com `.query()`.
05	`Aula_05_Visualizacao_e_Storytelling.ipynb`	Visualização de Dados e Storytelling	Criação e personalização de gráficos executivos com `matplotlib` e `seaborn`: Gráfico de Linha (sazonalidade), Barras Horizontais (ranking), Boxplot (distribuição) e Heatmap (mapa de calor).
---
📂 Estrutura do Repositório
```text
📦 capacitacao-python-ciencia-dados
 ┣ 📜 Campe_Supply_Corrompido.xlsx                     # Base de dados bruta (com armadilhas)
 ┣ 📓 Aula_01_Setup_e_Diagnostico.ipynb                # Módulo 1
 ┣ 📓 Aula_02_Limpeza_Textos_e_Funcoes.ipynb           # Módulo 2
 ┣ 📓 Aula_03_Limpeza_Numerica_e_Outliers.ipynb        # Módulo 3
 ┣ 📓 Aula_04_Analise_Exploratoria_Negocio.ipynb       # Módulo 4
 ┣ 📓 Aula_05_Visualizacao_e_Storytelling.ipynb        # Módulo 5
 ┣ 📓 Capacitacao_Python_Campe_Supply_Completo.ipynb   # Gabarito Mestre Unificado
 ┗ 📜 README.md                                        # Documentação do projeto
```
---
🚀 Como Executar o Projeto (PyCharm / Jupyter)
Clone este repositório:
```bash
   git clone https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git
   cd NOME-DO-REPOSITORIO
   ```
Instale as bibliotecas necessárias:
```bash
   pip install pandas numpy openpyxl matplotlib seaborn jupyter
   ```
Abra no PyCharm (ou VS Code / Jupyter Lab):
Certifique-se de que o arquivo `Campe_Supply_Corrompido.xlsx` está na mesma pasta dos notebooks (`.ipynb`).
Abra o notebook da aula desejada e execute as células sequencialmente.
---
🛠️ Tecnologias Utilizadas
Python 3
Pandas & NumPy (Manipulação, limpeza e análise de dados)
Difflib (Correspondência aproximada de strings para limpeza de texto)
Matplotlib & Seaborn (Visualização de dados e storytelling)
OpenPyXL (Leitura e exportação de planilhas Excel `.xlsx`)
