# acl2022-impli

The <font color="#1560BD" style="font-family:'Inconsolata'">IMPLI</font> Dataset

This repository contains the data collected as part of the <font color="#1560BD" style="font-family:'Inconsolata'">IMPLI</font> dataset, to be published at ACL 2022.

This dataset consists of both semi-supervised and gold annotated pairs. These pairs consist of a literal sentence and a figurative counterpart. The pairs are designed to be either entailing or non-entailing, providing a rich, diverse set of paired data to explore figurative language.

The <u>idioms</u> and <u>metaphors</u> folders each contain files of paired sentences. These are grouped by the type of collection used, the dataset, and the intended entailment relation. Each is in .tsv format, with the first column being the context and the second the hypothesis (some also contain scores for metaphoricity from the original datasets as the third column).

<i>Collection Types</i>

<ul>
<li><b>adversarial_definition</b>: Annotators created hand-crafted adversarial definitions of idioms, which were then slotted into relevant contexts, yielding non-entailing pairs.</li>
<li><b>fig_context</b>: Dictionary definitions were substituted into figurative contexts, yielding entailment pairs.</li>
<li><b>lit_context</b>: Dictionary definitions were substituted into literal contexts, yielding non-entailment pairs.</li>
<li><b>replacement</b>: Annotators generated literal paraphrases for metaphoric constructions, which were replaced into figuraitve contexts, yielding entailments</li>
<li><b>manual</b>: Annotators manually wrote entailing and non-entailing pairs.</li>
</ul>

<i>Datasets</i>

For the automatic replacements, we started with sentences from other datasets, replacing key components to yield pairs.

<ul>
<li><b>magpie</b>: <a href="https://aclanthology.org/2020.lrec-1.35.pdf"> The MAGPIE idiom dataset</a></li>
<li><b>pie</b>: <a href="https://arxiv.org/abs/2105.03280"> The PIE idiom dataset</a></li>
<li><b>semeval</b>: <a href="https://aclanthology.org/S13-2007/"> The SemEval idiom dataset (Task 5)</a></li>
</ul>

<i>Relations</i>

Files ending in <b>_e</b>.tsv are intended to contain entailing relations between the context and hypothesis; files ending in <b>_ne</b>.tsv are intended to contain non-entailing pairs.

For questions/comments/suggestions, please contact Kevin Stowe:
```kevincstowe@gmail.com```

Disclaimer
```
This repository contains experimental software and is published for the sole purpose of giving additional background details on the respective publication. 
```

Citation

If you use the  <font color="#1560BD" style="font-family:'Inconsolata'">IMPLI</font> dataset, please cite the following publication, to appear at ACL 2022:
```bibtex
@inproceedings{stowe-2022,
    title = "IMPLI: Investigating NLI Models' Performance on Figurative Language",
    author = "Stowe, Kevin and Utama, Prasetya Ajie, and Gurevytch, Iryna",
    booktitle = "Proceedings of the 2022 Conference for the Association of Computational Linguistics",
    month = "06",
    year = "2022",
    publisher = "Association for Computational Linguistics",
    url = "tbd",
}
```