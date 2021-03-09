# youtube-dl

## 特定のチャンネルの動画をすべてダウンロードする
`youtube-dl -f best -ciw -o "%(title)s.%(ext)s" -v 【チャンネルの URL】`

## テキストファイル内に列挙された URL をすべてダウンロードする
`youtube-dl -f best -a 【テキストファイルの名前】`

## プレイリストを一括でダウンロードする。
`youtube-dl -i -f bestvideo+bestaudio 【URL】`  
`bestvideo+bestaudio` オプションにより、最高画質のファイルと最高音質のファイルが ffmpeg によって結合される。

## 動画のwavファイルをほぼ最高音質でダウンロードする。
`youtube-dl -f bestaudio --extract-audio --audio-format wav --audio-quality 0 【URL】`