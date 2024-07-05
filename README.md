<h1 align="left">
<img style="vertical-align:middle" width="50px" height="40px" src="DeepJudge-logo.png" /> DL-LLM
</h1>

# DL-LLM
TREC Deep Learning Full Synthetic Test Collection

## Prompt
`prompt.txt` contains the prompt that we used for the relevance judgment generation. This prompt template is inspired by Thomas et al. [1] recent paper on search prefenrce predictions using LLMs.

## Qrels
The qrels files can be found in the `./qrels/` folder. The qrels folder includes two qrel files. The files are with the same format of TREC DL: tab-seprated and similir columns:

> qid 0 docid score

- __DL-LLM_qrels_pass.txt__: This is the full synthetic qrel file.
- __DL-LLM_qrels_pass_withHuman.txt__: This qrel includes synthetic qrels based on our depth-10 pooling synthetic qrel construction and human qrels from all 5 years labelled by NIST assessors.

## Reference
[1] Paul Thomas, Seth Spielman, Nick Craswell, and Bhaskar Mitra. "Large language models can accurately predict searcher preferences." arXiv preprint arXiv:2309.10621 (2023).

## Acknowledgments
This research is supported by the Engineering and Physical Sciences Research Council [EP/S021566/1] and the EPSRC Fellowship titled "Task Based Information Retrieval" [EP/P024289/1].
