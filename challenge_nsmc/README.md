# Challenge : Sentiment Classification 
[Naver Sentiment Movie Corpus](https://github.com/e9t/nsmc)를 기반으로 진행되는 **Sentiment Classification** Challenge

## Rule
1. 150k review로 이루어진 `ratings_train.txt` data를 적절히 splitting하여 120k reviews로만 training하고 30k reviews로는 validation에 활용한다.
2. `ratings_text.txt` data로 Test accuracy를 계산하여 승자를 가린다.
3. epochs 수는 최대 10회로 제한한다.
4. Vocabulary 구성 시 1번의 120k reviews로만 구성한다.

## Baseline
[Sentence classification by MorphConv.ipynb](https://nbviewer.jupyter.org/github/modulabs/flipped_competition/blob/master/challenge_nsmc/Sentence%20classification%20by%20MorphConv.ipynb)