# TP2EAC
[Version English](README.md)

<img align="left" src="https://media.giphy.com/media/ADgfsbHcS62Jy/giphy.gif" width="200" height="200" /> 

TP2AEC Este projeto foi realizado em nome de uma disciplina do nosso 4º ano do Mestrado em Sistemas Inteligentes. Seu objetivo é conseguir um modelo viável o suficiente para produzir bons resultados no seguinte problema: Preparação e análise de um dataset relativo às características de funcionários de múltiplas empresas, como forma de prever o nível salarial anual do indivíduo.
Este projeto baseia-se num conjunto de casos de estudo apresentando informações referentes a funcionários de empresas espalhadas pelo mundo, onde são analisadas múltiplas
características sobre o indivíduo como forma de prever a sua classe salarial anual.






## Sobre a Equipa 
A equipa desenvolvedora é composta por 4 alunos da Universidade do Minho, Braga, Portugal.

* [Daniel Assunção](https://github.com/)
* [Diogo Ferreira ](https://github.com/DiogoFerreira99)
* [Leonardo Silva](https://github.com/leoproject)
* [Pedro Pinheiro](https://github.com/Pinheiro9655)

## Dataset
O dataset fornecido para trabalhar acerca do problema proposto encontra-se no diretório [recursos](resources/) que contêm :

 1. training.csv, onde se apresentam os casos de estudo a serem aplicados exclusivamente para o treino do modelo preditivo;

1. test.csv, onde se apresentam os casos de estudo a serem aplicados exclusivamente para a análise e validação do modelo preditivo;

2. attribute_info.docx, onde são apresentados alguns detalhes relativamente aos atributos do conjunto de dados fornecidos. Contendo 14 atributos e uma target de classificação salario anual maior que 50k por ano.



## Modelos

<img align="right" src="https://media.giphy.com/media/hTOOnpWeFOnYvkYTwo/giphy.gif" width="150" height="150"/> 

Aqui nos discutiremos os modelos criados pelo grupo. Todos os notebooks com seus respectivos modelos e descição estãonas suas respectivas diretórias, seguindo o pipeline exposto neste notebook padrão [TP2EAC_Standard_Notebook.ipynb](models/TP2EAC_Standard_Notebook.ipynb), demonstrado na tabela abaixo:



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