# helix-editorにmarkdown関連の設定を追加する

## 1. プレビューを表示したい
1-1  [cargoをインストールする](https://doc.rust-lang.org/cargo/getting-started/installation.html)

- install後は、shellを再起動する

1-2 [mdplsをインストールする](https://github.com/euclio/mdpls)

1-3 [設定に追記する](https://github.com/helix-editor/helix/issues/2824)

helixの設定は`~/.config/helix`にある
- `languages.toml`ファイルがなければ、そのフォルダに追加する

```toml
[[language]]
  name = "markdown"
  language-server = { command = "/path/to/mdpls" }
  config = { markdown.preview.auto = true, markdown.preview.browser = "firefox" }
```
        
- `path/to`部分にはmdplsのpassを入れる
  - `which mdpls`コマンドでpassを表示できる
  
  
  
## 2. シンタックスハイライトをかけたい
...と思ったが、1.を設定したらハイライトがかかってしまったので解決
