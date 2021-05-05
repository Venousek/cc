# Code for [Clickbait Challenge 2017](https://www.clickbait-challenge.org/) (Ranked 1st in the Final Evaluation)
## Corresponding report: https://arxiv.org/abs/1710.05364

## Steps:
1. Download glove: `wget http://nlp.stanford.edu/data/glove.6B.zip && unzip glove.6B.zip`
2. Change `dir` flag in `train.py` to correct directory.
3. Install:
    - pip install Pillow hickle
4. Download training data: `wget -O ./clickbait17-train-170630.zip https://zenodo.org/record/3346491/files/clickbait17-train-170630.zip?download=1`
5. TODO split data into training and validation
6. `python train.py`