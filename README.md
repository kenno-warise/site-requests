# Webスクレイピングツール

スクレイピングを行いたいサイトのURLとタグ名を指定し、欲しい情報をゲットしてきます。

# 使用方法

ビルドされたアーカイブ（dist/）を使用してローカル内でインストール

```
$ pip install .
```

Pythonインタプリタでの実装

```shell
>>> from site_request import example
>>>
>>> url = 'https://zerofromlight.com/blogs'
>>> tag = 'h5'
>>>
>>> for tag in example.get_data(url, tag):
...     print(tag)
...
【Python】音声合成ライブラリのPyttsx3を使ってサクッと文章から音声生成
【Python】音声認識ライブラリのSpeechRecognitionでサクッと文字起こし
...
...
>>>
```
