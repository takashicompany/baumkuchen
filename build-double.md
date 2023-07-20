# 基板2枚でつくる

Baumkuchenの基板を2枚用いて組み立てます。PCBをスイッチプレートとして利用します。


<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4606.jpg?raw=true" width = "600px" />

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
|[Pro Micro](https://shop.yushakobo.jp/products/pro-micro)|1||
|[Cherry MX互換キースイッチ](https://shop.yushakobo.jp/products/cherry-mx)|13|互換スイッチであれば良いのでKailh製やGateron製なども取り付け可能です。|
|[M2 3.5mmスペーサー](https://shop.yushakobo.jp/products/a0800c2?variant=43940969316583)|4||
|[M2 3mm ネジ](https://shop.yushakobo.jp/products/a0800n2)|8||

### あるとより良い部品

|部品|個数|備考|
|:--|:--|:--|
|[コンスルー](https://shop.yushakobo.jp/products/31)|2|無くても完成しますが、コンスルーを用いたほうがメンテナンスが容易になります。詳細は[こちら](https://scrapbox.io/self-made-kbds-ja/%E3%82%B3%E3%83%B3%E3%82%B9%E3%83%AB%E3%83%BC)。|
|[LED(SK6812MINI-E)](https://shop.yushakobo.jp/products/sk6812mini-e-10)|6|光ります。組み立て後に取り付けも可能です。|
|ゴム足シール|4~6|100円ショップなどで売っているものを取り付けることはできますが、グリップ力が弱い製品もありますので[こちら](https://shop.yushakobo.jp/products/a0800ur-01-6)等を購入するのが良いかと思います。|

※ 2枚で組む場合は、タクトスイッチ(リセットスイッチ)は取り付けません。

## 組み立て手順

### 1. 基板の表裏を確認する

Baumkuchenはリバーシブル基板です。
Pro Micro(USB取り付け部分)をキーボードのどちら側に取り付けるかで基板の表裏が決まります。

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4708_2.jpg?raw=true" width = "600px" />

<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4709_2.jpg?raw=true" width = "600px" />

以下の説明はPro Microをキーボードの右側に取り付ける場合で説明を進めます。

### 2. Pro Microを取り付ける

2枚あるうちの1枚にPro Micro等を取り付けます。

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

https://user-images.githubusercontent.com/4215759/236684506-b55b27fb-9b54-4a46-b0fb-f98aaa532069.mov
  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4584.jpg?raw=true" width = "600px" />

ピンヘッダを用いる場合は基板とピンヘッダをハンダ付けします。

### 3. リセットスイッチについて

**Baumkuchen基板を2枚で組む場合はリセットスイッチの取り付けは行いません。** 

Pro Microの配置箇所の反対側にあります。「RESET」と書かれた箇所です。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4710.jpg?raw=true" width = "600px" />

この二つの穴同士を繋ぐとリセットスイッチを押したことになります。金属製のピンセット等で通電させることでリセットスイッチを押したことと同じ挙動をします。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4711.jpg?raw=true" width = "600px" />

余談ですが、Pro MicroのRSTとGNDのピン同士を通電させると、リセットスイッチを押したことと同様になります。こちらもピンセットやドライバー等を用いて代用できます。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4712.jpg?raw=true" width = "600px" />

### 4. ファームウェアの書き込み

ファームウェアをPro Microに書き込みます。  
ファームウェアはキーの入力の検知をしたり、LEDを点灯させたりといったキーボードを動作させるためのプログラムみたいなものです。  

Remapに動作テスト用のファームウェアを用意しておりますので、完成するまでは一旦こちらのファームウェアを使うと良いかと思います。  

Remapに対応したWebブラウザから[こちらのリンク](https://remap-keys.app/catalog/hN0gqZgFJvkWriQdhvu9/firmware)を開きファームウェアを書き込んでください。

テスト用ファームウェアのFlashをクリック。  
<img src = "https://user-images.githubusercontent.com/4215759/236663787-7b852bd0-583d-47ea-82c0-5c72c5ee7334.png" width = "600px" />

Bootloaderを選択してFlashをクリック。  
<img width="600px" alt="temp 2023-05-07 16 23 58" src="https://user-images.githubusercontent.com/4215759/236663906-1cad7cf1-b092-4b5b-b28c-21399186c32c.png">

Baumkuchenのリセットスイッチを押す・ピンセットなどで通電させると、Pro Microの端末が出てくるので選択して接続をクリック。
<img width="600px" alt="temp 2023-05-07 16 25 07" src="https://user-images.githubusercontent.com/4215759/236663913-9a135bc6-1e75-43ca-8ef8-50575b41ff6a.png">

書き込み終わるのを待ちます。  
<img width="600px" alt="temp 2023-05-07 16 25 56" src="https://user-images.githubusercontent.com/4215759/236663924-3b81ccca-e2ca-4f6d-bca0-ef6c0edc9a7d.png">

Successが表示されたらPro Microの書き込みが成功となります。

### 5. LEDの取り付け
BaumkuchenはLEDを取り付けて光らせることができます。

LEDは完成後でも取り付けられますので、後回しにしても大丈夫ですし必要ではない方はこの項目の作業をしなくてもOKです。

LEDは[SK6812MINI-E](https://shop.yushakobo.jp/collections/all-products/products/sk6812mini-e-10)を用います。  
<img src = "https://cdn.shopify.com/s/files/1/0532/0880/9633/products/YS-SK6812MINI-E_16829ac6-2d6d-4f3c-951f-1646c9d32912_700x.jpg" width = "600px" />
(画像は遊舎工房さんのものを拝借)

LEDは信号が流れる順番があり、取り付け順はこの番号が低いものからハンダ付けをし、都度PCなどに繋いで点灯を確認すると良いです。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4564_led.jpg?raw=true" width = "600px" />

LEDは基板の裏側に取り付けます。  
LEDのライトが表側を向くようにしつつ、LEDの向きを確認します。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4688.jpg?raw=true" width = "600px" />

LEDのハンダ付け箇所にハンダを溶かして載せます。  
「予備ハンダ」と言われる作業方法です。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4689.jpg?raw=true" width = "600px" />

LEDをピンセットで持ちながら、予備ハンダを溶かして足の一部をハンダ付けします。  
LEDは熱に弱く、壊れやすいので本体を熱するのはなるべく避けましょう。
利き腕側の足からハンダ付けすると楽かと思います。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4690.jpg?raw=true" width = "600px" />

残りの足もハンダ付けします。  
ハンダ付けする足が利き腕側に来るように基板を回転させると、失敗しづらくなります。
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4691.jpg?raw=true" width = "600px" />

LEDの取り付けに慣れていない方は、一つのLEDを取り付ける毎にPCに接続して点灯するかを確認します。
テスト用のファームウェアはいずれかのキーを押すとLEDのON/OFFを切り替えますので、点灯しなかった場合はキーを押してみてください。
それでも点灯しない場合は、LEDが熱で壊れてしまったか、ハンダ付けが上手くいっていない可能性があります。
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4692.jpg?raw=true" width = "600px" />

全部で6個のLEDを取り付けて全て点灯したら完了です。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4693.jpg?raw=true" width = "600px" />

### 6. スイッチプレートの作成

もう1枚のPCBをスイッチプレートとして加工します。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4676.jpg?raw=true" width = "600px" />

スイッチ部分にある点線(青丸の箇所)をニッパーで切ります。    
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4677_2.jpg?raw=true" width = "600px" />

全部で13箇所をくり抜きます。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4679.jpg?raw=true" width = "600px" />

キースイッチを穴に差し込みます。入らない場合は、ニッパーで切り取り部分を削るなどします。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4681.jpg?raw=true" width = "600px" />

続いてPro Micro部分を切り取ります。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4682 .jpg?raw=true" width = "600px" />

ニッパーで穴の空いた部分を切り離してください。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4683.jpg?raw=true" width = "600px" />

スペーサーとネジで２つの基板を接続します。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4684 .jpg?raw=true" width = "600px" />

スイッチプレートにネジを差し込みます。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4685.jpg?raw=true" width = "600px" />

ネジにスペーサーを取り付けて固定します。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4686.jpg?raw=true" width = "600px" />

スペーサーをPro Microを取り付けた基板にネジで固定します。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4695.jpg?raw=true" width = "600px" />

以下のように組み上がればこの項目は完了です。  
スイッチプレートに入れたキースイッチは一度外したほうが作業がスムーズに進むかと思います。
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4696.jpg?raw=true" width = "600px" />


### 7. キースイッチの取り付け

BaumkuchenマクロパッドはCherry MX互換キースイッチを取り付けることができます。  
お好みのキースイッチを13個用意してください。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4595.jpg?raw=true" width = "600px" />

キースイッチをスイッチプレートに差し込み、基板の裏側から足が出ていることを確認します。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4697.jpg?raw=true" width = "600px" />

キースイッチの足をはんだ付けします。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4698.jpg?raw=true" width = "600px" />

慣れていない方は、キースイッチを取り付けるごとにキーが動作するかを確認すると、着実に作業を進められるかと思います。  
キースイッチの取付箇所は13箇所ありますが、Pro Microの手前にある箇所はロータリーエンコーダを取り付けることも可能です。 
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4600.jpg?raw=true" width = "600px" />

### 8. ロータリーエンコーダの取り付け

Pro Micro手前側の箇所はキースイッチかロータリーエンコーダを取り付けることができます。  
キースイッチを取り付けたい方はこの項目は省略しても問題ありません。  

ロータリーエンコーダは回転操作ができるパーツで、マウスのホイールスクロールに近い操作が可能です。  
ロータリーエンコーダ自体を押し込むことで、キーの押下と同様の入力ができるものもあります。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4601.jpg?raw=true" width = "600px" />

ロータリーエンコーダは基板の表側から足を差し込みます。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4700.jpg?raw=true" width = "600px" />

基板の裏側から、ロータリーエンコーダの足が出ていることを確認します。  
足が5本のものと7本のものが一般的です。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4702.jpg?raw=true" width = "600px" />

各ピンの説明は以下です。赤丸と青丸で囲ったピンを基板とハンダ付けします。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4603_2.jpg?raw=true" width = "600px" />

他のキースイッチ穴などと比較して、やや基板のハンダ付け箇所の穴が広めになっておりますので、正しくハンダ付けできているかを確認してください。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4604.jpg?raw=true" width = "600px" />

基板を表にして、ロータリーエンコーダを回しても正しく固定されているかを確認します。  
PCにUSBで繋いで動作するかを確認すると尚良いです。  
テスト用ファームウェアではロータリーエンコーダを回すと1キーと2キーが入力されます。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4605.jpg?raw=true" width = "600px" />

### 9. ゴム足シールを底面に貼り付け

ゴム足のシールを底面に貼り付けて打鍵時の衝撃で動かないようにします。  
<img src = "https://github.com/takashicompany/minidivide/blob/master/images/build/IMG_3748.jpg?raw=true" width = "600px" />

以下は貼付け例です。ご自身の打鍵スタイルに合わせて調整すると良いかと思います。ゴム足の高さが足りない場合はキースイッチ、ロータリーエンコーダ、リセットスイッチの足を短くしても良いかもしれません。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4717.jpg?raw=true" width = "600px" />

### 10. キーキャップを取り付ける

お好みのキーキャップを取り付けます。  
<img src = "https://github.com/takashicompany/baumkuchen/blob/master/images/build/IMG_4607.jpg?raw=true" width = "600px" />

### 11. キーマップをカスタマイズする

[こちら](https://remap-keys.app/catalog/hN0gqZgFJvkWriQdhvu9/firmware)からRemapからVIA用のファームウェアをPro Microに書き込むことで、Webブラウザからキーマップを変更することができます。  

<img width="600" alt="temp 2023-05-07 16 49 57" src="https://user-images.githubusercontent.com/4215759/236664932-613d52d2-141f-4364-b9a7-012cec4f8f70.png">

Remapの使い方は[こちらの記事](https://salicylic-acid3.hatenablog.com/entry/remap-manual)を参考にすると良いかと思います。  

### 完成したら

完成しましたら、ぜひSNSなどに写真を投稿頂ければと思います。
Twitterのハッシュタグは [`#BaumkuchenMacroPad #自作キーボード`](https://twitter.com/search?q=%23%E8%87%AA%E4%BD%9C%E3%82%AD%E3%83%BC%E3%83%9C%E3%83%BC%E3%83%89%20%23BaumkuchenMacroPad&src=typed_query) を付けていただけると幸いです。
キットを組み立てた感想や、キーボードを使った所感などをお待ちしております！次回作の励みとさせて頂きたいと思います。

また、毎週日曜日の１9時より実施されている[#KEEP_PD](https://twitter.com/hashtag/KEEB_PD?f=live)に投稿頂くこともオススメです。  
開催の告知は[@KEEB_PD](https://twitter.com/KEEB_PD)にて行われております。

ご不明な点などございましたら、[@takashicompany](https://twitter.com/takashicompany)にメンションやDM頂ければ回答できるかと思います。


<!---

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

--->
