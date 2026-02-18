# Git 基本操作チートシート

Gitのワークフローとコマンドの備忘録。

## 🔄 基本ワークフロー
1. **Working Directory** (作業場所): ファイルを編集する
2. **Staging Area** (レジ前): `git add` でコミットする準備をする
3. **Local Repository** (保管庫): `git commit` で記録を残す
4. **Remote Repository** (共有場所): `git push` でGitHubへアップロード

## 🛠 主要コマンド
### 1. 状態の確認
- `git status` : 今、どのファイルが変更・追加されているか確認（一番よく使う！）
- `git diff` : 具体的にどの行を書き換えたか、差分を確認
- `git log` : これまでのコミット履歴を一覧表示

### 2. 記録の保存
- `git add .` : 全ての変更ファイルをステージングエリア（レジ）に送る
- `git commit -m "メッセージ"` : ステージングされた変更を正式に記録する

### 3. リモートとの連携
- `git push origin [ブランチ名]` : ローカルの記録をGitHubへ送る
- `git pull origin [ブランチ名]` : GitHubの最新の状態をローカルに取り込む

### 4. 設定
- `git config --global user.name "名前"` : ユーザー名の設定
- `git config --global user.email "メール"` : メールの設定
