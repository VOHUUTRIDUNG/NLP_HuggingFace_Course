# NLP_HuggingFace_Course
My notes on learning NLP HuggingFace course!
## Table of Contents
- [Chapter 1. Transformer models](#chapter-1---transformer-models)
- [Chapter 2. Using 🤗 Transformers](#chapter-2---using--transformers)
- [Chapter 3. Fine-tuning a pretrained model](#chapter-3---fine-tuning-a-pretrained-model)
- [Chapter 4. Sharing models and tokenizers](#chapter-4---sharing-models-and-tokenizers)
- [Chapter 5. The 🤗 Datasets library](#chapter-5---the--datasets-library)
- [Chapter 6. The 🤗 Tokenizers library](#chapter-6---the--tokenizers-library)
- [Chapter 7. Main NLP tasks](#chapter-7---main-nlp-tasks)
- [Chapter 8. How to ask for help](#chapter-8---how-to-ask-for-help)
- [Chapter 9. Building and sharing demos](#chapter-9---building-and-sharing-demos)

-------------------------------------------------------------------------------------

## Chapter 1 - Transformer models
### Working with pipelines:
- The most basic object in the 🤗 Transformers library is the pipeline() function. It connects a model with its necessary preprocessing and postprocessing steps, allowing us to directly input any text and get an intelligible answer.
- There are three main steps involved when you pass some text to a pipeline:
  1. The text is preprocessed into a format the model can understand.
  2. The preprocessed inputs are passed to the model.
  3. The predictions of the model are post-processed, so you can make sense of them.
- Some of the currently available pipelines are:
  1. feature-extraction (get the vector representation of a text)
  2. fill-mask
  3. ner (named entity recognition)
  4. question-answering
  5. sentiment-analysis
  6. summarization
  7. text-generation
  8. translation
  9. zero-shot-classification
- You can see basic use of pipelines [here](working-with-pipelines.ipynb)

## Chapter 2 - Using 🤗 Transformers
### Behind the pipeline
- The pipeline groups together three steps: preprocessing, passing the inputs through the model, and postprocessing:
![pipeline](images/pipeline.svg)
#### 1, Preprocessing with a tokenizer
- Like other neural networks, Transformer models can’t process raw text directly, so the first step of our pipeline is to convert the text inputs into numbers that the model can make sense of. To do this we use a tokenizer, which will be responsible for:
  1. Splitting the input into words, subwords, or symbols (like punctuation) that are called tokens
  2. Mapping each token to an integer
  3. Adding additional inputs that may be useful to the model
#### 2, Going through the model

## Chapter 3 - Fine-tuning a pretrained model

## Chapter 4 - Sharing models and tokenizers

## Chapter 5 - The 🤗 Datasets library

## Chapter 6 - The 🤗 Tokenizers library

## Chapter 7 - Main NLP tasks
- Common NLP tasks:
  - Token classification
  - Masked language modeling (like BERT)
  - Summarization
  - Translation
  - Causal language modeling pretraining (like GPT-2)
  - Question answering
### Token classification
- This generic task encompasses any problem that can be formulated as “attributing a label to each token in a sentence,” such as:
 - Named entity recognition (NER): Find the entities (such as persons, locations, or organizations) in a sentence. This can be formulated as attributing a label to each token by having one class per entity and one class for “no entity.”
 - Part-of-speech tagging (POS): Mark each word in a sentence as corresponding to a particular part of speech (such as noun, verb, adjective, etc.)
 - Chunking: Find the tokens that belong to the same entity. This task (which can be combined with POS or NER) can be formulated as attributing one label (usually B-) to any tokens that are at the beginning of a chunk, another label (usually I-) to tokens that are inside a chunk, and a third label (usually O) to tokens that don’t belong to any chunk.
- I will exemplify it [here]()

## Chapter 8 - How to ask for help

## Chapter 9 - Building and sharing demos





