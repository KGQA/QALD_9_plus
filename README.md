# QALD+ Dataset Description

QALD+ is the dataset for Knowledge Graph Question Answering (KGQA) based on well-known [QALD-9](https://github.com/ag-sc/QALD/tree/master/9/data).

QALD+ enables to train and test KGQA systems over DBpedia and Wikidata using questions in 8 different languages.

Some of the questions have several alternative writings in particular languages which enables to evaluate the robustness of KGQA systems and train paraphrasing models.

As the questions' translations were provided by native speakers, they are considered as "gold standard", therefore, machine translation tools can be trained and evaluated on the dataset.

# Dataset Statistics

|       | en  | de  | ru   | lt | uk  | be | arm | fr | DBpedia | Wikidata | # questions |
|-------|-----|-----|------|----|-----|----|-----|----|---------|----------|-------------|
| Train | 408 | 545 | 1294 | 63 | 262 | 80 |  80 | 80 |     408 |      373 |         408 |
| Test  | 150 | 177 |  378 | 28 | 170 | 12 |  20 | 20 |     150 |      137 |         150 |

Given the numbers, it is obvious that some of the languages are covered more than once \ie there is more than one translation for a particular question.
For example, there are 1294 Russian translations available while only 408 unique questions exist in the training subset (\ie 3.2 Russian translations per one question).
This enables the dataset users to address also the paraphrasing task.

# Evaluation

We used [GERBIL]() system for the evaluation of the dataset. For the comparison, Macro F1 metric was used. The detailed information for the experiments is available at the individual link (click the value in the cells).

## Wikidata

### QAnswer

|     | en | de | ru | fr |
|-----|----|----|----|----|
|Test |[0.00](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110010001)|[0.00](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110010002)|[0.00](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110010003)|[0.00](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110010004)|
|Train|[0.00](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110010007)|[0.00](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110080002)|[0.00](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110080003)|[0.00](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110080004)|

### DeepPavlov


|     | en | ru |
|-----|----|----|
|Test |[0.00](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110080010)||
|Train|||

### Platypus

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
