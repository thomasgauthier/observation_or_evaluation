# Observation or Evaluation Dataset Generation

This repository contains code for generating, refining, and evaluating a synthetic dataset based on the principles of Nonviolent Communication (NVC) as taught by Marshall Rosenberg. The project aims to distinguish between observations (factual statements) and evaluations (judgmental statements) to aid in understanding and practicing effective empathetic communication. This dataset serves as a benchmark for assessing language models' abilities in sentiment analysis and subjective interpretation.

## Overview

The project leverages open-source language models and a small budget to create a high-quality synthetic dataset. It involves generating initial statements, classifying them as observations or evaluations, refining the dataset for quality and balance, and finally, pushing the dataset to the Hugging Face Hub for accessibility.

## Links

A [post](https://thomasgauthier.dev/devlog/nvc) detailing the creation process of this dataset can be found on my blog.
The same content is present in the [observation or evaluation notebook](/observation_or_evaluation.ipynb)

The final dataset can be found on Hugging Face
https://huggingface.co/datasets/thomasgauthier/observation_or_evaluation  

## Workflow

1. **Dataset Generation:** Utilizes large language models to generate statements based on exercises from NVC literature and scripts from the TV show "Seinfeld" to ensure variety and relatability.
2. **Classification:** Each statement is classified as an observation or evaluation, with some being marked as mixed or given pure observation alternatives.
3. **Quality Control:** A subset of generated statements undergoes a quality assessment process to filter out low-quality samples.
4. **Balancing:** The dataset is balanced to ensure an equal representation of observations and evaluations.
5. **Push to Hugging Face Hub:** The final dataset is pushed to the Hugging Face Hub, making it accessible for further research and application.

## Structure

- `observation_or_evaluation.ipynb`: The complete code for generating, filtering and refining the dataset
- `generations.csv`: A CSV file with all the prompts and generations (with generation parameters) sent and received from Together.ai


## Acknowledgments

- Marshall B. Rosenberg for the foundational work on Nonviolent Communication.
- The creators and maintainers of the language models and APIs used in this project.
- Hugging Face for providing an accessible platform to host and share datasets.
