# TestJudge Generation
Generating judgment for TREC DL test collections using GPT-4 model (gpt-4-32k)

- __final-qrels__: This folder incldues the final merged synthetic qrels for all TREC DL years from 2019 to 2023. There are two different qrel files in this folder:
    - __TestJudge_qrels_pass.txt__ is the file that only includes the synthetic judgments for the query-document pairs created using 10-depth pooling approach form each year submissions.
    - __TestJudge_qrels_pass_withNIST.txt__ is the file that not includes synthetic ones (i.e., __XX__) but also the human judgements for the query-document pairs that judged by NIST assessors.

## Statistics of Qrels

| Factor                 | Synthetic Qrels | Synthetic + Human (NIST) Qrels |
| ---------------------- | --------------- | ------------------------------ |
| TREC (Judged) Queries  | 1,763           | 1,988                          |
| TREC (Initial) Queries | 1,763           | 1,988                          |
| TREC Qrels             | 196,849         | 637,063                        |
| TREC Qrels/Query       | 111.65          | 320.45                         |
| TREC Docs              | 146.8M          | 146.8M                         |
| Irrelevant (0)         | 51,966          | 369,567                        |
| Related (1)            | 63,212          | 126,406                        |
| Highly relevant (2)    | 32,658          | 86,162                         |
| Perfectly relevant (3) | 49,010          | 54,928                         |