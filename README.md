This project implements a machine learning pipeline that converts knowledge graph triples into natural language sentences using a combination of T5 transformer and Graph Isomorphism Network (GIN).

## Table of Contents

1. [Installation](#installation)
2. [Project Overview](#project-overview)
3. [Data](#data)
4. [Model Architecture](#model-architecture)
5. [Usage](#usage)
6. [Dependencies](#dependencies)

## Installation

To set up the project, run the following command:

```bash
pip install datasets torch_geometric transformers torch
```

## Project Overview

This project aims to generate natural language sentences from structured knowledge graph triples. It utilizes the T5 model for text generation and a Graph Isomorphism Network (GIN) for processing graph-structured data.

## Data

The project uses the KELM corpus dataset, which contains knowledge graph triples and corresponding natural language sentences. The dataset is loaded from the following URLs:

- Train: https://storage.googleapis.com/gresearch/kelm-corpus/updated-2021/quadruples-train.tsv
- Validation: https://storage.googleapis.com/gresearch/kelm-corpus/updated-2021/quadruples-validation.tsv
- Test: https://storage.googleapis.com/gresearch/kelm-corpus/updated-2021/quadruples-test.tsv

## Model Architecture

The project combines two main components:

1. **T5 Model**: A pre-trained T5-small model is used for text generation tasks.
2. **Graph Isomorphism Network (GIN)**: A custom GIN model is implemented to process graph-structured data.

## Usage

1. The script first loads and preprocesses the KELM corpus dataset.
2. It then tokenizes the input data using the T5 tokenizer.
3. The preprocessed data is loaded into DataLoader objects for training, validation, and testing.
4. The GIN model is defined for graph processing.
5. (Note: The training loop and evaluation steps are not included in the provided snippet)

## Dependencies

- PyTorch
- Transformers
- Datasets
- PyTorch Geometric
