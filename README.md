## Learning basic Python syntax
## Pythonの基本構文の学習

<sub> Introductory Python Study </sub>

<sub> Pythonの入門学習 </sub>

**環境構築**

*dockerコマンド*

* ビルドコマンド
```
docker compose build
```
* 環境の立ち上げ
```
docker compose up -d
```
* Pythonのコンテナにアクセス
```
docker exec -it stady-python bash
```

*Pythonのコマンド*

* Pythonのバージョン確認
```
python3 --version
```

* set.py(Pythonのパッケージをビルド、インストール、配布する際の必要情報記載)
```
python setup.py sdist
```

*gitコマンド*

* ローカルリポジトリの新規作成
```
git init
```

* ファイルの追跡(変更分全て)
```
git add .
```

* コミット
```
git commit
```

* ローカルリポジトリにリモートリポジトリのURLを貼り付ける
```
git remote add pysyntax URLを貼り付ける
```

* リモートリポジトリへプッシュ
```
git push -u pysyntax main
```

* リモートリポジトリからローカルに反映
```
git fetch
```

* ブランチの移動
```
git checkout main
```

* マージ
```
git merge pysyntax/main
```

---

**Pythonコードスタイルガイド**
* pep8
```
pep8 対象ファイル
```

* flake8
```
flake8 対象ファイル
```

* pylint
```
pylint 対象ファイル
```