---
layout: default
title: Choosing a Starting Point 
parent: Terarium Workbench
nav_order: 2
has_toc: true
---

# Choosing a Starting Point

Terarium helps users find a starting point in a proliferation of research by:

- Serving as a repository for uploaded modeling resources such as models, documents, and datasets.
- Enabling the automatic recreation of models extracted from scientific literature.
- Generating goal-driven model comparisons.

## Uploading resources

With Terarium, users can gather, store, and manage resources needed for their modeling and simulation workflows. They can upload documents, models, and datasets or get them from other projects in Terarium.

![Upload dialog showing the types of documents, models and datasets that Terarium supports](/assets/img/terarium/upload.png)

Users can transform and simulate uploaded documents, models, and datasets from the project resources by dragging them into a workflow.

Most uploaded resources are available for use right away. Uploaded PDFs however, are first processed to extract any linear ordinary differential equations found in the text.

## Recreating models from literature

![Equations automatically extracted from a scientific report on COVID-19 interventions](/assets/img/terarium/create-model-from-equations.png)

The Create model from equations operator helps users recreate a model from literature or build a new model from LaTeX equations. In this process, users:

1. Choose or enter the equations to include in the model by:
   - Selecting equations extracted from an attached document.
   - Extracting equations from a pasted screenshot.
   - Entering or pasting LaTeX code. 
2. Create the model as an output or resource for use in other modeling and configuration processes.

## Comparing models

![Side-by-side diagrams and summaries of SIR and SEIRHD models](/assets/img/terarium/compare-models.png)

Users can compare two or more models in Terarium to see:

- A brief overview of their structural and metadata similarities and differences.
- Side-by-side comparisons of key model details.
- An AI-assisted visualization of common and unique state variables and transitions across each model.

The Compare models operator is powered by an interactive AI assistant. The assistant automatically compares the models based on any enriched metadata and can generate summaries tailored to user modeling goals.