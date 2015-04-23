Learning-Python
===============

## Setup Python

### pyenvのインストール
<pre>
$ brew install pyenv-virtualenv pyenv
$ vim ~/.zshrc
export PYENV_ROOT="${HOME}/.pyenv"
if [ -d "${PYENV_ROOT}" ]; then
    export PATH=${PYENV_ROOT}/bin:$PATH
    eval "$(pyenv init -)"
fi

$ source ~/.zshrc

</pre>

#### Pythonをインストールする
<pre>
pyenv install -l
pyenv install 2.7.7
pyenv versions
</pre>

<pre>
mkdir %project home%
cd %project home%
pyenv virtualenv 2.7.7 netcomm_dev
pyenv local netcomm_dev
pyenv version
</pre>

#### ライブラリのインストール
<pre>
$ pip install -e .
$ pip install -r requirements.txt
</pre>

#### ライブラリの追加
<pre>
pip freeze
</pre>

## コーディング

### チュートリアル
http://docs.python.jp/

### コーディング規約
PEP8:
http://pep8-ja.readthedocs.org/ja/latest/#

Google Python Style Guide:
http://works.surgo.jp/translation/pyguide.html

### ドキュメンテーション
Sphinx, docstring

### プロジェクト雛形の生成
cookiecutter:
PasteScript:
http://collective-docs.takanory.net/tutorials/paste.html#

### 3rd Party Libraryの探し方・追加方法

### ロギング

### 設定ファイル

## Unit Test
unittest2, pytest, doctest

## カバレッジの測定

## 配布
Distutils, setuptools (distribute)

## 起動と終了