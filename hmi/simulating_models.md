---
layout: default
title: Simulating Models
parent: Terarium Workbench
nav_order: 4
has_toc: true
---

# Simulating models
{: .no_toc }

Terarium's simulation capabilities help predict outcomes and reveal system behaviors by enabling users to calibrate models, conduct sensitivity analyses, create interventions, and optimize ensemble models to make informed decisions.

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Calibrating a model

Calibration enables users to improve the performance of a model by updating the value of configuration parameters. Calibrate a model with a reference dataset of observations and an optional intervention policy representing historical events. The calibrated model essentially represents the best estimate of the state of the world conditioned on data.

![Calibration results showing decreased loss over time and before/after parameter distributions](/assets/img/terarium/model-calibrate-notebook.png)

## Running a sensitivity analysis

Using the Terarium Simulation operator, users can conduct a sensitivity analysis to determine how changes in model parameters affect the outcome variables of interest (e.g., to see how varying vaccination rates and transmission impact hospitalizations).

![Sensitivity analysis of the effect of transmission rates on hospitalizations due to Mpox](/assets/img/terarium/sensitivity-analysis.png)

Sensitivity analysis workflows can be built manually or using a template to automatically set up the required components.

## Creating interventions

Users can define intervention policies to specify changes in state variables or parameters at specific points in time. This can help answer key decision-maker questions like:

> How does increasing vaccination rate affect cases and hospitalizations?

![Two static interventions to introduce masking and vaccination policies at a specific time](/assets/img/terarium/create-intervention-policy.png)

Given a model configuration and a proposed intervention policy, users can also identify the optimal parameter values and/or times to implement an intervention that satisfy specified constraints. This helps users make informed decisions when faced with questions like:

- What is the smallest possible transmission rate reduction that will keep infections below 1000 over the next 100 days?
- When is the latest possible time an intervention that reduces the transmission rate by half may be implemented in order to ensure infections remain below 1000 over the next 100 days?
- What is the minimal reduction in transmission rate, and the latest time it can be applied in order to keep infections below 1000 over the next 100 days?

## Ensemble modeling

Terarium's ensemble modeling capabilities allow users to first independently process (calibrate or simulate) individual models and then collectively optimize as a single ensemble. Ensemble operations allow for the discovery of solutions where member models can specialize in different aspects, enhancing overall performance.

![Charts showing the effects of ensemble calibration on susceptible and exposed populations](/assets/img/terarium/ensemble-variables.png)

## Comparing results

Compare simulation results to understand the impact of scenarios, rank interventions based on multiple criteria, or assess model errors.

![Graph comparing cases and deaths under different intervention policies](/assets/img/terarium/compare-datasets-variables-over-time.png)