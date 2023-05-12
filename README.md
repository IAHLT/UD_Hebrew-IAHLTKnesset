# UD Hebrew-IAHLT

```
האיגוד הישראלי לטכנולוגיות שפת אנוש
الرابطة الإسرائيلية لتكنولوجيا اللغة البشرية
The Israeli Association of Human Language Technologies
https://www.iahlt.org
```

A Universal Dependencies treebank for contemporary Hebrew covering Knesset
protocols. It is released under CC-BY-4.0, see COPYING for details.

## Data set

The Universal Dependencies (UD) Hebrew-IAHLT treebank is a work in
progress. The dataset consists of 2619 annotations of 2619 sentences
(with a total of 45538 tokens annotated, 4382 unique lemmas) for
dependency syntax, part-of-speech, lemmatization and morphological
analysis. The texts were sampled from Knesset protocols.

Note that although the `sentnumber` values are not necessarily consecutive, the
sentences are in fact sorted according to the original order.

## Introduction

The UD Hebrew-IAHLT treebank consists of texts originating from Knesset
protocols. The schema for the UD Hebrew-IAHLT treebank is based on the
conversion of the Hebrew Treebank (HTB) into UD V2 and is checked against the
Universal Dependencies validator as of UD release V2.8.

The HTB was initially converted automatically, then a subset of the converted
data was manually validated and adopted as a gold standard for training the
model for UD parsing used in Hebrew-IAHLT.

The parsed data has been manually edited to correct parsing errors. Quality
assurance (QA) scripts were used to apply corrections following updates in the
schema. All sentences in this release pass level-5 validation of the
Universal Dependencies validator.

## Metadata fields

  * fields for technical use:

    * `sent_id`    - a unique identifier for the tree within this release
    * `text`       - the (Hebrew) text of the original sentence
    * `url`        - the link for the source entry/article
    * `source`     - the source of the sentence
    * `doc_id`     - a unique identifier for the source document
    * `protocol`   - the source protocol file
    * `parnumber`  - the paragraph sequence number within the source document
    * `sentnumber` - the sentence sequence number within the source paragraph

## Guidelines

The annotation guidelines can be found at
https://github.com/ivrit/IAHLT-HTB-GUIDELINES

## Acknowledgments

We would like to thank all the people who contributed to this corpus:

Emmanuelle Ko
Israel Landau
Nick Howell
Noam Ordan
Omer Strass
Shira Wigderson
Yifat Ben Moshe

