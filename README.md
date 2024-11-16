# NER-with-Transformers

A Python-based sentiment analysis implementation using the FinBERT transformer model from Hugging Face's transformers library. This project demonstrates how to perform sentiment analysis on text data using state-of-the-art transformer models.

## Overview

This repository contains a Jupyter notebook that showcases sentiment analysis using the ProsusAI/finbert model. While FinBERT was originally trained on financial texts, it can be used for general sentiment analysis tasks as well.

## Prerequisites

- Python 3.6+
- transformers
- torch
- jupyter

## Installation

1. Clone the repository:
```bash
git clone https://github.com/SakibAhmedShuva/NER-with-Transformers.git
cd NER-with-Transformers
```

2. Install required packages:
```bash
pip install transformers torch jupyter
```

## Usage

1. Open the Jupyter notebook:
```bash
jupyter notebook sentiment_analysis_tf.ipynb
```

2. Run the notebook cells to perform sentiment analysis. Example usage:
```python
from transformers import pipeline

pipe = pipeline(task="text-classification", model="ProsusAI/finbert")
result = pipe("The sun rose, filling the sky with warm colors and bringing hope for a beautiful day ahead.")
print(result)
```

## Features

- Utilizes the ProsusAI/finbert model for sentiment analysis
- Simple pipeline implementation using Hugging Face transformers
- Support for processing single text inputs
- Returns sentiment classifications with confidence scores

## Model Information

The project uses the ProsusAI/finbert model, which can classify text into three sentiment categories:
- Positive
- Negative
- Neutral

## Project Structure

```
NER-with-Transformers/
│
├── sentiment_analysis_tf.ipynb    # Main Jupyter notebook with implementation
├── README.md                      # Project documentation
└── .gitignore                    # Git ignore file
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Hugging Face Transformers](https://github.com/huggingface/transformers)
- [ProsusAI/finbert](https://huggingface.co/ProsusAI/finbert)

## Contact

For any questions or feedback, please open an issue in the repository.
