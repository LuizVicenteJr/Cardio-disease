## Resumo 
Este é um projeto de classificação de doenças cardiovasculares usando o conjunto de dados [Cardiovascular Disease Dataset](https://www.kaggle.com/sulianova/cardiovascular-disease-dataset). Com o pensamento voltado para a resolução de problemas de negócio, utilizei o meu conhecimento em Machine Learning, estatística e programação para criar um modelo de classificação de pacientes com doenças cardiovasculares. Meu objetivo principal foi não apenas focado na precisão do modelo, mas também em melhorar o recall do mesmo.
O recall é particularmente importante no contexto de detecção de doenças cardiovasculares,pois é melhor identificar uma maior quantidade de casos verdadeiramente positivos (pacientes com doenças cardiovasculares) para garantir que esses pacientes recebam o tratamento necessário o mais cedo possível, do que ter uma alta precisão, mas com um baixo recall, o que resultaria em pacientes com doenças cardiovasculares não sendo detectados e tratados adequadamente.
 
## Instalação
1. Clone este repositório: `git clone https://github.com/LuizVicenteJr/Cardio-disease.git`.
2. As bibliotecas utilizadas estão no arquivo : requeriments.txt
3. O último ciclo trabalho neste projeto consta em(https://github.com/LuizVicenteJr/Cardio-disease/blob/main/cardio_diseases_cycle5.ipynb) fique a vontade para melhorar o projeto com novos ciclos!


# **1.0 DATA DESCRIPTION**
Nesta etapa, os dados são carregados em um DataFrame do Pandas. Os dados são pré-processados para remover valores ausentes e duplicados. Também é criada uma coluna adicional para representar a idade em anos .

# **2.0 Feature Engineering**
São criadas novas features derivadas das já existentes e uma função que estima em pontos o risco de uma pessoa ter problemas cardíacos em 10 anos (para saber mais https://www.heartscore.org/en_GB/).

# **3.0 Exploratory Data Analysis - EDA**
São utilizadas diversas técnicas de análise de dados.Estas análises ajudam a entender melhor as características do conjunto de dados e identificar possíveis correlações entre as variáveis. Por exemplo, a matriz de correlação e os gráficos de dispersão mostram que há uma correlação positiva entre a idade e a presença de doença cardíaca. Além disso, os boxplots mostram que há diferenças nas distribuições das variáveis entre as classes da variável alvo. Essas informações podem ser úteis para selecionar variáveis relevantes para o modelo e escolher a estratégia de pré-processamento dos dados.

# **4.0 OUTLIERS**
É verificado o número de registros que contêm outliers para cada variável utilizando o método interquartil . Depois de alguns testes percebi que era mais prudente seguir com estes dados no dataset. 

# **5.0 PREPROCESSING**
Os dados são normalizados e escalados. Técncas de correlação são utilizadas para definir as variáveis que farão parte do modelo final,

# **Passo 6: MACHINE LEARNING**
Nesta etapa os dados são divididos e treinados. São calculadas as métricas de precisão,recall e acurácia . Uma matriz de confusão ajuda a avaliar o modelo . Cada modelo é salvo para facilitar o processo de produção em um próximo passo.
