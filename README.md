# Transformer Notebook

This Jupyter notebook contains the implementation of a sequence-to-sequence (seq2seq) transformer model for Neural Machine Translation (NMT). The model is trained to translate from French to English.

## Requirements

The notebook uses the following libraries:

- PyTorch
- Huggingface's `transformers` and `datasets`
- NLTK

## Structure

The notebook is divided into several sections:

1. **Learning Objectives**: This section provides an overview of the tasks to be accomplished in the notebook.

2. **Installing Packages**: This section installs the necessary packages.

3. **Download NMT data**: This section downloads the data for NMT, which contains pairs of parallel sentences.

4. **Data preprocessing**: This section loads and tokenizes the data for NMT.

5. **Transformer model for NMT**: This section implements the encoder-decoder transformer model for NMT. It includes the implementation of the MultiHeadAttention, TransformerEmbeddings, TransformerBlock, and EncoderDecoderModel classes.

6. **Train the model**: This section trains the seq2seq model on the parallel tokenized corpus.

7. **Evaluate the model**: This section evaluates the model on the test set by generating translations with beam search and comparing them to the gold translations using the BLEU score.

## Usage

To use this notebook, you need to run each cell in order. The training process can take a while, especially if you're not using a GPU. The notebook includes a function for saving the model parameters to a file `model.pt` throughout training, so you can resume training later or use the trained model for evaluation without having to train it again.

## Output

The output of the notebook includes the trained model, the translations it generates on the test set, and the BLEU score of these translations. The notebook also includes some examples of the translations and the corresponding gold translations for comparison.
