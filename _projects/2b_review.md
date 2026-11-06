---
layout: page
title: LitReview — Systematic Literature Review Workbench
description: A local desktop application for screening, notes, clustering, and interactive bibliometric analysis
img: assets/img/litreview_thumb.jpg
importance: 2
category: fun
github: https://github.com/lvnttran/litreview_project
---

Conducting systematic literature reviews often means dealing with thousands of papers spread across spreadsheets, reference managers, and static PDF folders. I wanted a self-contained application that streamlines title and abstract screening, qualitative extraction, and interactive topic clustering while remaining fully local and non-destructive to existing research databases.   

**LitReview Insight Hub** is a desktop workbench designed for researchers needing speed, repeatability, and control over large literature corpora. Rather than locking research into proprietary cloud tools, the application operates directly on local SQLite databases. It features an additive architecture that tracks screening decisions, custom note types, and automated document clusters without altering legacy schemas or raw notes.   

Built with **Python (Tkinter), scikit-learn, and pandas**, the application integrates traditional systematic review workflows—like PRISMA tracking and duplicate resolution—with machine learning text vectorization for interactive corpus exploration.

### Current features

- Multi-criteria paper screening (Included, Excluded, Maybe, Unscreened) with keyboard shortcuts
- Non-destructive side-table architecture that preserves original database schemas and legacy note fields
- Automated duplicate detection using fuzzy title matching and record merging
- TF-IDF vectorization paired with K-Means clustering for automatic topic discovery
- PRISMA flow counts, exclusion reason tracking, and automated audit logging
- Categorized note-taking with dedicated tags for findings, quotes, questions, and action items.
- Keyword search with prefix wildcard support (configur*) and full-text abstract highlighting.
- Interactive analytics dashboard for co-occurrence networks, keyword trends, and temporal distributions.
- Automated SQLite snapshot backups generated prior to schema migrations or bulk actions
- Responsive web interface for desktop and tablet use.

### Ideas explored

As a playground for research productivity tools, this project experiments with features that reduce manual labor in literature synthesis while maintaining methodological rigour:

- 🎯 Relevance-First Sorting that automatically reorders unscreened papers based on TF-IDF similarity to previously included items.
- 📊 Interactive Co-occurrence Heatmaps connecting keywords, tags, screening statuses, and topic clusters.
- 💡 Contextual Keyword Expansion that extracts characterising terms from filtered results to guide further searches.
- 📋 Automated PRISMA Generator to produce exportable flow diagrams for journal submissions.
- 🔄 Background Cluster Execution to process thousands of abstracts without freezing the user interface.

### Technologies

- Python
- Tkinter / ttk
- SQLite
- SQLAlchemy
- pandas
- Numpy
- scikit-learn
- Matplotlib
