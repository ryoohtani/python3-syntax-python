FROM python:3.13.0b3-bookworm

WORKDIR /src

COPY . /src/

# パッケージの更新
RUN apt-get update
# キャッシュクリーンアップと不要なリストの削除
RUN apt-get clean && rm -rf /var/lib/apt/lists/*
# リナックスコマンドのパッケージインストール
RUN apt-get update && apt-get install -y vim less sudo tree
# pip関連
RUN pip install --upgrade pip

RUN pip install --upgrade setuptools

# コードスタイルの制約をするライブラリ
RUN pip install --upgrade pep8
RUN pip install --upgrade flake8
RUN pip install --upgrade pylint

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

EXPOSE 8800