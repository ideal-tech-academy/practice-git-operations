# 02. Commands
Git コマンドに関するドキュメント

## Basic - 基本コマンド

### Clone
クローン：Web上のリモートリポジトリを、自分のPCにローカルリポジトリとして複製する
```bash
git clone {リポジトリ}
```

例）このリポジトリをクローンする場合
```bash
git clone git@github.com:ideal-tech-academy/practice-git-operations.git
```

### pull
プル：リモートリポジトリ状態を、ローカルリポジトリに反映させて最新化する

```bash
git pull
```

### add
ステージング：

```bash
## add の後に対象を入力. "." の場合は全ての変更を対象とする
git add .
```

### commit
コミット：

```bash
git commit -m "何を変更したのかわかるメッセージ（50文字以内）"
```

### push
プッシュ：

```bash
git push origin
```

## Branch Operation - ブランチ操作

### Branch
一覧表示：

### Checkout
ブランチ切り替え：

### Delete branch
ブランチ削除：

### Merge
マージ：
