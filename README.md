# QALD+ Dataset Description

QALD+ is the dataset for Knowledge Graph Question Answering (KGQA) based on well-known [QALD-9](https://github.com/ag-sc/QALD/tree/master/9/data).

QALD+ enables to train and test KGQA systems over DBpedia and Wikidata using questions in 8 different languages.

Some of the questions have several alternative writings in particular languages which enables to evaluate the robustness of KGQA systems and train paraphrasing models.

As the questions' translations were provided by native speakers, they are considered as "gold standard", therefore, machine translation tools can be trained and evaluated on the dataset.

# Dataset Statistics

|       | en  | de  | ru   | lt | uk  | be | hy | fr | DBpedia | Wikidata | # questions |
|-------|-----|-----|------|----|-----|----|-----|----|---------|----------|-------------|
| Train | 408 | 545 | 1294 | 63 | 262 | 80 |  80 | 80 |     408 |      371 |         408 |
| Test  | 150 | 177 |  378 | 28 | 170 | 12 |  20 | 20 |     150 |      136 |         150 |

Given the numbers, it is obvious that some of the languages are covered more than once \ie there is more than one translation for a particular question.
For example, there are 1294 Russian translations available while only 408 unique questions exist in the training subset (\ie 3.2 Russian translations per one question).
This enables the dataset users to address also the paraphrasing task.

# Evaluation

We used [GERBIL]() system for the evaluation of the dataset.The detailed information for the experiments is available at the individual link (click the value in the cells).

## Wikidata

### QAnswer

|     | en | de | ru | fr |
|-----|----|----|----|----|
|Test |[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110010001)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110210028)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202111120007)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110210030)|
|Train|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110010007)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110080002)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110080003)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110080004)|

### DeepPavlov

|     | en | ru |
|-----|----|----|
|Test |[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110080010)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202111120004)|
|Train|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110090001)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110110000)|

### Platypus

|     | en | fr |
|-----|----|----|
|Test |[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110110004)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110110005)|
|Train|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110110006)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110120000)|


## DBpedia

### QAnswer

|     | en | de | ru | fr |
|-----|----|----|----|----|
|Test |[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110120004)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110120005)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110130000)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110130001)|
|Train|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110130002)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110140000)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110150000)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110150001)|

# Cite

To Be Done

# Licence

Shield: [![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
