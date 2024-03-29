
#### 自己紹介

杉本 雅広（すぎもと まさひろ）

WebGL に関するサイトやスクールの運営などをしているおじさんです。

![](sample.png)

---

#### もくもく会の前に

Web3D でもくもくしようという本日の企画。

既にみなさん自分のもくもくネタをお持ち寄りのこととは思うのですが……

---

#### もくもく会の前に

ぶっちゃけあんまり具体的に作業内容決めてきてない、という人がもしかしたらいるかもしれないので、私のほうで WebGL やら GLSL やら、ブラウザベースの 3D テクノロジーについて超簡単にですが、さらりと解説しておこうと思います。

もし気になるテーマがあったら、今日の作業に割り振ってみても、いいかもしれません。

---

#### WebGL

WebGL は JavaScript の API として、ブラウザに組み込まれています。

特にプラグインなどが無くても実行できるのは、ブラウザのなかで動く JavaScript のエンジンそのものが WebGL を解釈して実行することができるからです。

---

#### WebGL

ですから WebGL の開発環境は、通常の JavaScript での開発環境と基本的には変わりません。

最近では WebGL を実行できないブラウザというのは、メジャーなところではほぼ無いので、気軽に開発を始めることができます。

---

#### GLSL

GLSL は WebGL で使われる「シェーダ」という概念を操作するために必要な、シェーダを記述するための言語です。

GLSL 単体での開発というのは、厳密に言うとあり得ないのですが、ベースとなる WebGL の実行環境が既にブラウザ上に用意されていて、そこでシェーダだけを書いていろいろ遊んだりすることもできます。

glslsandbox などが有名ですね。

---

#### three.js

mr.doob 氏が作った WebGL のラッパーライブラリ。ちなみに、glslsandbox も氏の手によるもの。

まあ世の中の WebGL 関連作品の九割以上はコレ使ってるでしょう。

つまり、かなり WebGL が扱いやすくなるライブラリですね。

---

#### 最近のびっくり WebGL 案件

独断と偏見により選ばれた WebGL 案件のご紹介。

選定基準は、3D 野郎だろうがそうでなかろうが、ぱっと見ですごいと思うんじゃないかなというやつ。

<span class="capt">ちなみに 3D 野郎は基本的にすごいと感じるところが一般人とかなり違いますね……</span>

---

#### 最近のびっくり WebGL 案件

<a href="http://www.adultswim.com/toonami/" target="_blank">Toonami - Saturday Nights on Adult Swim</a>

アメリカのアニメ専門チャンネルの特設サイト。

---

#### 最近のびっくり WebGL 案件

<a href="http://mondialautomobile.bmw.fr/en" target="_blank">BMW - Paris Motorshow 2016</a>

BMW のデジタルショールーム。

---

#### 最近のびっくり WebGL 案件

<a href="https://www.collectivei.com/" target="_blank">Collective Intelligence</a>

ハイセンスすぎる企業のウェブサイト。

---

#### 最近のびっくり WebGL 案件

<a href="https://www.dewanddoritos.com/" target="_blank">Fuel Your Titan</a>

ノイズのポストエフェクトを無駄に使いまくる。

---

#### 最近のびっくり WebGL 案件

<a href="http://www.duhaihang.com/archive/dev-random-notes-2016/" target="_blank">DEV # RANDOM NOTES - WebGL Playground and Interactive Experiments</a>

ハイセンスで技術力もあるとか反則だろ事案。

---

#### WebGL で 3D に挑戦していくスタンス

WebGL で 3D プログラミング始めてみるというのは、とてもいい考え方だと思います。

C++ で OpenGL 実装とかゼロから作っていくのに比べたら、百倍はらくちんです。

---

#### WebGL で 3D に挑戦していくスタンス

ただし、WebGL を大きなテーマと捉えた場合でも、付き合い方にはいろいろあると思います。

* フルスクラッチで WebGL でゴリ押しする

<span class="capt">おすすめ度：★★☆☆☆</span>

<span class="capt">普通に 3DCG エンジニアになる覚悟が必要</span>

---

#### WebGL で 3D に挑戦していくスタンス

* three.js を使ってまずは触ってみる

<span class="capt">おすすめ度：★★★★☆</span>

<span class="capt">jQuery みたいなもんです</span>

---

#### WebGL で 3D に挑戦していくスタンス

* three.js を使ってなんかカスタムシェーダとかする

<span class="capt">おすすめ度：★★★☆☆</span>

<span class="capt">この世界で勝負するなら使いこなせなきゃ無理！</span>

---

#### WebGL で 3D に挑戦していくスタンス

* ゲームエンジンとか使ってみちゃう

この場合はゲームエンジンの特性をきちんと理解することも求められる。

<span class="capt">おすすめ度：★★★☆☆</span>

<span class="capt">エンジンによっていろいろ違ってきます</span>

---

#### WebGL で 3D に挑戦していくスタンス

* 神々が棲むというシェーダ神界を目指す

参考： Shadertoy

<span class="capt">おすすめ度：🔥 🔥 🔥 🔥 🔥 </span>

<span class="capt">チカラがほしいか？</span>

---

#### 要するに

Web で 3D を実現する方法には、こうしなければならないというルールはなく、最近では選択肢も様々あります。

また、最終的にどのように使われるのかによっても、かなり実装が違ってきます。

---

#### 要するに

モバイル端末でも動作するようにしなければならないとか、ハイエンドマシンで動く半ばネイティブアプリみたいな体裁のものであるとか、本当にいろいろなところで WebGL が使われるようになってきています。

最終的に自分がどのようなものを、なんのために実装したいのか。

これをしっかり把握した上で、適宜、手法なり勉強内容なりを取捨選択していくのがいいと思います。

---

#### 大事なのは楽しくやること

大事なのは、楽しくやること。

そのためにも、わからんことはぶっちゃけ聞いたほうが早いということも多いです。

---

#### 大事なのは楽しくやること

ぜひ気軽に質問してください。

わかることなら、答えますので。

<span class="capt">注：このおじさんは three.js 使えません！</span>

---

#### 大事なのは楽しくやること

enjoy!

---


