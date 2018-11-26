# Challenge : Sentiment Classification 
[Naver Sentiment Movie Corpus](https://github.com/e9t/nsmc)를 기반으로 진행되는 **Sentiment Classification** Challenge

## Rule
1. 150k review로 이루어진 `ratings_train.txt` data를 적절히 splitting하여, ***120k reviews를 training data으로, 30k reviews는 validation data로 활용한다.***
2. tokenizing 결과에 따라 Vocabulary 구성해야할 경우, 1번의 120k reviews로만 구성한다. 즉 120k reviews에 없는 token일 경우 `<unk>`로 처리한다.
  + Vocabulary of training data : {"모두의연구소", "딥러닝"}, 
  + Vocabulary of validation data : {"파이토치", "모두의 연구소"}
  + Vocabulary of test data : {"모두의연구소","텐서플로우"}
  + 위의 경우 Vocabulary of validation data에 있는 "파이토치", Vocabulary of test data에 있는 "텐서플로우"는 모두 `<unk>`로 취급한다.
  + 이는 Character level로 tokenizing을 해도 마찬가지이다.
3. `ratings_text.txt` data는 test data로, 해당 data에 대해서 Test accuracy를 계산하여 승자를 가린다.
  + `.ipynb` 파일로 제출하되, 계산한 Test accuracy를 `.ipynb` 파일에 병기한다.
  + `.ipynb` 파일 자체는 실행이 가능한 코드인지만 확인한다.
4. epochs 수는 최대 30회로 제한한다.


## Baseline
[Sentence classification by MorphConv.ipynb](https://nbviewer.jupyter.org/github/modulabs/flipped_competition/blob/master/challenge_nsmc/Sentence%20classification%20by%20MorphConv.ipynb)