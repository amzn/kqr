## CycleKQR: Unsupervised Bidirectional Keyword-Question Rewriting

This repository contains the dataset for the paper ["CycleKQR: Unsupervised Bidirectional Keyword-Question Rewriting"](https://aclanthology.org/2022.emnlp-main.814/) published at EMNLP 2022. 

The data is organized in the following folders:
- **ms-pairs**: Contains keyword-question query pairs collected in the open domain QA scenario, using questions from MS-MARCO and keyword queries from ORCAS;
- **qsp-pairs**: contains keyword-question query pairs collected in the knowledge-based QA scenario, using questions from WebQuestionsSP and keyword queries from ORCAS.

The *ms-pairs* folder is then divided into two subfolders:
- **all**: contains all relevant question-keyword query pairs that were generated automatically using the approach described in Section 5.2.1 in the paper.
- **with_answer**: contains only the question-keyword query pairs that have an answer in the MS-MARCO dataset. Due to the lack of answers in the original MS-MARCO test set, we created our own test set by sampling pairs from the training and dev sets.

Each folder contains three files: train.tsv, dev.tsv, test.tsv, which contain the training, development, and test sets respectively. Each file is in the TSV format, and features the following columns:
- **question_id**: ID of the question in MS-MARCO/WebQuestionsSP
- **question**: Natural language question
- **query**: Keyword query

## Dataset Usage

If you are using this dataset please cite the following paper:

```
@inproceedings{iovine-etal-2022-cyclekqr,
    title = "{C}ycle{KQR}: Unsupervised Bidirectional Keyword-Question Rewriting",
    author = "Iovine, Andrea  and
      Fang, Anjie  and
      Fetahu, Besnik  and
      Zhao, Jie  and
      Rokhlenko, Oleg  and
      Malmasi, Shervin",
    booktitle = "Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing",
    month = dec,
    year = "2022",
    address = "Abu Dhabi, United Arab Emirates",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2022.emnlp-main.814",
    pages = "11875--11886"
}

```

## License Summary

The documentation is made available under the Creative Commons Attribution-ShareAlike 4.0 International License. See the LICENSE file.

The sample code within this documentation is made available under the MIT-0 license. See the LICENSE-SAMPLECODE file.
