# youtube-dl

## 特定のチャンネルの動画をすべてダウンロードする
`youtube-dl -f best -ciw -o "%(title)s.%(ext)s" -v 【チャンネルの URL】`

## テキストファイル内に列挙された URL をすべてダウンロードする
`youtube-dl -f best -a 【テキストファイルの名前】`