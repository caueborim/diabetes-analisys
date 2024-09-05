# diabetes-analysis

## EXPLORAÇÃO DE DADOS

Para este projeto, utilizamos o conjunto de dados de diabetes do *scikit-learn*.  
O conjunto de dados contém 442 instâncias e 10 atributos, que incluem características como idade, sexo, índice de massa corporal (IMC), pressão arterial e várias medidas relacionadas ao colesterol e glicose. A variável alvo é descrita como:

"Uma medida quantitativa da progressão do diabetes um ano após o início."

Os atributos são os seguintes:

* `age` idade
* `sex` gênero
* `bmi` Índice de Massa Corpórea (IMC) - *Body Mass Index* (BMI)
* `bp` pressão arterial média *blood pressure* (bp)
* `s1` colesterol total
* `s2` colesterol LDL
* `s3` colesterol HDL
* `s4` colesterol VLDL
* `s5` triglicerides
* `s6` glicose

Renomeamos as colunas para:

- `Idade`
- `Sexo`
- `IMC`
- `Pressão Arterial`
- `Colesterol Total`
- `Colesterol LDL`
- `Colesterol HDL`
- `Colesterol VLDL`
- `Triglicerídeos`
- `Glicose`

Durante nossa exploração inicial, tratamos valores faltantes introduzindo alguns valores *NaN* artificiais para simular cenários reais. Exploramos diferentes métodos para lidar com esses valores, como preencher valores faltantes e remover linhas ou colunas com dados ausentes. Após isso, restauramos o conjunto de dados original para prosseguir com a análise.

Também processamos a variável categórica "Sexo" convertendo-a em valores numéricos usando técnicas de *label encoding* e *one-hot encoding* para preparar os dados para modelagem.

## ANÁLISE DE DADOS

Iniciamos com uma visão estatística do conjunto de dados, examinando medidas como média, mediana, desvio padrão e quartis para cada variável. As variáveis foram visualizadas através de *boxplots* para identificar valores atípicos e padrões de distribuição.

Usando uma matriz de correlação, identificamos fortes relações entre certas características, como medidas de colesterol e glicose. Uma visualização em *heatmap* destacou essas correlações, o que pode orientar a seleção de variáveis na fase de modelagem.

Realizamos uma análise de gráficos de dispersão entre colesterol, glicose e triglicerídeos para visualizar as relações entre essas características. Histogramas de distribuição e estimativas de densidade também foram gerados para todas as variáveis, revelando padrões na distribuição dos dados. *Boxplots* adicionais ajudaram a destacar a distribuição e possíveis valores atípicos.

## PRÓXIMOS PASSOS

Após concluir a análise exploratória de dados e o pré-processamento, estamos prontos para iniciar a modelagem. Os insights obtidos na exploração dos dados irão guiar a seleção de variáveis e a escolha de modelos, que incluirão técnicas como regressão linear, árvores de decisão e métodos de ensemble.
