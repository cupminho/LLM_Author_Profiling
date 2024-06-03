# LLM_Author_Profiling

This repository contains the source code and data used for the paper submitted to DFRWS APAC 2024, titled "Author Profiling using Large Language Models for Digital Text Forensics".

## Overview

In this study, we explore the use of large language models (LLMs) for author profiling in digital text forensics. Our work investigates the effectiveness of various fine-tuning strategies, including full fine-tuning, Low-Rank Adaptation (LoRA), and Quantized LoRA (QLoRA), in predicting the age and gender of authors based on their writing styles. The dataset used in our experiments is the "NIKL Korean Dialogue Corpus 2022 (v.1.0)", provided by the National Institute of Korean Language.

## Dataset

The original dataset can be downloaded from the National Institute of the Korean Language website at the following link:

- [Original Dataset](http://www.korean.go.kr/front/)

The preprocessed CSV file used in this study contains information such as the utterance text, speaker's age, occupation, gender, current residence, and the corresponding original and cleaned utterance forms.

## Fine-Tuning Configurations

The fine-tuning hyperparameters and training configurations for each model are provided in the `configurations` directory.

## Source Code

The source code used for training the models and conducting experiments is available in the `src` directory.

## Usage

To reproduce the results of the study, follow the instructions below:

1. Clone this repository:
    ```sh
    git clone https://github.com/your-username/LLM_Author_Profiling.git
    cd LLM_Author_Profiling
    ```

2. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

3. Run the training scripts:
    ```sh
    python src/train_polyglot.py
    python src/train_eeve.py
    python src/train_blossom.py
    ```

4. Evaluate the models:
    ```sh
    python src/evaluate.py
    ```

## Contact

For any questions or issues, please open an issue on this repository or contact the maintainer at [your-email@example.com](mailto:your-email@example.com).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
