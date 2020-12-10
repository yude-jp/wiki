# 公開鍵認証 (SSH) 周りのトラブル

## 権限設定
大半のWebサイトでは、`.ssh/authorized_keys`周りの権限設定を重視するが、ホームディレクトリ自体の権限設定も重要である。
```
sudo chmod 600 ~/.ssh
sudo chmod 600 ~/.ssh/authorized_keys
sudo chmod 755 ~/
```
最後の1行も重要。`777`等になっていると、永久的に`authorized_keys`は無効化される。