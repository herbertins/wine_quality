# Atividade de Algoritmos Supervisionados

Nessa disciplina, aprendemos nossos conhecimentos em algoritmos supervisionados, família de algoritmos que é extremamente importante para o dia a dia de um cientista de dados. Agora iremos validar nosso conhecimento.

## 1. Faça o módulo do [Kaggle Intro to Machine Learning](https://www.kaggle.com/learn/intro-to-machine-learning):
Comprove a finalização do módulo com um print que contenha a data e identificação do aluno.

## Trabalho com base:
Iremos usar a base de dados de vinhos verdes portugueses (nas variantes branco e tinto) que encontra-se disponível no [Kaggle](https://www.kaggle.com/).

> **Para as questões 2-5 usaremos apenas os vinhos do tipo "branco".**

## 2. Faça o download da base
Esta é uma base real, apresentada no artigo:
> P. Cortez, A. Cerdeira, F. Almeida, T. Matos e J. Reis.  
> *Modeling wine preferences by data mining from physicochemical properties*.  
> In Decision Support Systems, Elsevier, 47(4):547-553, 2009.

Ela possui uma variável denominada **"quality"**, uma nota de 0 a 10 que denota a qualidade do vinho.  
Crie uma nova variável chamada **"opinion"**, que será uma variável categórica com os seguintes critérios:
- `0` quando *quality* for menor ou igual a 5.
- `1` caso contrário.

> Desconsidere a variável **quality** para o restante da análise.

## 3. Descrição das variáveis
- Quais são as variáveis presentes na base?  
- Quais são os tipos de variáveis? (discreta, categórica, contínua)  
- Quais são as médias e desvios padrões?  

## 4. Com a base escolhida:

### a. Descreva as etapas necessárias para criar um modelo de classificação eficiente.

### b. Treinamento com Regressão Logística  
Treine um modelo de regressão logística usando validação cruzada estratificada com **k-folds (k=10)**. Calcule para a base de teste:
1. Média e desvio da **acurácia** dos modelos obtidos;  
2. Média e desvio da **precisão** dos modelos obtidos;  
3. Média e desvio do **recall** dos modelos obtidos;  
4. Média e desvio do **F1-score** dos modelos obtidos.  

### c. Treinamento com Árvore de Decisão  
Treine um modelo de árvores de decisão com validação cruzada estratificada com **k-folds (k=10)**. Calcule para a base de teste:
1. Média e desvio da **acurácia** dos modelos obtidos;  
2. Média e desvio da **precisão** dos modelos obtidos;  
3. Média e desvio do **recall** dos modelos obtidos;  
4. Média e desvio do **F1-score** dos modelos obtidos.  

### d. Treinamento com SVM  
Treine um modelo de **SVM** com validação cruzada estratificada com **k-folds (k=10)**. Calcule para a base de teste:
1. Média e desvio da **acurácia** dos modelos obtidos;  
2. Média e desvio da **precisão** dos modelos obtidos;  
3. Média e desvio do **recall** dos modelos obtidos;  
4. Média e desvio do **F1-score** dos modelos obtidos.  

## 5. Escolha do melhor modelo
Com base na questão anterior:
- Qual modelo deve ser escolhido para uma eventual operação?  
- Compare todos os modelos utilizando um gráfico com a **curva ROC média**.  
- Justifique sua escolha.  

## 6. Avaliação com vinhos tintos
Utilizando o melhor modelo escolhido:
- Use os dados de **vinho tinto** presentes na base original.  
- **Faça apenas a inferência** (não treine novamente!).  
- Descubra quantos vinhos são considerados **bons** ou **ruins** usando o mesmo critério utilizado com os vinhos brancos.  
- O modelo funciona da mesma forma para essa nova base? **Justifique.**  
