# Class 5: Supervised modelling

This folder adapts the original 2025 supervised class for Class 5 in 2026:

- `main.pdf`: the 2026 title and simplified SVM, tree, and ensemble sections, combined with the retained 2025 material
- `main.tex`: editable source for the new sections and the PDF-page assembly
- `source/ceu_2025_supervised.pdf`: the unchanged original 2025 deck
- `meeting_05.ipynb`: `CEU_2025/meeting_slides/meeting_07/supervised_ml.ipynb`
- `reviews.csv`: the original notebook's local dataset
- `loss_viz.jl`: the original loss visualization script

The opening and Naive Bayes material retain the original incremental builds. The ideology in one dimension and nonlinear-map slides are preserved. The detailed kernel section and gradient-boosting section are omitted. The deck has 42 logical slides across 86 PDF pages, with updated 2026 footers.

Eight added slides cover preprocessing leakage, a worked Naive Bayes prediction, learned log-odds word weights, logistic regression and log loss, and regularization with a training/validation plot.

The original repository provides no LaTeX source. The new source imports retained pages directly from the archived PDF, so their contents remain intact. The notebook retains the full 2025 material. Its regularization section now fits TF-IDF on training text only and exports the plot used in the slides. That section has been rerun; the remainder of the legacy notebook has not been re-executed as part of this edit.

To compile from the repository root:

    latexmk -pdf meeting_slides/meeting_05/main.tex

Run the notebook from this folder so it can find `reviews.csv`.

The earlier 2026 draft, including its LaTeX source, notebook, results, and figures, is preserved in `previous_draft_2026-10-12/`.
