# NLP for Tanglish (Code mixed Tamil+English)

This repository contains state of the art Language models and
 Classifier for Code mixed Tanglish (Tamil and English) - spoken
  in Indian sub-continent.

  
## Dataset

1. [Tamil Wikipedia Articles](https://www.kaggle.com/disisbig/tamil-wikipedia-articles) : 
Preprocessed and Transliterated versions of this dataset, used for 
language modeling in this repo, can be downloaded directly from [here](https://drive.google.com/drive/folders/1doonhH7exVGA9EFbk3KRqJ773685UyPI?usp=sharing)

2. [Dravidian Codemix HASOC @ FIRE 2020](https://sites.google.com/view/dravidian-codemix-fire2020/overview)

3. [Dravidian Codemix Sentiment Analysis @ FIRE 2020](https://dravidian-codemix.github.io/2020/)

## Results

### Language Model Perplexity (on validation set)


| Architecture/Dataset | Tamil Wikipedia Articles | Vocab size |
|:--------:|:----:|:----:|
|   ULMFiT  |  37.50  |  8000  |

### Classification Metrics

##### ULMFiT

| Dataset | F1 | Precision | Recall | Notebook to Reproduce results |
|:--------:|:----:|:----:|:----:|:----:|
| Dravidian Codemix HASOC @ FIRE 2020 |  0.88  |  0.88  |  0.88  | [Link](https://github.com/goru001/nlp-for-tanglish/blob/master/classification/classification_model_hasoc.ipynb) |
| Dravidian Codemix Sentiment Analysis @ FIRE 2020 |  0.62  |  0.65 | 0.69 | [Link](https://github.com/goru001/nlp-for-tanglish/blob/master/classification/classification_model_dc_fire.ipynb) |

### Visualizations
 
##### Word Embeddings

| Architecture | Vocab Size | Visualization |
|:--------:|:----:|:----:|
| ULMFiT | 8k | [Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-tanglish/master/language-model/embedding_projector_config.json) |

## Pretrained Models

#### Language Models 
Download pretrained ULMFiT LM with 8k vocab from [here](https://drive.google.com/drive/folders/16QJPPifbh7I85FMP8ASCL68jEmMvvf-V?usp=sharing)

#### Tokenizer

Trained tokenizer using Google's [sentencepiece](https://github.com/google/sentencepiece)

Download the trained model and vocabulary from [here](https://drive.google.com/drive/folders/1dWMr0Uu5GqsxpQRw4wasBDmYChMxPLnp?usp=sharing)