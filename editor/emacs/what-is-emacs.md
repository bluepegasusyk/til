#emacsとは

## 概要

テキストエディターのひとつ。
しかし、lispマシンでもあり、アプリケーションとして、emacs内でさまざまなことができる。
- webブラウザでメールを送ったりTwitterを見たりウェブサイトを見たり、あるいはファイルを開いたりできるのと同様である
- emacs環境内にもさまざまなアプリケーションが存在する
  - メーラ、カレンダー、Twitterクライアント、ファイラなど

## emacsの利点

1. 文字入力が一元化できること
2. 外部プログラムとの連携が容易であること
3. 拡張言語がLISPであること

### 文字入力が一元化できる

- エディタで使用しているコマンドで、プログラミング、文書作成、Twitterやメッセージ入力を同じように行うことができる
  - 具体例
    - 基本的に、ほかのエディタを使っている場合、ブラウザ、メール、スカイプ, etcetcと、たくさんのアプリケーションを別ウィンドウで開くことになる。画面を行ったり来たりするのは面倒だし、エディタで使える便利コマンドがほかでは使えないことが面倒
    - emacsを使えば、普段エディタで使っている文字入力方法やコマンドを「文字入力をする全ての場面で｣ 使用可能となる

### 外部プログラムとの連携

- プロセスを扱う機能が存在する
- 外部プログラムを呼び出してその結果を処理することで、あたかもEmacs組み込みの機能であるかのように動作してくれる
- 具体例
  - シェルコマンドの実行結果の表示・挿入、シェルなどの対話的プログラムを動かすことができる
  - emacsからプログラムを使いやすくするコマンドの存在

### emacs lispの存在

なにが嬉しいのか?
- lispの考え方を学べること!
  - lispは現在のプログラミング言語の多くに影響を与えているので、lispを学ぶことでプログラミング言語をより深く理解できる
  - 関数型プログラミングを学ぶことができる



