# Sentence similarity

## Synopsis

This repository contains several implementations of neural networks to learn a either a measure or a binary classification for Sentence Similarity:

* A Siamese LSTM Network

## Installation

This installation list represent solely the main tasks to do in order to have the SA trainer/predicter running on a supposed system.
Do not take it a perfect and suitable for your current env.

1. Install [python 3.6](https://www.python.org/downloads/release/python-360)
  1. Set your PYTHONPATH to the python libraries path (`/usr/lib/python3.6/site-packages/` on archlinux)
2. Clone the repo: `git clone git@git.recast.ai:lab/sentence_similarity.git --recurse-submodules`
3. Go to the working dir: `cd sentence_similarity`
4. Install the dependencies: `[sudo] pip install -r requirements.txt`
5. Get FastText embeddings
  1. Download the english embeddings `wget https://cdn.recast.ai/models/en.ft.vec -O sentiment_analysis/vectors/en.vec`
  2. Download the french embeddings `wget https://cdn.recast.ai/models/fr.ft.vec -O sentiment_analysis/vectors/fr.vec`
  3. Download the spanish embeddings `wget https://cdn.recast.ai/models/es.ft.vec -O sentiment_analysis/vectors/es.vec`
  3. Download the other languages embeddings `wget https://cdn.recast.ai/models/ot.ft.vec -O sentiment_analysis/vectors/ot.vec`
6. Create your keras configuration: `mkdir ~/.keras && mv ./keras.dist ~/.keras/keras.json`
7. Run SA trainer `python ./train.py (fr|en|es|ot) dataset`
8. Make a predict test.
  1. Fill a test file with test sentences
  2. Test your model: `python ./predict.py (en|fr|es|ot) model meta --interactive`
9. ???
10. Profit!

## Usage

## Future work
