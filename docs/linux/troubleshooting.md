# トラブルシューティング

## 外付けハードディスク等が読み取り専用になってしまうときの問題の切り分け
* `dmesg | tail`

## rdesktop で音を出したい
* 起動オプションに `-r sound` を追加する。

## 強制的にマウントを解除したい
**オプション: `-l` を用いれば良い。**  
これは、例えば google-drive-ocamlfuse のリードが追いつかなくなって固まった時に有用。  
e.g. `sudo unmount -l ~/gdrive`

## byobu 越しにファンクションキーが使えなくなった
* 参考: [putty越しのbyobuでF2,F3,F4,が効かない | plastic skies](https://renidentia991.wordpress.com/2013/01/21/putty%E8%B6%8A%E3%81%97%E3%81%AEbyobu%E3%81%A7f2f3f4%E3%81%8C%E5%8A%B9%E3%81%8B%E3%81%AA%E3%81%84/)  

PuTTY の設定において、Terminal --> Keyboard --> The function keys and keypad を Xterm R6 に指定する。