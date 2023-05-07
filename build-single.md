# 基板1枚でつくる

## 組み立てに必要なもの

### 道具

迷った場合は[遊舎工房さんの工具セット](https://shop.yushakobo.jp/products/a9900to)を購入すると良いかと思います。  
以下の道具も基本的には上述のセットを抜粋したリストとなります。

|道具|備考|
|:--|:--|
|ハンダごて|おすすめは[HAKKO FX-600](https://www.hakko.com/japan/products/hakko_fx600.html)です。[こて台](https://www.hakko.com/japan/products/hakko_kote_board.html)もあると、より作業をスムーズに進められます。|
|ハンダ|[こちら](https://www.goot.jp/products/detail/se_06008)などを使う方が多いようです。|
|ピンセット|100均などで手に入るものでも充分利用できるかと思います。|
|ニッパー|100均などで手に入るものでも充分利用できるかと思いますが、1000円程度ものを買っても損では無いかと思います。|

### 必須部品

|部品|個数|備考|
|:--|:--|:--|
|基板|1||
|Pro Micro|1||
|Cherry MX互換キースイッチ|13||

### あるとより良い部品

|部品|個数|備考|
|:--|:--|:--|
|コンスルー|2||
|リセットスイッチ|1||
|LED(SK6812MINI-E)|6||
|ゴム足シール|4~6|100円ショップなどで売っているものを取り付けることはできますが、グリップ力が弱い製品もありますので[こちら](https://shop.yushakobo.jp/products/a0800ur-01-6)等を購入するのが良いかと思います。|

## 組み立て手順

### 1. 基板の表裏を確認する

Baumkuchenはリバーシブル基板です。
Pro Micro(USB取り付け部分)をキーボードのどちら側に取り付けるかで基板の表裏が決まります。

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4708_2.jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4709_2.jpg?raw=true" width = "600px" />

以下の説明はPro Microをキーボードの右側に取り付ける場合で説明を進めます。

### 2. Pro Microを取り付ける

Pro MicroはキーボードのMCU(Micro Controller Unitの略)で平たく言うと、キーボードの頭脳部分です。  
キーの入力をPCやタブレットに伝達する役割があります。

Pro Microは取り付け位置で表裏が変わります。

基板の右側にPro Microを取り付ける場合は、平たい面が上に向くようにします。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4567.jpg?raw=true" width = "600px" />

基板の左側にPro Microを取り付ける場合は、チップなどが乗っている面を上に向くようにします。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4566.jpg?raw=true" width = "600px" />

Pro Microと基板を繋ぐには[コンスルー]()を使用するのがオススメです。  
ピンヘッダというパーツを用いて基板とPro Microをハンダ付けする方法もありますが、Pro Microが壊れた時に交換が難しくなります。  
コンスルーをPro Microにハンダ付けすると、基板への取り付けはハンダ付けをせずとも挿し込むだけで良いので交換が容易になります。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4568.jpg?raw=true" width = "600px" />

コンスルーには向きがあります、詳しくは[こちら](https://yushakobo.zendesk.com/hc/ja/articles/360044233974-%E3%82%B3%E3%83%B3%E3%82%B9%E3%83%AB%E3%83%BC-%E3%82%B9%E3%83%97%E3%83%AA%E3%83%B3%E3%82%B0%E3%83%94%E3%83%B3%E3%83%98%E3%83%83%E3%83%80-%E3%81%AE%E5%8F%96%E3%82%8A%E4%BB%98%E3%81%91%E6%96%B9%E3%82%92%E6%95%99%E3%81%88%E3%81%A6%E4%B8%8B%E3%81%95%E3%81%84#:~:text=%E3%82%B3%E3%83%B3%E3%82%B9%E3%83%AB%E3%83%BC%EF%BC%88%E3%82%B9%E3%83%97%E3%83%AA%E3%83%B3%E3%82%B0%E3%83%94%E3%83%B3%E3%83%98%E3%83%83%E3%83%80%EF%BC%89%E3%81%AE%E5%8F%96%E3%82%8A%E4%BB%98%E3%81%91%E6%96%B9%E3%82%92%E6%95%99%E3%81%88%E3%81%A6%E4%B8%8B%E3%81%95%E3%81%84,-%E9%81%8A%E8%88%8E%E5%B7%A5%E6%88%BF&text=%E3%82%B3%E3%83%B3%E3%82%B9%E3%83%AB%E3%83%BC%E3%81%AF%E9%87%91%E8%89%B2%E3%81%AE%E7%AA%93,%E3%82%92%E6%8F%83%E3%81%88%E3%81%A6%E5%B7%AE%E3%81%97%E8%BE%BC%E3%81%BF%E3%81%BE%E3%81%99%E3%80%82)の記事を御覧ください。

基板にコンスルーを差し込みます。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4578.jpg?raw=true" width = "600px" />

コンスルーにPro Microを載せます。Pro Microを基板の左側に置く場合はPro Microの表裏を写真とは反対にしてください。
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4579.jpg?raw=true" width = "600px" />

コンスルーとPro Microをハンダ付けします。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4584.jpg?raw=true" width = "600px" />

ピンヘッダを用いる場合は基板とピンヘッダをハンダ付けします。

### 3. リセットスイッチの取り付け

リセットスイッチは、Pro Microにファームウェアを書き込む際などに押すスイッチです。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4586.jpg?raw=true" width = "600px" />

Pro Microの配置箇所の反対側にあります。「RESET」と書かれた箇所です。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4710.jpg?raw=true" width = "600px" />

この二つの穴同士を繋ぐとリセットスイッチを押したことになります。金属製のピンセット等で通電させることでリセットスイッチを押したことと同じ挙動をします。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4711.jpg?raw=true" width = "600px" />

余談ですが、Pro MicroのRSTとGNDのピン同士を通電させると、リセットスイッチを押したことと同様になります。こちらもピンセットやドライバー等を用いて代用できます。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4712.jpg?raw=true" width = "600px" />

以上のことから、リセットスイッチを取り付けることは必須ではありません。  
ただ、スイッチを押すだけで動作するというのは便利ではありますので、迷ったら取り付けることをオススメします。  
以下は取り付けの手順となります。  

基板の表側からリセットスイッチの足を穴に差し込みます。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4587.jpg?raw=true" width = "600px" />

基板の裏側からリセットスイッチの足が出ていることを確認します。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4590.jpg?raw=true" width = "600px" />

リセットスイッチの足と基板をハンダ付けします。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4591.jpg?raw=true" width = "600px" />

ハンダ付けしたリセットスイッチの足をニッパーで短くしておくと、安定性が増します。
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4593.jpg?raw=true" width = "600px" />

### 4. ファームウェアの書き込み
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

### 5. キースイッチの取り付け

BaumkuchenマクロパッドはCherry MX互換キースイッチを取り付けることができます。  
お好みのキースイッチを13個用意してください。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4595.jpg?raw=true" width = "600px" />

キースイッチを基板に載せます。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4596.jpg?raw=true" width = "600px" />

そのままでは
そのままでは直ぐに

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4597.jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_ .jpg?raw=true" width = "600px" />
