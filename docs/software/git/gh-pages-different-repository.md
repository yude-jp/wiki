# 別リポジトリにあるディレクトリを他のリポジトリで既に使用中のドメインのサブディレクトリとしてGitHub Pagesで公開する

## 解決法
* gh-pages ブランチ (または公開したいブランチ) を submodule として追加する。  

    1. まず、使用中のドメインのディレクトリに入る。
    1. 以下のコマンドを実行する。  
        ```
        git submodule add -b gh-pages (別リポジトリにあるディレクトリ) ./(公開するサブディレクトリの名前)
        ```
