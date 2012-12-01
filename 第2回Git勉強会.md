### 第2回Git勉強会

#### 事前準備

* [事前準備.md](https://github.com/yatemmma/study_git/blob/master/%E4%BA%8B%E5%89%8D%E6%BA%96%E5%82%99.md)の内容をやっておくこと！

#### Gitを使ってみよう！

* git config
  * 色を付ける
     * $ git config --global color.status auto
     * $ git config --global color.diff auto
     * $ git config --global color.branch auto
     * $ git config --global color.interactive auto
     * $ git config --global color.grep auto
  * alias
     * $ git config --global alias.st status
     * など
  * 参考サイト
     * http://yuroyoro.hatenablog.com/entry/20101008/1286531851

* 現在の作業状態を確認
  * $ git status
     * ローカルリポジトリ
     * インデックス(緑)
     * ワーキングツリー(赤)

* ワーキングツリーからインデックスに追加する
  * $ git add
     * $ git add filename.txt
     * $ git add dirname
     * $ git add .
     * $ git add --all

* 差分確認
     * $ git diff # ワーキングツリーとインデックスの差分
     * $ git diff filename
     * $ git diff dirname
     * $ git diff ハッシュ値 ハッシュ値
     * $ git diff --cached # インデックスとローカルリポジトリ
     * $ git diff HEAD # ワーキングツリーとローカルリポジトリ

* ローカルリポジトリにコミット
     * $ git commit 
     * $ git commit -a
     * $ git commit filename.txt
     * $ git commit --amend
     * $ git commit --amend # ファイルを修正してaddしてから。直前のコミットやり直し

* コミット履歴を確認する
  * $ git log
  * $ git log ハッシュ値..ハッシュ値
  * $ git log ハッシュ値..
  * $ git log ..ハッシュ値 # HEAD..ハッシュ値
  * $ git log -p
  * $ git log -3
  * $ git log -1 ハッシュ値 # ハッシュ値からN個のログを表示
  * $ git log --oneline
