### 事前準備
 * gitクライアント
     * インストール(Windows)
     * http://code.google.com/p/msysgit/
     * Git-1.7.11-preview20120710.exe
     * git bashというやつを起動

 * githubアカウント
     * 公開鍵の設定
     * http://blog.glasses-factory.net/2011/08/16/github
     * study_gitのCollaboratorsに追加する

 * 初期処理・名前変更
     * $ git init
     * $ git config --global user.name "名前"
     * $ git config --global user.email "メールアドレス"

### ソースコードをチェックアウト

 * リモートリポジトリをローカルにクローンする
     * $ git clone https://github.com/yatemmma/study_git.git
     * $ cd study_git


### ファイルを修正する
 * index.htmlファイル修正
 * $ git status
 * $ git diff index.html
 * $ git commit index.html
 * $ git status
 * $ git push

### ローカルのファイルを最新化する
 * $ git pull

### ファイルを追加する
 * ファイルを新規作成 username.html
 * $ git status
 * $ git add username.html
 * $ git status
 * $ git commit username.html
 * $ git status
 * $ git push

### 変更を元に戻す
 * username.htmlを修正
 * $ git status
 * $ git diff index.html
 * $ git checkout username.html
 * $ git status

### ブランチを作成する
 * $ git pull
 * $ git status
 * $ git branch
 * $ git branch -a
 * $ git push origin master:username-branch
 * $ git status
 * $ git branch
 * $ git branch -a

### 現在いるブランチを切り替える
 * $ git status
 * $ git checkout username-branch
 * $ git status
 * $ git branch

### ブランチの修正をpushする

### ファイルを追加する
### ファイルを削除する

### コミットをやめる
### コメントを修正する
### マージする

