# gpt_index_japanese_trial

このリポジトリは、gpt-index(0.2.5)をOpenAI APIの代わりにHuggingfaceの日本語モデルを使って行った試みのスクリプトを共有するためのものです。

記事
https://note.com/oshizo/n/n137aaa2c29d4

## 動かしてみたい場合
`pip install requirements.txt`を行ってgpt-index_trial.ipynbを実行してください。


## gpt-indexで使えるQAモデルの学習データセット作成とモデル学習を行いたい場合

`create_dataset.ipynb`を使って`train.csv`を作成し、
Google Colab ProのA100で`train_qa_refine.ipynb`を実行してください。

ベースモデルをmediumサイズに変更することで、T4でも学習が可能です。

学習環境の依存ライブラリは`requirements-train.txt`に記載しています。