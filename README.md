# Portuguese BERT Paraphrase Evaluation

A compact NLP experiment that creates Portuguese paraphrases using a masked
language model and evaluates their semantic similarity using two independent
transformer-based metrics.

## Pipeline

1. Read Portuguese source sentences from `frases.txt`.
2. Select eligible words in each sentence.
3. Replace selected words with BERT's mask token.
4. Generate replacements using `neuralmind/bert-base-portuguese-cased`.
5. Evaluate each generated sentence with:
   - **BERTScore F1**
   - **SBERT cosine similarity** using
     `paraphrase-multilingual-MiniLM-L12-v2`.
6. Produce a comparative table with source sentence, generated paraphrase and
   both semantic scores.

## Authors

- **Gustavo Fraiz**
- **Gustavo Albiero**

These names are preserved from the original notebook.

## Repository structure

```text
.
├── README.md
├── requirements.txt
├── notebooks/
│   └── paraphrase_evaluation.ipynb
└── data/
    └── README.md
```

No license is included by default.
