本项目为《机器学习导论》课程的结课作业。

各文件的用途说明如下：

1. [机器学习导论作业报告.docx](/机器学习导论作业报告.docx) 和 [机器学习导论作业报告.pdf](/机器学习导论作业报告.pdf) 分别为作业报告的 word 版和 pdf 版。

1. [NB variants on IMDB](/NB_variants_on_IMDB.ipynb)：该 notebook 记录了作业报告第 2.3 节所使用的三个朴素贝叶斯模型 BNB、MNB 和 CNB 的代码和运行结果。在 kaggle 上也有[该 notebook](https://www.kaggle.com/code/noal02d/imdbnbvariants)。

2. [11 models comparision without keepwords](/11_models_comparision_without_keepwords.ipynb)：该 notebook 记录了作业报告第 2.4 节所进行的多种传统机器学习模型的代码和运行结果，且未保留诸如 not、don't 等含有确切含义的停止词。在 kaggle 上也有[该 notebook](https://www.kaggle.com/code/noal02d/11modelsonimdb/notebook?scriptVersionId=322653797)。

> [!note]- 具体的模型：
> | 模型名称 | 特征类型 |
> |:-:|:-:|
> |LinearSVC | TF-IDF|
> |Logistic Regression | TF-IDF|
> |SGD Classifier | TF-IDF|
> |Passive Aggressive | TF-IDF|
> |Complement Naive Bayes | TF-IDF|
> |Bernoulli Naive Bayes | BERN|
> |Multinomial Naive Bayes | BOW|
> |Random Forest | TF-IDF|
> |Gradient Boosting | TF-IDF|
> |K-Nearest Neighbors | TF-IDF|
> |Decision Tree | TF-IDF|

> [!note]- 具体的含有明确含义的停止词：
> ```python
> KEEP_WORDS = {
>    'not', 'no', 'nor', 'neither', 'never', 'nobody', 
>    'nothing', 'nowhere', 'don', 'doesn', 'didn', 
>    'won', 'wouldn', 'shouldn', 'couldn', 'isn', 'aren',
>    'but', 'however', 'although', 'though',
>    'very', 'too', 'so', 'most', 'more'
>}
> ```
>


4. [11 models comparison with keepwords](/11_models_comparision_with_keepwords.ipynb)：同上，但保留了诸如此类的停止词。在 kaggle 上也有[该 notebook](https://www.kaggle.com/code/noal02d/11modelsonimdb)，上个文件在 kaggle 上是本文件的一个旧 version。

4. [LSTM model](/EmbeddingLSTM.ipynb)：该 notebook 记录了作业报告第 3 节所使用的 Bi-LSTM 架构的代码和运行结果。在 kaggle 上也有[该 notebook](https://www.kaggle.com/code/noal02d/purelstmonimdb)。

5. [best LSTM model](/embedding_lstm_model.pt)：该文件是保存的最好 LSTM 模型，文件类型为 `.pt`。在 kaggle 上保存在上个文件的 output 中。

6. [BERT+LSTM+CNN](/BERT+LSTM+CNN.ipynb)：该 notebook 是第 4 节文末引用的两张图的来源。在 kaggle 上也有[该 notebook](https://www.kaggle.com/code/noal02d/notebook813a8e6e24)。