# MySQL

## パスワードが合っているにも関わらず、接続に失敗する。
* バージョンが新しくなったことで生まれる不具合。  
mysql にログインした後、以下のコマンドを実行する。
```
grant all privileges on *.* to 'user'@'localhost' with grant option;
```
オプションは適宜変更する。
