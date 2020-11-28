# TP2EAC


<img align="left" src="https://media.giphy.com/media/ADgfsbHcS62Jy/giphy.gif" width="200" height="200" /> 

TP2AEC This project was carried out on behalf of a discipline from our 4th year of the Master in Intelligent Systems. Its objective is to achieve a model that is viable enough to produce good results in the following problem: Preparation and analysis of a dataset related to the characteristics of employees of multiple companies, as a way of predicting the individual's annual salary level.
This project is based on a set of case studies presenting information regarding employees of companies around the world, where multiple
characteristics about the individual as a way of predicting his annual salary class.


   


## About Team
The developer team is four master students from University of Minho, Braga, Portugal.

* [Daniel Assunção](https://github.com/)
* [Diogo Ferreira ](https://github.com/DiogoFerreira99)
* [Leonardo Silva](https://github.com/leoproject)
* [Pedro Pinheiro](https://github.com/Pinheiro9655)

## Dataset
The dataset provided to work on the proposed problem is found in the [resources] (resources /) directory which contain:

1. training.csv, which presents the case studies to be applied exclusively for the training of the predictive model;

2. test.csv, which presents the case studies to be applied exclusively for the analysis and validation of the predictive model;

3. attribute_info.docx, where details about the attributes of the given data set are presented. Containing 14 attributes and 1 annual salary classification target information if the employee receives 50 thousand per year.



## Models

<img align="right" src="https://media.giphy.com/media/hTOOnpWeFOnYvkYTwo/giphy.gif" width="200" height="150"/> 

Here we discuss the models created by our group. All notebooks with their respective model follow the pipeline exposed in the standard notebook, [TP2EAC_Standard_Notebook.ipynb](models/TP2EAC_Standard_Notebook.ipynb), and are displayed on the following table:



Link to model| Short description | Articles About| 
--- | --- | --- | 
[TP2EAC_KNN](models/knn/) | | [Artigo]()
[TP2EAC_CBR](models/cbr/) | | [Artigo]()
[TP2EAC_SVM](models/svm/) | |[Artigo]()
[TP2EAC_ANN](models/ann/)|  |[Artigo]()
[TP2EAC_Regressão Logística](models/reglog/)|  | [Artigo]()
[TP2EAC_Naive Bayes](models/naive/)| | [Artigo]()


## Conclusion


|             | Accuracy | Precision | Precision | Recall   | Recall  |            
|:-----------:|:--------:|:--------:|:---------:|:---------:|:--------:|
|             |          | > 50k/Y  |   <=50k/Y |  > 50k/Y  | <=50k/Y  |                 
|    KNN      |          |          |           |           |          |
|    CBR      |          |          |           |           |          |
|    SVM      |          |          |           |           |          | 
|    ANN      |          |          |           |           |          |
|   Reg Log   |          |          |           |           |          |   
| Naive Bayes |          |          |           |           |          | 



