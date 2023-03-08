# LeCoNTra

We present LeCoNTra, a learner corpus consisting of English-to-Dutch news translations enriched with translation process data. Three students of a Master’s programme in Translation were asked to translate 50 different English journalistic texts of approximately 250 tokens each. Because we also collected translation process data in the form of keystroke logging, our dataset can be used as part of different research strands such as translation process research, learner corpus research, and corpus-based translation studies. Reference translations, without process data, are also included. The data has been manually segmented and tokenized, and manually aligned at both segment and word level, leading to a high-quality corpus with token-level process data. The data is freely accessible via the Translation Process Research DataBase and GitHub, which emphasises our commitment of distributing our dataset. The tool that was built for manual sentence segmentation and tokenization, [Mantis](https://github.com/BramVanroy/mantis), is also available as an open-source aid for data processing.


## Metadata

Metadata was collected with [TICQ](https://traco.uni-mainz.de/ticq/). Identifiable columns such as IP addresses and initials have been removed. You will find that there is a P04 in the data who is not present in the metadata. As the paper describes, P04 are reference translations. There is no process data for P04 (only a final translation and product-related metrics). It is unlikely that all translations were made by the same person, so be vigilant when using P04 for analyses as it is a collection of reference translations, likely by different translators.

## Citation

Vanroy, B. and Macken, L. (2022). [LeConTra: A Learner Corpus of English-to-Dutch News Translation](https://aclanthology.org/2022.lrec-1.192). In *Proceedings of the Language Resources and Evaluation Conference*, pages 1807-1816, Marseille, France. European Language Resources Association.

```bibtex
@InProceedings{vanroy-macken:2022:LREC,
  author    = {Vanroy, Bram  and  Macken, Lieve},
  title     = {{LeConTra}: A Learner Corpus of English-to-Dutch News Translation},
  booktitle = {Proceedings of the Language Resources and Evaluation Conference},
  month     = {June},
  year      = {2022},
  address   = {Marseille, France},
  publisher = {European Language Resources Association},
  pages     = {1807--1816},
  abstract  = {We present {LeConTra}, a learner corpus consisting of English-to-Dutch news translations enriched with translation process data. Three students of a Master's programme in Translation were asked to translate 50 different English journalistic texts of approximately 250 tokens each. Because we also collected translation process data in the form of keystroke logging, our dataset can be used as part of different research strands such as translation process research, learner corpus research, and corpus-based translation studies. Reference translations, without process data, are also included. The data has been manually segmented and tokenized, and manually aligned at both segment and word level, leading to a high-quality corpus with token-level process data. The data is freely accessible via the Translation Process Research DataBase, which emphasises our commitment of distributing our dataset. The tool that was built for manual sentence segmentation and tokenization, Mantis, is also available as an open-source aid for data processing.},
  url       = {https://aclanthology.org/2022.lrec-1.192}
}

```

## Erratum

In the paper, the number of tokens column in the Appendix is incorrect. The cause of this is not immediately clear but may have to do with changes in the TPR-DB table generation, and/or white-space and newline handling. To get the right number of tokens per text, please consider the number of rows in the *.st tables (source tokens) in this repository. They show one row per token.
