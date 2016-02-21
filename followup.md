Git再入門 フォローアップ資料
=============================

Gitの設定事例集
-----------------------------

### 改行コードの自動変換を行う

```
git config --global core.autocrlf true|input|false
```

core.autocrlfの設定内容に応じた自動変換の内容は次のとおりです

- true: コミット時とチェックアウト時に改行コードの自動変換を行います
- input: コミット時のみ改行コードの自動変換を行います
- false: 改行コードの自動変換は行いません

### コミット時のデフォルトメッセージを設定したい

```
git config --global commit.template /path/to/template_file
```

### 日本語ファイル名をgit statusなどで表示したい

```
git config --global core.quotepath false
```

### fetchやpullする際にリモートで削除されているリモートブランチを削除したい

```
git config --global fetch.prune true
```

### pullする際にmergeではなくrebaseしてほしい

```
git config --global pull.rebase
```
