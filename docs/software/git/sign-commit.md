# コミットに署名を行う

* 参考: [Git Commit で OpenPGP 署名を行う — OpenPGP の実装 | http://text.Baldanders.info](https://text.baldanders.info/openpgp/git-commit-with-openpgp-signature/)

    1. Chocolatey などから Gpg4Win をインストールする。  
        `choco install gpg4win`  
    1. 鍵を生成する。 gpg --gen-key --> 表示されたものに従う。  
    1. PC に入っている鍵の一覧を表示させる。 `gpg --list-keys` --> 鍵のIDを確認する。  
    1. Git で指定した鍵を使うようにする。   
        `git config --global user.signingkey [先の手順で確認した鍵のID]`  
    1. コミット時に署名するようにする。   
        `git config --global commit.gpgsign true`
    1. **【重要】GitHub 等に鍵を登録する。 **  
        `gpg --armor --export [鍵のID]` でサイトに登録するべき文字列が表示されるので、コピペする。  
    1. __エラーが出た場合__
        `git config --global gpg.program "gpg コマンドの実行ファイルへのパス"` を実行してみる。