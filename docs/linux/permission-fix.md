# 誤って "/" 以下のパーミッションを破壊してしまったとき

## 参考
* [誤って” / “以下のパーミッションを一括で変更した場合の対処法 – http://wp.bmemo.pw](https://t.co/SnbD2sxEWo?amp=1)

## 本文
まず、Live CDなどで起動し、sudo が使えるようにする。
実行するべきコマンド:

* `chmod -R go-w /bin`
* `chmod -R go-w /etc`
* `chmod -R go-w /boot`
* `chmod -R go-w /dev`

特殊なパーミッションを持つディレクトリについて:

* `chmod 440 /etc/sudoers`
* `chmod 440 /etc/sudoers.d/README`
* `chmod 755 /etc/sudoers.d`
* `chmod 640 /etc/shadow /etc/gshadow`
* `chmod 600 /etc/ssh/*_key`
* `chmod 600 /etc/ssh*key`
* `chmod 710 /etc/ssl/private`
* `chmod 710 /etc/cups/ssl`
* `chmod 1777 /tmp /var/tmp /var/lock`
* `chmod 4755 /bin/su /usr/bin/passwd /usr/bin/sudo /usr/bin/sudoedit`
* `chmod 2755 /var/mail /var/spool/mail`