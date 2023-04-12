[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/ymop5HUw)
# CMPSC 310 Activity 15

## Deadline: April 12 by 9:50am

## Assignment

 For this activity follow [Neural machine translation with a Transformer and Keras](https://www.tensorflow.org/text/tutorials/transformer).

## Submission

Submit completed Colab notebook showing generated output.

## Description

### Embedding and Positional Encoding

This layer takes a set of tokens in and converts them to vectors. Since the attentional layers use these vectors in no particular order and in parallel, we use positional encoding to define the order of the words being used.

### Attention Layers

The model contatins many basic attention layers. These layers are used as a type of fuzzy, non-static dictionary lookup. This allows the model to provide an input sequence and be returned a query.

#### Cross Attention Layer

This attention layer is similar to the others, but it uses attention to instead connect the encoder and decoder.

#### Global Self-Attention Layer

This attention layer processes the context sequence, and propogates information along its length. Use attention here as opposed to RNNs and CNNs allows the model to be used in parallel. This allows us to move the work to GPU hardware, massively improving performance and efficiency.
