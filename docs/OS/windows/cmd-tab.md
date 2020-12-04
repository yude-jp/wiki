# コマンド プロンプトでTab補完が効くようにする

何らかのきっかけでコマンド プロンプトにおける補完が効かなくなることがある。

## 解決法
* レジストリを修正する。  

|  種類  |  パス  |
| ---- | ---- |
|  全ユーザー  |  \HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Command Processor  |
|  ユーザー毎  |  \HKEY_CURRENT_USER\SOFTWARE\Microsoft\Command Processor  |

|  キー  |  値  |
| ---- | ---- |
|  CompletionChar  |  4 または 6 または 9  |
|  PathCompletionChar  |  4 または 6 または 9  |

それぞれ 4: Ctrl + D、6: Ctrl + F、9: Tab で入力補完となる。
