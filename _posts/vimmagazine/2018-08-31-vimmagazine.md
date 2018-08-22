---
layout: vimmagazine
category: vimmagazine
title: Vim Magazine 2018 年 08 月号

---

## 話題

*   [Asakusa.vim #3](https://asakusavim.connpass.com/event/95401/) が 2018-08-03 (金) に二子玉川で開催されました
*   [meguro.vim #11](https://megurovim.connpass.com/event/94477/) が 2018-08-11 (土) に開催されました
*   [VimConf 2018](https://vimconf.org/2018/) 関連
    *   VimConf 2018 が 2018-11-24 に秋葉原のアキバPLAZAで開催されます
    *   VimConf 2018 に登壇して発表するためのCFPが2018-08-13 (月)に締め切られました
*   [コミックマーケット94](https://www.comiket.co.jp/)にて[スパルタンVim 7.0](https://twitter.com/kaoriya/status/1027415480670158848)が[発売](https://twitter.com/kaoriya/status/1027701062264807424)されました

## 今月の新機能

今月の新機能及びユーザーに影響のある変更は以下のとおりです。

*   8.1.0232: if_ruby 実行中にエラーが起きた場合、そのバックトレースが Vim のコマンドラインに表示されるようになりました
*   8.1.0251: `set backupdir=~/vimbackupdir//` のように指定すると、`~/vimbackupdir/` 以下にファイルのフルパスが連結されたファイル名で書き出されるようになりました
    *   例: 上記の設定を行った際、ファイル `/home/vim/vimrc` のバックアップファイルは `~/vimbackupdir/%home%vim%vimrc{backupext}` となります (`{backupext}` = `'backupext'` オプションの値)
    *   スワップファイルの場合は以前から可能です `set directory=~/swapdir//`
*   8.1.0253: タイトルスタックに対応した端末では、端末のタイトルが正しく復帰されるようになりました
    *   参考記事: [「Vimを使ってくれてありがとう」にさようなら](https://qiita.com/ttdoda/items/903e85f07d58018c851d)
*   8.1.0263: チャンネルのログにどのパート ("sock", "out", "err", "in") かの情報が出力されるようになりました
*   8.1.0271: `'incsearch'` オプションが `:s`, `:g`, `:v` コマンドでもサポートされ、パターン入力中にマッチした箇所にジャンプするようになりました (関連: 8.1.0273,0274,0277)
*   8.1.0305: Lua 5.4 32 ビットがサポートされました
*   8.1.0307: ウィンドウレイアウトを取得する `winlayout()` 関数が追加されました
*   8.1.0313: スワップファイルの情報を取得する `swapinfo()` 関数が追加されました



## Vimに関する脆弱性

特筆すべき脆弱性の報告はありませんでした。