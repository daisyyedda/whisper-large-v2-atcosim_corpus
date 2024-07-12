# Evaluate
This folder contains two Jupyter notebooks for evaluating models on the `Jzuluaga/atcosim_corpus` dataset. The notebooks are:

1. `eval_blank_large.ipynb`: This notebook is intended for evaluating the performance of a Whisper base model on the dataset.
2. `eval_finetuned_large.ipynb`: This notebook is intended for evaluating the performance of our fine-tuned model on dataset.

## Word Error Rate (WER)
**Word Error Rate (WER)** is a common metric used to evaluate the performance of speech recognition systems. It measures the difference between the reference (correct) transcription and the hypothesis (system output) transcription. WER is calculated using the following formula:

`WER = (S + D + I)/N`

Where:
- `S` is the number of substitutions (words in the hypothesis that are different from the reference).
- `D` is the number of deletions (words that are present in the reference but missing in the hypothesis).
- `I` is the number of insertions (words that are present in the hypothesis but not in the reference).
- `N` is the total number of words in the reference transcription.

A lower WER indicates better performance, with 0% representing a perfect transcription.

## Evaluation Metrics
1. **Clean**: Transcription results of the model without any added prompts or normalization applied.

2. **Prmpt** (Prompt): Transcription results of the model with added prompts. Prompts are additional context or instructions provided to the model to guide its transcription process.

3. **Clean-Norm** (Clean Normalized): Transcription results of the model on clean data after normalization has been applied. Normalization typically involves processes like lowercasing, removing punctuation, and other steps to standardize the text.

4. **Prmpt-Norm** (Prompt Normalized): Transcription results of the model with added prompts after normalization has been applied.

## Evaluation Results
To be added.

## Usage
To run these notebooks:

1. `gh repo clone daisyyedda/whisper-large-v2-atcosim_corpus`
2. `cd Evaluate`
3. Execute the cells in sequence to run the evaluations.
