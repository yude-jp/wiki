# Ubuntu デスクトップ

## Chrome をダークモードにする
### 手段 1
`/opt/google/chrome/google-chrome` の最終行を下記のように変更する。
```
exec -a "$0" "$HERE/chrome" "--enable-features=WebUIDarkMode" "--force-dark-mode" "$@"
```

### 手段 2
起動する際に、引数に `--enable-features=WebUIDarkMode --force-dark-mode` を追加する。