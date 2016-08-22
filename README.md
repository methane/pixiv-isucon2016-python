# Pixiv 社内 ISUCON 2016, Python 実装

[Pixiv 社内 ISUCON 2016](https://github.com/catatsuy/private-isu) の Python 版実装です。

Python で ISUCON 2016 に参加する予定の人が、 Pixiv 社内 ISUCON を使って練習するときの
参照実装として使えるようにと考えています。


## セットアップ

### チェックアウト

AMI からのスタートでも、 リポジトリからのスタートでも、 `webapp` ディレクトリがあるはずなので、
そこにこのリポジトリをチェックアウトしてください。

```console
$ cd private_isu/webapp
$ git clone https://github.com/methane/pixiv-isucon2016-python python
$ cd python
```


### 実行環境の準備

pyenv 等を利用して Python 3.5.2 を準備しておいてください。
以下の例では venv を用意していますが、 pyenv を使ってる場合は venv を利用せず直接インストールしても大丈夫です。


```console
$ python3 -V
Python 3.5.2
$ python3 -m venv venv
$ venv/bin/pip install -r requirements.freeze
```


## デバッグモードで実行

```console
$ FLASK_APP=app.py venv/bin/flask run -p 8080 --debugger
```

