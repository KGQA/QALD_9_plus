# QALD-9-plus Dataset Description

QALD-9-plus is the dataset for Knowledge Graph Question Answering (KGQA) based on well-known [QALD-9](https://github.com/ag-sc/QALD/tree/master/9/data).

QALD-9-plus enables to train and test KGQA systems over DBpedia and Wikidata using questions in 10 different languages: English, German, Russian, French, Spanish, Armenian, Belarusian, Lithuanian, Bashkir, and Ukrainian.

Some of the questions have several alternative writings in particular languages which enables to evaluate the robustness of KGQA systems and train paraphrasing models.

As the questions' translations were provided by native speakers, they are considered as "gold standard", therefore, machine translation tools can be trained and evaluated on the dataset.

# Dataset Statistics

|       |  en |  de | fr |  ru  |  uk |  lt |  be |  ba | hy | es | # questions DBpedia | # questions Wikidata |
|-------|:---:|:---:|:--:|:----:|:---:|:---:|:---:|:---:|:--:|:--:|:-----------:|:-----------:|
| Train | 408 | 543 | 260 | 1203 | 447 | 468 | 441 | 284 | 80 | 408 |     408     |     371     |
| Test  | 150 | 176 | 26 |  348 | 176 | 186 | 155 | 117 | 20 | 150 |     150     |     136     |

Given the numbers, it is obvious that some of the languages are covered more than once i.e., there is more than one translation for a particular question.
For example, there are 1203 Russian translations available while only 408 unique questions exist in the training subset (i.e., 2.9 Russian translations per one question).
The availability of such parallel corpora enables the researchers, developers and other dataset users to address the paraphrasing task.

# Evaluation

We used [GERBIL](https://github.com/dice-group/gerbil/) system for the evaluation of the dataset. The detailed information for the experiments is available at the individual link (click the value in the cells).

## Wikidata

### QAnswer

|     | en | de | ru | fr | es |
|-----|----|----|----|----|----|
|Test |[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110010001)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180000)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180001)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180002)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202211180000)|
|Train|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110010007)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180006)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180007)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112180008)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202211210000)|

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
|Test |[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110120004)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190000)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190001)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190002)|
|Train|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202110130002)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190003)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190004)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190005)|

## Wikidata Original Translations

### QAnswer

|     | de | ru | fr |
|-----|----|----|----|
|Test |[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190006)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190007)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190008)|
|Train|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190009)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190010)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190011)|

### DeepPavlov

|     | ru |
|-----|----|
|Test |[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190012)|
|Train|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190014)|

### Platypus

|     | fr |
|-----|----|
|Test |[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190013)|
|Train|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190015)|

## DBpedia Original Translations

### QAnswer

|     | de | ru | fr |
|-----|----|----|----|
|Test |[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190016)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190017)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190018)|
|Train|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190019)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190020)|[link](http://gerbil-qa.aksw.org/gerbil/experiment?id=202112190021)|

# Cite

```bibtex
@inproceedings{perevalov2022qald9plus,
      author={Perevalov, Aleksandr and Diefenbach, Dennis and Usbeck, Ricardo and Both, Andreas},
      booktitle={2022 IEEE 16th International Conference on Semantic Computing (ICSC)},
      title={QALD-9-plus: A Multilingual Dataset for Question Answering over DBpedia and Wikidata Translated by Native Speakers},
      year={2022},
      pages={229-234},
      doi={10.1109/ICSC52841.2022.00045}
}
```

# Useful Links

* ArXiv [link](https://arxiv.org/abs/2202.00120)
* Papers with Code: [Paper](https://paperswithcode.com/paper/qald-9-plus-a-multilingual-dataset-for-1), [Dataset](https://paperswithcode.com/dataset/qald-9-plus)
* Video presentation on YouTube: https://youtu.be/W1w7CJTV48c
* Presentation [slides](https://drive.google.com/file/d/1cDphq4DeSiZr-WBvdwu34rcxQ0aP4q95/view?usp=sharing)
* Google Colab [notebook](https://colab.research.google.com/drive/1eWsQoIaeT9_vii1v3PVU04Rms4EoyLAh?usp=sharing)

# Licence [![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg


# Dataset Metadata

The following table is necessary for this dataset to be indexed by search
engines such as <a href="https://g.co/datasetsearch">Google Dataset Search</a>.
<div itemscope itemtype="http://schema.org/Dataset">
<table>
  <tr>
    <th>property</th>
    <th>value</th>
  </tr>
  <tr>
    <td>name</td>
    <td><code itemprop="name">QALD-9-plus: A Multilingual Dataset for Question Answering over DBpedia and Wikidata Translated by Native Speakers</code></td>
  </tr>
  <tr>
    <td>alternateName</td>
    <td><code itemprop="alternateName">QALD-9-plus</code></td>
  </tr>
  <tr>
    <td>url</td>
    <td><code itemprop="url">https://github.com/Perevalov/qald_9_plus/tree/main/data</code></td>
  </tr>
  <tr>
    <td>description</td>
    <td><code itemprop="description">QALD-9-Plus is the dataset for Knowledge Graph Question Answering (KGQA) based on well-known QALD-9.<br/>
QALD-9-Plus enables to train and test KGQA systems over DBpedia and Wikidata using questions in 9 different languages: English, German, Russian, French, Armenian, Belarusian, Lithuanian, Bashkir, and Ukrainian.<br/>
Some of the questions have several alternative writings in particular languages which enables to evaluate the robustness of KGQA systems and train paraphrasing models.<br/>
As the questions' translations were provided by native speakers, they are considered as "gold standard", therefore, machine translation tools can be trained and evaluated on the dataset.</code></td>
  </tr>
  <tr>
    <td>license</td>
    <td>
      <div itemscope itemtype="http://schema.org/CreativeWork" itemprop="license">
        <table>
          <tr>
            <th>property</th>
            <th>value</th>
          </tr>
          <tr>
            <td>name</td>
            <td><code itemprop="name">CC-BY-4.0</code></td>
          </tr>
          <tr>
            <td>url</td>
            <td><code itemprop="url">https://creativecommons.org/licenses/by/4.0/</code></td>
          </tr>
        </table>
      </div>
    </td>
  </tr>
  <tr>
    <td>citation</td>
    <td><code itemprop="citation">Perevalov, Aleksandr, Diefenbach, Diefenback, Usbeck, Ricardo, Both, Andreas: QALD-9-plus: A multilingual dataset for question answering over DBpedia and Wikidata translated by native speakers. In: 2022 IEEE 16th International Conference on Semantic Computing (ICSC). IEEE (2022)</code></td>
  </tr>
</table>
</div>
