# PostgreSQL

## 鍵の権限がないと怒られる。
これはバグらしい？  

* 参考: [FATAL: could not access private key file “/etc/ssl/private/ssl-cert-snakeoil.key”: Permission denied | Stack Overflow](https://t.co/SnbD2sxEWo?amp=1)  

下記コマンドで修正する。
```
chown postgres:ssl-cert /etc/ssl/private/
chown postgres:postgres /etc/ssl/private/ssl-cert-snakeoil.key
```