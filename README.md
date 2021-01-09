# TP2EAC
[Version English](README-en.md)

<img align="left" src="https://media.giphy.com/media/ADgfsbHcS62Jy/giphy.gif" width="200" height="200" /> 

O TP2EAC - É um projeto realizado para uma disciplina do 4º ano do Mestrado em Engenharia Informática, do perfil de Sistemas Inteligentes. Seu objetivo é conseguir um modelo de classificação a produzir bons resultados. Neste trabalho temos os seguintes problemas: Preparação e análise de um dataset relativo às características de funcionários de múltiplas empresas, no intuito de prever o nível salarial anual do indivíduo.
Este projeto baseia-se num conjunto de casos de estudo, os quais apresentadam informações referentes aos funcionários de empresas espalhadas pelo mundo, as quais possuem
 multiplas características sobre o indivíduo.







## Sobre a Equipa 
A equipa desenvolvedora é composta por 4 alunos da Universidade do Minho, Braga, Portugal.

* [Daniel Assunção](https://github.com/guiyrt)
* [Diogo Ferreira ](https://github.com/DiogoFerreira99)
* [Leonardo Silva](https://github.com/leoproject)
* [Pedro Pinheiro](https://github.com/Pinheiro9655)

## Dataset
O dataset fornecido para trabalhar neste problema, encontra-se no diretório [recursos](resources/) deste repositório. Nele contêm :

1. training.csv, este apresenta os casos de estudo a serem usados exclusivamente para o treino dos modelos;

2. test.csv, este apresenta os registos para validação dos modelos;

3. attribute_info.docx, neste documento é apresentado alguns detalhes relativamente do conjunto de atributos presentes nos datasets. Contendo 14 atributos e uma target de classificação que é salario anual.
   

# Metodologia de Desenvolvimento:
<img align="right" src="https://media.giphy.com/media/l4pTsNgkamxfk2ZLq/giphy.gif" width="200" height="150"/> 
A metodologia adotada pela equipa é a CRISP-DM (Cross Industry Standard Process for Data Mining) consiste num ciclo composto por 6 fases.

1. **Estudo do Negócio:** Esta fase inicial foi o estudo do dataset perceber qual objetivo e atributos presentes no dataset;

2. **Analise dos Dados:** Esta fase foi concretizada pelo estudo sobre os dados e as features, presente no dataset de treino em especial. Esta fase pode ser encontrada no [notebook da analise dos dados](../TP2EAC/data_analysis/TP2EAC_AnaliseDados.ipynb);

3. **Preparação dos Dados:** Nesta fase foi confeccionado um [notebook](../TP2EAC/Data_Preparation/TP2EAC_Preparação_dos_Dados.ipynb) o qual teve como  [input](../TP2EAC/Data_Preparation/Input) os datasets de treino e teste, forneceidos pela equipa docente. 
   
   A seguir foi verificado missing values, correlações, feature engineering entre outras técnicas. O [output](../TP2EAC/Data_Preparation/Output) deste notebook foi geração de novos datasets. Sendo eles de treino e teste, com o tratamento dos dados e outros para além do tratamento dos dados contêm a normalização. Resultando em 4 datasets ( 2 de treino e 2 de teste). Estes serão usados na fase posterior;

4. **Modelação dos Algoritmos:** Para esta fase para padronização  do flow de desenvolvimento dos modelos, fizemos um [notebook padrão](models/reglog/TP2EAC-STANDARD-MODEL.ipynb) usando o algoritmo de regressão logistica. O qual o output é o próprio modelo de classificação do algoritmo em uso.  Uma vez guardado todos os modelos gerados pelos algoritmos escolhidos iremos para próxima fase;

5. **Avaliação dos Modelos:** Esta fase tem-se o [notebook de avaliação](benchmark/TP2AEC-AVALIACAO.ipynb) com todos os modelos para possamos visualizar e comparar os resultados dos modelos usando os datasets de teste seja o com normalização ou não. Uma vez decidido qual é o melhor modelo de classificação para este problema este passará para próxima fase;
   
6. **Desenvolvimento:** Esta fase é colocar o modelo escolhido na fase anterior em produção, para isso foi utilizado o Heroku e criado uma API para aceder ao modelo com Flask, o qual encontra-se num [repositório](https://github.com/leoproject/appModel) a parte. Caso deseje testar a api com o modelo em produção temos um notebook para isso na diretória [testApi](testApi/Testar%20Modelo.ipynb).




## Considerações Finais
Com a resolução deste trabalho, o grupo desenvolveu capacidades para criar e treinar modelos de classificação usando uma grande variedade de algoritmos diferentes. Também evoluímos no que toca á análise e preparação de dados, que são duas fases importantes para qualquer desenvolvimento de um método de classificação e previsão.

Posto isto, concluímos que o melhor modelo treinado pelo nosso grupo, se analisarmos só pela acurácia dos modelos, é o que implementa o algoritmo K-Nearest-Neighbors. No entanto, o que o grupo escolheria para a fase de Desenvolvimento, por critérios estabelecidos anteriormente, escolheríamos o modelo que implementa o algoritmo de Regressão Logística, utilizando o método criado pelo nosso grupo.
