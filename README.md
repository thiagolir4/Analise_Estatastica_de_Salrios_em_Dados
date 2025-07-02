# 📊 Projeto de Análise de Salários na Área de Dados com Python

Este repositório contém um projeto completo de análise de dados, focado em salários de profissionais da área de tecnologia. O objetivo é aplicar conceitos de estatística descritiva e manipulação de dados para extrair insights valiosos sobre o mercado de trabalho. O desenvolvimento foi realizado utilizando Python com as bibliotecas **pandas**, **Matplotlib** e **Seaborn**.

Este projeto segue um roteiro estruturado de análise, simulando um desafio real de dados, e serve como um portfólio prático das técnicas aprendidas durante o curso de formação em **Engenheiro de Dados da Escola DNC**.

---

## 📁 Estrutura do Projeto e Acesso aos Códigos
Os códigos e análises estão organizados em um script ou notebook Jupyter (`.ipynb`) neste repositório. Você pode navegar pelo arquivo para acessar o código específico de cada etapa da análise, desde a limpeza dos dados até a visualização final e interpretação dos resultados.

---

## 📚 Conteúdo Abordado

-   **Introdução ao pandas e Manipulação de DataFrames**:
    -   Leitura de arquivos CSV (`pd.read_csv`).
    -   Visualização inicial do DataFrame para entender sua estrutura (`.head()`, `.info()`, `.shape`, `.columns`).
    -   Seleção de colunas de interesse para análises específicas.

-   **Limpeza e Preparação de Dados**:
    -   Identificação e contagem de valores ausentes (NaNs) com `.isnull().sum()`.
    -   Tratamento de dados ausentes através da remoção de linhas com `.dropna()`.
    -   Identificação e contagem de dados duplicados com `.duplicated().sum()`.
    -   Remoção de linhas duplicadas para garantir a qualidade da análise com `.drop_duplicates()`.

-   **Análise Exploratória de Dados (EDA)**:
    -   Análise descritiva univariada para variáveis categóricas e numéricas.
    -   Cálculo e interpretação de frequências absolutas e relativas (porcentagens) com `value_counts()` e o parâmetro `normalize=True`.
    -   **Cálculo de Medidas de Tendência Central**:
        -   Média (`.mean()`) para variáveis numéricas.
        -   Mediana (`.median()`) para variáveis numéricas, fundamental para entender a distribuição de salários.
    -   **Cálculo de Medidas de Dispersão**:
        -   Amplitude (através de `.min()` e `.max()`).
        -   Desvio Padrão (`.std()`).
    -   Utilização da função `describe()` para obter um resumo estatístico completo das variáveis numéricas.
    -   Agrupamento de dados para análises comparativas com `.groupby()`, utilizado para comparar salários por país.

-   **Análise de Correlação**:
    -   Cálculo da matriz de correlação entre as variáveis numéricas (`salary_in_usd`, `work_year`, `years_of_experience`) com `.corr()`.
    -   Análise da relação entre variáveis categóricas (Quali vs Quali) através da discussão de tabelas de contingência (`pd.crosstab`).

-   **Visualização de Dados**:
    -   Criação de gráficos de Histograma com **Seaborn** (`sns.histplot`) para visualizar a distribuição dos salários.
    -   Criação de gráficos de Boxplot com **Seaborn** (`sns.boxplot`) para comparar a distribuição salarial entre diferentes níveis de experiência.
    -   Criação de gráficos de Barras com **Seaborn** (`sns.barplot`) para visualizar os países com as maiores médias salariais.
    -   Visualização da matriz de correlação de forma intuitiva com um Mapa de Calor (Heatmap) do **Seaborn** (`sns.heatmap`).

---

## 📂 Dados Utilizados

Neste projeto, foi analisado o seguinte conjunto de dados:

1.  **`salario_profissionais_dados.csv`**:
    * **Descrição**: Dataset contendo informações sobre salários de profissionais da área de dados, incluindo variáveis como ano do registro, nível e anos de experiência, cargo, localização da empresa e salário em dólares (USD).
    * **Disponibilidade**: O arquivo f o material principal para este desafio de análise e está incluído no drive, conforme link -  https://drive.google.com/drive/folders/1sGmGykGOX0tz_ONaHpWe5TMyZYUQzGal?usp=sharing

---

## 🛠️ Tecnologias Utilizadas

-   [Python 3.x](https://www.python.org/)
-   [pandas](https://pandas.pydata.org/) (para manipulação e análise de DataFrames)
-   [Matplotlib](https://matplotlib.org/) (utilizada como base para os gráficos do Seaborn)
-   [Seaborn](https://seaborn.pydata.org/) (para visualizações estatísticas avançadas e mais elaboradas)
-   Ambiente de Desenvolvimento como VS Code ou Jupyter Notebook.

---

## 🎯 Objetivo

O objetivo principal deste projeto é demonstrar a aplicação prática de um ciclo completo de análise de dados. Partindo de um dataset bruto, foram realizadas as etapas de limpeza, exploração, análise estatística e visualização para responder a perguntas de negócio específicas sobre o mercado de trabalho em dados, tais como:
- Qual o perfil predominante dos profissionais?
- Como o salário se distribui e quais os principais fatores de influência?
- Onde estão as maiores médias salariais no mundo?
- Qual a relação entre experiência e remuneração?

Este trabalho serve como um portfólio prático das técnicas aprendidas durante o curso de **Engenheiro de Dados da Escola DNC**.

---

## 🚀 Como Utilizar

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
    cd seu-repositorio
    ```

2.  **Instale as dependências:**
    Recomenda-se a criação de um ambiente virtual para o projeto.
    ```bash
    pip install pandas matplotlib seaborn jupyterlab
    ```

3.  **Execute o notebook ou script:**
    Abra o arquivo `.ipynb` (com Jupyter Lab ou VS Code) ou execute o script `.py` para reproduzir toda a análise.

4.  **Verifique o Dataset:**
    Certifique-se de que o arquivo `salario_profissionais_dados.csv` está no mesmo diretório para que o código possa ser executado sem erros de caminho de arquivo.

---

## 📌 Observações

-   Este projeto foi desenvolvido como parte das atividades do curso de formação em Engenheiro de Dados da Escola DNC.
-   Os códigos são apresentados com fins didáticos e para demonstração das técnicas de análise de dados em um cenário prático.

---
