# Code for [Clickbait Challenge 2017](https://www.clickbait-challenge.org/) (Ranked 1st in the Final Evaluation)
## Corresponding report: https://arxiv.org/abs/1710.05364

## Steps:
0. Create conda env and install deps:
```
conda create -y -n p37_tf1 python=3.7
conda activate p37_tf1
conda install tensorflow-gpu==1.15.0
pip install Pillow hickle nltk gensim scikit-learn python-Levenshtein
```
1. Download glove: `wget http://nlp.stanford.edu/data/glove.6B.zip && unzip glove.6B.zip`
2. Change `dir` flag in `train.py` to correct directory.
3. Download training data: `wget -O ./clickbait17-train-170630.zip https://zenodo.org/record/3346491/files/clickbait17-train-170630.zip?download=1`
4. split data into training and validation (70:30)
5. Run `python train.py`