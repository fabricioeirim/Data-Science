📊 Análise de Dados Financeiros Governamentais
📌 Visão Geral
Este projeto realiza uma análise exploratória e estatística de dados financeiros governamentais, com foco em entender a relação entre gastos públicos (educação e saúde), receitas do governo e o crescimento do PIB ao longo do tempo.
A análise utiliza dados públicos disponibilizados pelo Banco Mundial, coletados via API, tratados e analisados com Python e bibliotecas de ciência de dados.

🎯 Objetivos da Análise
As principais perguntas que orientam o projeto são:

📈 Em que ano o país apresentou maior crescimento do PIB per capita?
🏥 Qual ano teve as maiores despesas com saúde?
🎓 Qual ano teve os maiores gastos com educação?
💰 Como a receita do governo se correlaciona com a despesa do governo?
🔗 Como os gastos com educação e saúde se correlacionam com o crescimento do PIB?
📉📈 Como os gastos do governo com educação e saúde afetam o crescimento do PIB?
🧠 Com base na análise, quais recomendações podem ser feitas aos gestores públicos?


🗂️ Fonte dos Dados

Origem: Banco Mundial (World Bank)
Acesso: API pública
🔗 http://api.worldbank.org/v2/en/country

Os dados incluem indicadores econômicos e sociais como:

PIB
Crescimento populacional
Despesas com saúde e educação
Receita tributária
Gastos nacionais brutos


🛠️ Tecnologias Utilizadas

Python 3
Pandas – manipulação e análise de dados
NumPy – operações numéricas
Matplotlib / Seaborn – visualização de dados
Scikit-learn – regressão linear
OpenPyXL – leitura de arquivos Excel
Jupyter Notebook


🧪 Pipeline da Análise
1️⃣ Carregamento e Compreensão dos Dados

Leitura do dataset original em Excel
Avaliação da estrutura, tipos de dados e dimensões
Identificação de valores ausentes


2️⃣ Limpeza e Processamento

Tratamento de valores ausentes com:

Backfilling
Interpolação


Remoção de colunas redundantes
Padronização e arredondamento de valores
Exportação do dataset limpo (dataset_limpo.csv)


3️⃣ Análise Exploratória (EDA)

Análise estatística descritiva
Visualizações temporais
Identificação de tendências e outliers
Cálculo de gastos absolutos com:

Saúde
Educação




4️⃣ Análise de Correlação

Correlação de Pearson entre variáveis econômicas
Visualização com heatmap
Interpretação das relações entre:

Receita tributária
Despesas públicas
Crescimento do PIB




5️⃣ Modelagem Estatística

Construção de um modelo de regressão linear
Avaliação do impacto combinado dos gastos com:

Educação
Saúde


Interpretação do coeficiente de regressão


📈 Principais Resultados
✅ Crescimento do PIB per Capita

O maior crescimento do PIB per capita ocorreu no ano com o maior valor da variável pib_cresc_per_capita_%pib.

✅ Gastos com Saúde

O maior gasto absoluto com saúde ocorreu em 2019, impulsionado pelo aumento do gasto nacional bruto.

✅ Gastos com Educação

Os maiores gastos com educação acompanham o crescimento do gasto público total ao longo dos anos.


🔗 Correlações Relevantes


Receita tributária × Despesas com saúde:
Correlação positiva forte (+0,78)


Receita tributária × Despesas com educação:
Correlação positiva moderada (+0,47)


Empréstimos (BIRD / AID) × Educação:
Correlação positiva forte (+0,75), indicando dependência de financiamento externo


Educação × Crescimento do PIB:
Correlação levemente negativa (-0,15)


Saúde × Crescimento do PIB:
Correlação levemente negativa (-0,05)



📉 Impacto dos Gastos no Crescimento do PIB
A regressão linear indica que:

Os gastos combinados com educação e saúde têm um impacto positivo no crescimento do PIB
O coeficiente estimado é 5.2e‑13, um valor pequeno em termos absolutos, mas positivo
O resultado sugere que o impacto ocorre no longo prazo, e não de forma imediata


🧠 Recomendações aos Gestores Públicos
Com base na análise:

✅ Manter investimentos consistentes em educação e saúde, considerando seus efeitos estruturais de longo prazo
✅ Reduzir dependência excessiva de financiamento externo
✅ Avaliar a eficiência dos gastos, não apenas o volume investido
✅ Integrar políticas sociais com estratégias de crescimento econômico sustentável


🚀 Possíveis Extensões do Projeto

Análise por país ou comparação entre países
Modelos econométricos mais avançados
Séries temporais (ARIMA, VAR)
Análise de causalidade
Dashboards interativos


📄 Observações
Projeto desenvolvido com finalidade educacional, voltado ao aprendizado de análise de dados, estatística aplicada e ciência de dados, utilizando dados públicos governamentais.
