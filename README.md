# Heavy Left

95キーの分割型の日本語配列のキーボードです。  
左手側にテンキーが備え付けられており、数字の入力だけでなく専用のマクロパッドとしても使用が可能です。  
MXソケットによるキースイッチの付替えや、LEDによるアンダーグロウにも対応しています。  

![image](https://github.com/takashicompany/heavy_left/blob/master/images/qmk.jpg?raw=true)

## Store
[Booth](https://takashicompany.booth.pm/items/3403718)

## ビルドログ
組み立ての際は以下の記事もご覧頂けるとスムーズに作業が進めるかと思います。
- [いとうひよこさんのビルドログ](https://note.com/tsubuan_145/n/n2819f89d4f97)

## 必要な部品

### キットに同梱されているもの
|部品|個数|備考|
|:--|:--|:--|
|PCB|2|リードタイプと表面実装のダイオードに対応。|
|トッププレート|２||
|ボトムプレート|2||
|ダイオード（リードタイプ)|95||
|m2スペーサー(7mm)|12||
|m2ネジ(5mm)|24||
|リセットスイッチ|2||
|TRRSソケット|2||
|滑り止めシール|12||

### 別途用意するもの
|部品|個数|備考|
|:--|:--|:--|
|キースイッチ|95|Cherry MX互換のもの。|
|キーキャップ|95|Chery MX互換のもの。|
|Pro Micro|2||
|USBケーブル|1|Pro MicroとPCを接続します。|
|TRRSケーブル|2||

### オプション
|部品|個数|備考|
|:--|:--|:--|
|コンスルー|4||
|MXソケット|95||
|2uスタビライザー|4||
|LED(WS2812B)|12|アンダーグロウライトとしてキーボードの底面を光らせることができます。|


## 組み立て方

### 1. PCBの表裏を確認する

表  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8100.jpg?raw=true" width="600px">

裏  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8103.jpg?raw=true" width="600px">

### 2. ダイオードのはんだ付け

ダイオードの向きを確認してPCBに刺します。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8114.jpg?raw=true" width="600px">

表面に足が出るようにします。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8110.jpg?raw=true" width="600px">

はんだ付けを行い、ダイオードの足をニッパーで切ります。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8112.jpg?raw=true" width="600px">

---

表面実装のダイオードを使用する場合は、マスキングテープなどで表面にはんだが漏れないようにするとキレイに仕上がります。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8118.jpg?raw=true" width="600px">

表面実装のダイオードをはんだ付けする際は、はんだ付け箇所の片方にはんだを事前に乗せておきます。(予備ハンダ)  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8119.jpg?raw=true" width="600px">

ピンセットでダイオードを抑えながら、事前に乗せておいたはんだを溶かしてはんだ付けを行います。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8120.jpg?raw=true" width="600px">

もう片方もはんだ付けをして完了です。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8121.jpg?raw=true" width="600px">

左右の基板ともにはんだ付けを済ませます。

### 3. TRRSソケットのはんだ付け

TRRSソケットをPCBの裏面に乗せます。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8122.jpg?raw=true" width="600px">

マスキングテープなどで仮止めしておくと、裏返した時にスムーズに作業できます。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8123.jpg?raw=true" width="600px">

PCBの表面からはんだ付けを行います。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8124.jpg?raw=true" width="600px">

両手のPCBにTRRSソケットを付けたら完了です。

### 4.リセットスイッチのはんだ付け

リセットスイッチの取り付け位置を確認します。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8255.jpg?raw=true" width="600px">

リセットスイッチをPCBの裏面に刺します。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8135.jpg?raw=true" width="600px">

PCB表面からはんだ付けをします。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8136.jpg?raw=true" width="600px">

リセットスイッチの足をニッパーで可能な限り平らにしておくと後の作業がスムーズになります。
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8137.jpg?raw=true" width="600px">

私はこれぐらい頑張りました笑  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8138.jpg?raw=true" width="600px">

### 5. ピンヘッダの取り付け

**※Pro Microをコンスルー(スプリングピンヘッダ)で取り付ける場合はこの項目はスキップしてください。**

ピンヘッダでPro Microを取り付ける際は、**キースイッチとトッププレートをPCBに取り付ける前に**ピンヘンダをPCBにはんだ付けを行います。  
PCBの裏面にピンヘッダを取り付けます。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8247.jpg?raw=true" width="600px">

ピンヘッダをマスキングテープなどで仮止めしておくとスムーズに作業を進められます。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8248.jpg?raw=true" width="600px">

PCBの表面からはんだ付け行います。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8251.jpg?raw=true" width="600px">

### 6. MXソケットの取り付け(オプション)

はんだをPCB裏面のMXソケット配置場所の片方に乗せます。(予備はんだ)  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8141.jpg?raw=true" width="600px">

その後、ピンセットでMXソケットを抑えながら予備はんだを溶かしつつMXソケットをはんだ付けします。(写真でピンセットが映っていませんがお気になさらず笑)  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8142.jpg?raw=true" width="600px">

もう片方もはんだ付けをします。

### 7. トッププレートとキースイッチの取り付け

トッププレートに貼ってある保護シートを両面ともに剥がします。

左手のトッププレート  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8618.jpg?raw=true" width="600px">

右手のトッププレート  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8619.jpg?raw=true" width="600px">

トッププレートとPCBをキースイッチで留めます。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8260.jpg?raw=true" width="600px">

「5.ピンヘッダの取り付け」を行った場合で且つ「6. MXソケットの取り付け(オプション)」を**行わなかった場合**はPro  Microを取り付ける前にキースイッチを先に取り付けます。  
ここの手順を間違えるとリカバリーが大変です。(MXソケットを使っている or コンスルーでPro Microを固定する場合はやり直しができる)  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8261.jpg?raw=true" width="600px">

はんだ付けを行います。  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8262.jpg?raw=true" width="600px">

Pro Micro部分のキースイッチが固定できたらPro Microをはんだ付けします。  
(写真の工程がちょっと異なりますがお気になさらず)  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8131.jpg?raw=true" width="600px">

ある程度キースイッチを取り付けたら、スペーサーとネジでボトムプレートとトッププレートを留めます。  
ボトムプレートもトッププレート同様に保護シートを剥がします。

ボトムプレート左  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8620.jpg?raw=true" width="600px">

ボトムプレート右  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8621.jpg?raw=true" width="600px">

ボトムプレートを取り付けた図です。

左手  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8146.jpg?raw=true" width="600px">

右手  
<img src = "https://github.com/takashicompany/heavy_left/blob/master/images/build/IMG_8146.jpg?raw=true" width="600px">

キースイッチ・キーキャップをを全て取り付け、ゴム足シールを貼ったら完成です。
![image](https://github.com/takashicompany/heavy_left/blob/master/images/qmk.jpg?raw=true)

### 8. ファームウェア

QMKへのPull Requestは[こちら](https://github.com/qmk/qmk_firmware/pull/15052)

RemapのサイトからファームウェアのDLと書き込みが可能です。  
https://remap-keys.app/catalog/3ROWY1pMxcepNJD944Gs/firmware


## キーマップの変え方

### 1. USBを左側に挿す

優しく挿す。USBの口がもげちゃうことがあるので。  
![image](https://github.com/takashicompany/heavy_left/blob/master/images/02_600x450.jpg?raw=true)

### 2. 分割用のケーブルを挿す
![image](https://github.com/takashicompany/heavy_left/blob/master/images/03_600x450.jpg?raw=true)

### 3. **Google Chrome**で https://remap-keys.app/configure にアクセスする

### 4. +Keyboardをクリック  
![image](https://user-images.githubusercontent.com/4215759/138217454-b6baf0d0-8e31-4303-a0fa-29aec9c64035.png)

### 5. キーボードを選択する
![image](https://user-images.githubusercontent.com/4215759/138394611-de1c786c-508c-4ff7-9e44-5f4580286866.png)

### 6. Webアプリが起動する

![image](https://user-images.githubusercontent.com/4215759/138394760-13e8b76f-cf60-48e2-b0fb-bd0869cd68a9.png)

### 7. 好きなキーを入れる
ドラッグ & ドロップでキーを配置できる  
![image](https://user-images.githubusercontent.com/4215759/138394709-ae228e46-5031-49b2-9b6e-e0b6c6de99fe.png)

### 8. 画面右上のFlashを押すと反映される
![image](https://user-images.githubusercontent.com/4215759/138218286-5435b012-5f93-4494-862f-ca177083b234.png)

### 9. キー配置の詳細な使い方は[こちら](https://salicylic-acid3.hatenablog.com/entry/remap-manual)
