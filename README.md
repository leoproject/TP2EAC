# TP2EAC
[Version English](README-en.md)

<img align="left" src="https://media.giphy.com/media/ADgfsbHcS62Jy/giphy.gif" width="200" height="200" /> 

TP2AEC Este projeto foi realizado em nome de uma disciplina do nosso 4º ano do Mestrado em Sistemas Inteligentes. Seu objetivo é conseguir um modelo viável o suficiente para produzir bons resultados no seguinte problema: Preparação e análise de um dataset relativo às características de funcionários de múltiplas empresas, como forma de prever o nível salarial anual do indivíduo.
Este projeto baseia-se num conjunto de casos de estudo apresentando informações referentes a funcionários de empresas espalhadas pelo mundo, onde são analisadas múltiplas
características sobre o indivíduo como forma de prever a sua classe salarial anual.






## Sobre a Equipa 
A equipa desenvolvedora é composta por 4 alunos da Universidade do Minho, Braga, Portugal.

* [Daniel Assunção](https://github.com/guiyrt)
* [Diogo Ferreira ](https://github.com/DiogoFerreira99)
* [Leonardo Silva](https://github.com/leoproject)
* [Pedro Pinheiro](https://github.com/Pinheiro9655)

## Dataset
O dataset fornecido para trabalhar acerca do problema proposto encontra-se no diretório [recursos](resources/) que contêm :

 1. training.csv, onde se apresentam os casos de estudo a serem aplicados exclusivamente para o treino do modelo preditivo;

1. test.csv, onde se apresentam os casos de estudo a serem aplicados exclusivamente para a análise e validação do modelo preditivo;

2. attribute_info.docx, onde são apresentados alguns detalhes relativamente aos atributos do conjunto de dados fornecidos. Contendo 14 atributos e uma target de classificação salario anual maior que 50k por ano.

# Processo da Geração dos Modelos:
Para a geração dos modelos foi realizado um pipeline da seguinte forma :

1. **Analise dos Dados:** processo ao qual foi realizado um estudo sobre os dados e as features presente no dataset de treino;

2. **Preparação dos Dados:** aqui o processo foi dar o [input](../TP2EAC/Data_Preparation/Input/) do dataset de treino e teste, preparar os dados e verificar correlações com a target produzindo no final um [output dos datasets](../TP2EAC/Data_Preparation/Output/) (de treino e teste ) com tratamento dos dados e outros dois que para além do tratamento os dados foram normalizados. 

3. **Modelação dos Algoritmos:** para a titulo depadronização para o flow do desenvolvimento dos modelos, fizemos um [notebook padrão](models/reglog/TP2EAC-STANDARD-MODEL.ipynb) usando o algoritmo de regressão logistica. O output dos notebook dos modelos é o proprio modelo do algoritmo guardado para caso for escolhido ser colocado em produção. 



## Modelos

<img align="right" src="https://media.giphy.com/media/l4pTsNgkamxfk2ZLq/giphy.gif" width="150" height="150"/> 

Aqui nos discutiremos os modelos criados pelo grupo. Todos os notebooks com seus respectivos modelos e descição estãonas suas respectivas diretórias, seguindo o pipeline exposto neste notebook padrão [TP2EAC_Standard_Notebook.ipynb](models/reglog/TP2EAC-STANDARD-MODEL.ipynb), demonstrado na tabela abaixo:



Link do modelo| Breve Descrição | Artigo sobre o Modelo| 
--- | --- | --- | 
[TP2EAC_KNN](models/knn/) | | [Artigo]()
[TP2EAC_CBR](models/cbr/) | | [Artigo]()
[TP2EAC_SVM](models/svm/) | |[Artigo]()
[TP2EAC_ANN](models/ann/)|  |[Artigo]()
[TP2EAC_Regressão Logística](models/reglog/)|  | [Artigo]()
[TP2EAC_Naive Bayes](models/naive/)| | [Artigo]()



## Resultados


|             | Accuracy | Precision | Precision | Recall   | Recall  |            
|:-----------:|:--------:|:--------:|:---------:|:---------:|:--------:|
|             |          | > 50k/Y  |   <=50k/Y |  > 50k/Y  | <=50k/Y  |                 
|    KNN      |          |          |           |           |          |
|    CBR      |          |          |           |           |          |
|    SVM      |          |          |           |           |          | 
|    ANN      |          |          |           |           |          |
|   Reg Log   |          |          |           |           |          |   
| Naive Bayes |          |          |           |           |          | 



## Considerações Finais