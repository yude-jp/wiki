# SSH 接続を簡単にする
* `ssh cherry` とタイプするだけで接続できるようになります。

1. 設定ファイルを作成する。
以下のディレクトリ内に `config` ファイルが無ければ、作成します。
* Windows: `%USERPROFILE%\.ssh`
* Linux / macOS: `~/.ssh`

2. 設定する。
以下の内容を `config` ファイルに追記、または編集します。適宜中身を変更してください。
```
Host (名前、ssh 【ココ】に使用します。)
  HostName (宛先サーバーのIPアドレス または ホスト名)
  User (ユーザー名)
  IdentityFile (公開鍵認証に使用する秘密鍵)
```
