# 文字コード

文字や記号をコンピュータ上でデータとして扱うために、
一文字ずつ固有の識別番号を与えて区別できるようにした符号のこと。

- 固有の識別番号とは
  - たとえばASCIIであれば、
  アルファベットの大文字のAは65番(ビット列で1000001) など
  - バイト表現と文字を紐づけてしている

## 文字コードの例

- ASCII
- Shift_JIS
- Unicode
  - UTF-8

## 所感

- なにかおまじないのようにShift_JISやUnicodeというものを
理解していたが、あるテキストファイルがあったときに
その保存されたテキストの文字コードとそのファイルを
読み出すときに指定する文字コードが違っていた場合、
そもそもバイトのグループを全く違う形式で扱ったり、
対応する文字が異なっていたりするために
文字化けやエラーが起こるのだということがわかった。
