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
ステージング：変更（新規作成・修正・削除）したファイルを指定し、「インデックス」に加える
👉 インデックス：変更内容を確定する前に、候補としてファイルが登録される場所

```bash
## add の後に対象を入力. "." の場合は全ての変更を対象とする
git add .
```

### commit
コミット：変更履歴を確定し、ローカルリポジトリに変更履歴を保存する
👉 インデックスに登録されたファイルと変更内容が記録される

```bash
git commit -m "何を変更したのかわかるメッセージ（50文字以内）"
```

### push
プッシュ：ローカルリポジトリの状態をリモートリポジトリに送信する
👉 GitHub を見ると、コミット者・コミットメッセージ・コミット内容が表示される

```bash
git push origin
```

## 変更内容を GitHub に反映するまでの流れ一例

- 変更内容をインデックスにステージングする: `git add .`
- 変更内容をコミットする: `git commit -m "コミットメッセージ"`
- コミット内容をリモートリポジトリに反映する: `git push origin`

## Branch Operation - ブランチ操作

### Branch
一覧表示：ローカルリポジトリのブランチを一覧表示する
👉 更に後にブランチ名を決めて入力すると、現在のリポジトリから、その名前で新しいブランチを作成する
👉 オプション指定することで、リモートブランチの一覧表示など他にも色んな操作ができる

```bash
git branch
```

### Checkout
ブランチ切り替え：
👉 指定したローカルブランチに切り替える。ローカルになければリモートブランチから取得してローカルにブランチ生成して切り替える。
👉 オプション指定することで、変更内容の取り消しなど他にも色んな操作ができる

```bash
git checkout {ブランチ名}
```

### Delete branch
ブランチ削除：指定したブランチをローカルリポジトリから削除する（リモートリポジトリからは消えない）

```bash
git branch -D {ブランチ名}
```

### Merge
マージ：現在のリポジトリに、指定したリポジトリの内容を取り込む

```bash
git merge {ブランチ名}
```
