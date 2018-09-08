## golangマスターになる！！
---
## 自己紹介
<div><img src="https://avatars3.githubusercontent.com/u/2528278?s=460&v=4" style="width:20%" /></div>
- 名前: 安尾 友佑
- 年齢: 30歳 <!-- .element: class="fragment" -->
- 出身: 三重 <!-- .element: class="fragment" -->
- 趣味: 子供、アニメ・漫画、（サッカー） <!-- .element: class="fragment" -->
- 好きなアニメ: 化物語、Re:ゼロ、弱虫ペダル <!-- .element: class="fragment" -->

---
## 目標
- vimでgoの開発を行う準備をする<!-- .element: class="fragment" -->
- golangでREST APIを実装してみる<!-- .element: class="fragment" -->
- MySQLへ読み書きする<!-- .element: class="fragment" -->
- redish-apiの一部を置き換える<!-- .element: class="fragment" -->
- Docker化<!-- .element: class="fragment" -->
- Deploy!<!-- .element: class="fragment" -->

---
## いきなり脱線
- スライドどうやって作ろう...<!-- .element: class="fragment" -->
- 今まではGoogle Slideで作っていたけど......<!-- .element: class="fragment" -->
- もっとできるエンジニア感を出していきたいw<!-- .element: class="fragment" -->

---
## 目標
- vimでgoの開発を行う準備をする<!-- .element class="cancel" -->
- golangでREST APIを実装してみる<!-- .element class="cancel" -->
- MySQLへ読み書きする<!-- .element class="cancel" -->
- redish-apiの一部を置き換える<!-- .element class="cancel" -->
- Docker化<!-- .element class="cancel" -->
- Deploy!<!-- .element class="cancel" -->
- JSライブラリを使って資料を作る<!-- .element: class="fragment em" -->

---
## ライブラリ選定
なんか色々あるらしい
- reveal.js
- remark.js
- Marp
- Swipe
- Qiita

今回はreveal.jsで作ってみることに<!-- .element: class="fragment em" -->

---
## reveal.jsとは
- 綺麗で手軽にスライドを作成できるフレームワーク
- https://revealjs.com/#/

---
## 使い方
- インストール ~ サーバー起動
<pre>
  <code class="shell">
    $ git clone https://github.com/hakimel/reveal.js
    $ npm install
    $ npm start
  </code>
</pre>

---
## Markdownで書く準備
- index.htmlのbody内を編集
<pre>
  <code class="html">
    <div class="reveal">
      <div class="slides">
        <section data-markdown="slide.md"
                 data-separator="^---"
                 data-separator-vertical="^--"
                 data-notes="^Note:"
                 data-charset-"utf-8">
        </section>
      </div>
    </div>
  </code>
</pre>

---
## あとはMarkdownで書くだけ
<pre>
  <code class="shell">
    ## golangマスターになる！！
    ---
    ## 自己紹介
    <div><img src="https://avatars3.githubusercontent.com/u/2528278?s=460&v=4" style="width:20%" /></div>
    - 名前: 安尾 友佑
    - 年齢: 30歳
    - 出身: 三重
    - 趣味: 子供、アニメ・漫画、（サッカー）
    - 好きなアニメ: 化物語、Re:ゼロ、弱虫ペダル 

    ---
    ## 目標
    - vimでgoの開発を行う準備をする
    - golangでREST APIを実装してみる
    - ORマッパーを使ってMySQLへ読み書きする
    - redish-apiの一部を置き換える
  </code>
</pre>

---
## ここからはgolangの話
すでに15:37...

---
<div><img src="https://saruwakakun.com/wp-content/uploads/2017/07/f40f559f.jpg" style="width:80%" /></div>

---
## vimでgoの開発をする準備
- vim-goというのがあるらしい
  - https://github.com/fatih/vim-go

---
## vim-goのインストール
- .vimrcに以下を追記し、:GoInstallBinaries
<pre>
  <code class="shell">
    call dein#add('fatih/vim-go')
  </code>
</pre>
- vim-goの日本語版のチュートリアルも参考になった
  - https://github.com/hnakamur/vim-go-tutorial-ja

---
## vim-goの感想
- go拡張子のファイルを作成すると勝手にコードが書かれてビビった<!-- .element: class="fragment" -->
- GoFmt最強<!-- .element: class="fragment" -->
- GoDocめちゃ便利<!-- .element: class="fragment" -->

---
## REST APIの実装（16:25〜）
- 参考サイト
  - http://sgykfjsm.github.io/blog/2016/03/13/golang-json-api-tutorial/
- 成果物
  - https://github.com/yusukeyasuo/go-api-example
