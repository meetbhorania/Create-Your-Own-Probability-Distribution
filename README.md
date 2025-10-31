# Language Model Text Generation Lab

This project explores the fundamental principles of language models by implementing probability-based text generation. Using a sampling approach, the lab demonstrates how language models assign probability distributions to candidate words and generate coherent text continuations.

## Overview

This implementation focuses on generating text continuations from a given prompt by randomly sampling words based on their probability distributions. The core prompt used throughout the project is: *"Jide was hungry so she went looking for"* — adapted from Eldan and Li's 2023 paper *TinyStories: How Small Can Language Models Be and Still Speak Coherent English?*

The project demonstrates how probability values influence word selection and how context shapes the distribution over possible next words. By manually assigning and manipulating these probabilities, the implementation mimics the basic mechanics of language models before diving into automated model training.

## Key Features

- **Probability Assignment**: Assign probability values to candidate words based on contextual likelihood
- **Random Sampling**: Utilize `random.choices` function with custom probability distributions for word selection
- **Context-Aware Generation**: Generate text that adapts to different prompt variations
- **Prompt Exploration**: Investigate how modifications (e.g., changing "hungry" to "thirsty" or altering the subject) affect probability distributions and predictions

## Learning Outcomes

By working through this project, you will gain understanding of:

- How probabilities drive next-word prediction in language models
- The relationship between context and probability distributions
- Practical sampling techniques for text generation
- The foundational principles underlying modern language models

## Getting Started

### Prerequisites

- Python 3.x
- Google Colab (recommended) or Jupyter Notebook
- Basic understanding of probability and Python programming

### Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/language-model-text-generation-lab.git
```

2. Open the notebook in Google Colab or Jupyter Notebook

3. Run the cells sequentially to explore the text generation process

## Usage

The notebook guides you through:

1. Setting up the prompt and candidate words
2. Assigning probability distributions based on context
3. Sampling words using the probability distributions
4. Generating text continuations
5. Experimenting with different prompts and probability assignments

## Example
```python
prompt = "Jide was hungry so she went looking for"
candidates = ["food", "water", "help", "her phone"]
probabilities = [0.6, 0.1, 0.2, 0.1]

# Sample next word based on probabilities
next_word = random.choices(candidates, weights=probabilities)[0]
print(f"{prompt} {next_word}")
```

## References

[1] Eldan, R., & Li, Y. (2023). TinyStories: How Small Can Language Models Be and Still Speak Coherent English?

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Inspired by the TinyStories paper by Eldan and Li
- Part of a language models course curriculum
