# Rotten Tomatoes sentence-polarity data

This directory contains the two original data files from Pang and Lee's sentence polarity dataset v1.0. It was downloaded from Cornell's [Movie Review Data](https://www.cs.cornell.edu/people/pabo/movie-review-data/) page for the Class 4 teaching notebook.

- `rt-polarity.pos`: 5,331 positive snippets
- `rt-polarity.neg`: 5,331 negative snippets

Each line is a downcased movie-review snippet, usually about one sentence. The labels are inherited from the source review: snippets from reviews marked `fresh` at Rotten Tomatoes are treated as positive and snippets from reviews marked `rotten` as negative. They are therefore a useful benchmark for sentiment classification, but not independent sentence-level human annotations.

Please cite:

> Pang, Bo, and Lillian Lee. 2005. “Seeing Stars: Exploiting Class Relationships for Sentiment Categorization with Respect to Rating Scales.” *Proceedings of ACL*.
