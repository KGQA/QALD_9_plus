# QALD-9-Plus Dataset Description

QALD-9-Plus is the dataset for Knowledge Graph Question Answering (KGQA) based on well-known [QALD-9](https://github.com/ag-sc/QALD/tree/master/9/data).

QALD-9-Plus enables to train and test KGQA systems over DBpedia and Wikidata using questions in 9 different languages: English, German, Russian, French, Armenian, Belarusian, Lithuanian, Bashkir, and Ukrainian.

Some of the questions have several alternative writings in particular languages which enables to evaluate the robustness of KGQA systems and train paraphrasing models.

As the questions' translations were provided by native speakers, they are considered as "gold standard", therefore, machine translation tools can be trained and evaluated on the dataset.

# Dataset Statistics

|       |  en |  de | fr |  ru  |  uk |  lt |  be |  ba | hy | # questions DBpedia | # questions Wikidata |
|-------|:---:|:---:|:--:|:----:|:---:|:---:|:---:|:---:|:--:|:-----------:|:-----------:|
| Train | 408 | 543 | 260 | 1203 | 447 | 468 | 441 | 284 | 80 |     408     |     371     |
| Test  | 150 | 176 | 26 |  348 | 176 | 186 | 155 | 117 | 20 |     150     |     136     |

Given the numbers, it is obvious that some of the languages are covered more than once i.e., there is more than one translation for a particular question.
For example, there are 1203 Russian translations available while only 408 unique questions exist in the training subset (i.e., 2.9 Russian translations per one question).
The availability of such parallel corpora enables the researchers, developers and other dataset users to address the paraphrasing task.

# Evaluation

We used [GERBIL](https://github.com/dice-group/gerbil/) system for the evaluation of the dataset. The detailed information for the experiments is available at the individual link (click the value in the cells).

## Wikidata

### QAnswer

|     | en | de | ru | fr |
|-----|----|----|----|----|
|Test |[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110010001)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180000)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180001)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180002)|
|Train|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110010007)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180006)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180007)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180008)|

### DeepPavlov

|     | en | ru |
|-----|----|----|
|Test |[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110080010)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180003)|
|Train|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110090001)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180009)|

### Platypus

|     | en | fr |
|-----|----|----|
|Test |[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110110004)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180004)|
|Train|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110110006)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180010)|


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
