---
layout: default
title: Augmenting Models
parent: Terarium Workbench
nav_order: 3
has_toc: false
---

# Augmenting Models
{: .no_toc }

Using any model uploaded to or created in Terarium, users can:

- [Edit the model](#editing-a-model)
- [Stratify the model](#stratifying-a-model)
- [Create model configurations](#configuring-and-validating-a-model)

## Editing a model

Model editing enables users to build on existing models. Supported edits include:

- Answering questions about, adding, removing, or changing state variables, transitions, parameters, rate laws, and observables.
- Renaming model elements.
- Setting variable or parameter units.
- Replacing parameters with more complex formulas.
- Resetting the model to its original state.

![Code notebook with AI-generated python code for adding parameters and transitions to an SEIRHD model](/assets/img/terarium/model-edit-notebook.png)

The Edit model operator is a code notebook with an interactive AI assistant. Users describe in plain language the changes they want to make, and the large language model (LLM)-powered assistant automatically generates code to fulfill the request.

## Stratifying a model

Users can make a simple model more complex by stratifying its state variables and parameters. Stratification builds many different versions of a model and its parameters---by location, demographics, or other contextual data---into one large model.

![Stratification of SEIRHD model states and parameters by vaccination status](/assets/img/terarium/model-stratify-wizard.png)

## Configuring and validating a model

![Various country-specific configurations of an SIR model extracted from a scientific paper](/assets/img/terarium/configure-model.png)

Before running a simulation, users can configure a model by setting the initial values and parameters for the condition they want to test. You can use the Configure model operator to:

- Automatically extract a configuration from an optional document or dataset.
- Manually enter values and account for uncertainty in any downstream simulations.
- Select from previously saved configurations in the current project.