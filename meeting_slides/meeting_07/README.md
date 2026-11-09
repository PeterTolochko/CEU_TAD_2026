# Unsupervised learning

The PDF adapts the 2025 unsupervised learning slides for the 2026 course. The opening on measurement and disciplinary perspectives is shortened. The clustering, topic modelling, validation, and scaling sections retain the original slides and incremental builds. The Dirichlet prior slide corrects a notation inconsistency in the 2025 deck.

The 2025 source is included in the source directory. Retained slides are imported as PDF pages, so their content is not individually editable. The opening, corrected prior slide, and page assembly are in the LaTeX files.

Compile from the repository root with latexmk -pdf meeting_slides/meeting_07/main.tex.

The accompanying unsupervised_ml.ipynb adapts the full 2025 notebook for this class. It uses sotu.csv in this directory, demonstrates k-means and Gensim LDA, and includes a named-entity preprocessing comparison. The notebook lists its Python and spaCy model requirements. The topic-model comparison is optional because it can take several minutes. STM and Wordfish are covered only in the slides.
