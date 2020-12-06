# VMware Workstation Player で Windows 9x 系を動かす

## 知見
* FreeDOS でも動かすことはできる。
* 予め仮想ハードディスクを Windows XP 等から FAT でフォーマットしておく。
* フォーマットした仮想ハードディスクに MS-DOS 6.22 (または [FreeDOS](https://www.freedos.org/download/)) と Windows 95 のセットアップディスクの中身を移しておき、それらを DOS から実行すると、ディスクドライブ等のドライバーに悩まされることがない。
* セットアップ終了後フロッピードライブを切断しないと DOS の画面に戻って起動できなくなる。 (?)
    * プロンプトされるのでそのタイミングで切断すれば良い。
* 万一の時のために起動ディスクは作成しておくべきである。
    * VMware の `flp` ファイルで良い。
    ![作成](../../assets/images/win95_rundisk.png)

## 音が出ない
* VMware Tools をインストールしても、サウンドドライバーはインストールされない。
* 以下の方法では MIDI の音が出ないかもしれないが、起動音や音声ファイル等に関しては再生できる。
* 参考: [VMWare に入ったWindows 95用のサウンドドライバ - Windows 2000 Blog](http://blog.livedoor.jp/blackwingcat/archives/1434847.html)
* `ES1371` という型番のデバイスのドライバーをインストールすればよい。
    * ダウンロード先: [Creative Media (Japan) : Customer Support - Drivers & more for all your Creative products](https://jp.creative.com/support/downloads/download.asp?Product_ID=420&Product_Name=Creative+Ensoniq+Audio+PCI&OSName=Windows+98&OS=2&DriverType=0&details=1)
    ![ここ](../../assets/images/ES1371.png)

## インターネットに接続する
行い  
![手順](../../assets/images/win95_tcpip.png)

### Internet Explorer 4.0 で接続できた Web サイトの一覧
HTTPS 接続の Web サイトには接続できない。

* [ようこそ AMAKATAs' WEBSITE へ](http://www.asahi-net.or.jp/~mi5k-amkt/)
* [1998特報!!倶楽部](http://www.big.or.jp/~talk/t-club/)
* [ようこそ「ｍａｒｉａ」のホームページヘ](http://www009.upp.so-net.ne.jp/maria/index.htm)
* [阿部寛のホームページ](http://abehiroshi.la.coocan.jp/)
* [侍魂](http://www6.plala.or.jp/private-hp/samuraidamasii/tamasiitop/tamasiitop.htm)
* [kota'sHomePageへようこそ](http://www5.airnet.ne.jp/kota/)
* [ようこそ、幸子のホームページへ](http://ftp.fuchu.or.jp/~sachiko3/index.htm)

`’s home page　ようこそ` で [Google 検索](https://www.google.co.jp/search?client=ubuntu&hs=uxn&channel=fs&hl=ja&sxsrf=ALeKk01iTVeg26WWFYNkk42VpSmHcECkug%3A1607224198259&ei=hkvMX5qgD4nv-Qa23JH4CA&q=%E2%80%99s+home+page%E3%80%80%E3%82%88%E3%81%86%E3%81%93%E3%81%9D&oq=%E2%80%99s+home+page%E3%80%80%E3%82%88%E3%81%86%E3%81%93%E3%81%9D&gs_lcp=CgZwc3ktYWIQAzIECCMQJzoHCAAQsAMQHlDQDljQDmCNHmgBcAB4AIABXYgBXZIBATGYAQCgAQKgAQGqAQdnd3Mtd2l6yAEBwAEB&sclient=psy-ab&ved=0ahUKEwia-6TbsLjtAhWJd94KHTZuBI8Q4dUDCA0&uact=5) を行うと、たくさん出てくる。  
参考: [懐かしの90年代（〜2000年代初頭）ホームページ](https://miz2403.com/nineties/)
