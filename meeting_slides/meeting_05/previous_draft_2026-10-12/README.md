# Class 5: Supervised text classification

The lecture continues the Class 4 Rotten Tomatoes exercise and connects the Federalist multinomial model to Naive Bayes. The classifiers are multinomial Naive Bayes on counts, regularized logistic regression on TF-IDF, and a linear SVM on the same unigram TF-IDF representation.

The notebook reads the original sentence-polarity files from `../meeting_04/data/rotten_tomatoes/`. It uses a seeded stratified split (approximately 60% training, 20% validation, 20% test), selects model settings on validation F1, refits on combined development data, and compares all methods on the same test snippets.

Requirements: Python with NumPy, Matplotlib, scikit-learn, and Jupyter. No network connection is needed. Run the notebook from this directory or the repository root.

The notebook exports the figures and TeX result tables used by the slides. Rerun it before rebuilding the deck if the analysis changes.

From the repository root, compile with:

    latexmk -pdf -interaction=nonstopmode -halt-on-error meeting_slides/meeting_05/main.tex

The source-review labels and absence of review/author identifiers are discussed in the lecture and notebook. This split is a classroom example, not a claim about generalization to unseen reviewers or genres.

## Material carried forward from 2025

The 2025 supervised deck has 115 PDF pages because many of its 40 numbered slides have incremental overlays. The revised deck consolidates those repeated builds while retaining the substantive content of the following sections:

- Supervised versus unsupervised learning, classification versus regression, and dictionary versus supervised rules (2025 numbered slides 2–5).
- The supervised workflow, representation and feature selection, training-sample coverage and size, train/validation/test splits, and cross-validation (slides 6–14).
- Model, objective, and optimization, including squared-error loss (slides 15–16).
- Bayes' rule, prior/likelihood/posterior, and multinomial Naive Bayes (slides 19–22).
- Hyperplanes, classification by the sign of a score, signed distance, margins, support vectors, and SVMs (slides 25–30).

Detailed kernels, trees, forests, boosting, and neural models are omitted. Annotation procedures and the definitions of evaluation metrics remain in Class 4. Logistic loss, regularization, leakage, and the empirical comparisons complement the retained 2025 material. Soft margins clarify how the ideal separable geometry extends to real text.
