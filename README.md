# Setup_Mac
## 0.初期化
- 工場出荷状態に戻す：  
 「システム環境設定」メニューから「すべてのコンテンツと設定を消去」で工場出荷状態に戻せる。Mac を購入後はじめて設定するときと同様に、設定アシスタントで設定プロセスを実行できる。
- OSをaクリーンインストールする：  
「command (⌘) + R」キーを長押し、「OSを再インストール」を選択。

## 1. キーボード
Windows用のキーボードを使う場合、うまく認識されないことがあるので、設定する。  
サンワサプライ「SKB-ERG5BK」はエルゴノミックで左右分割されているうえにトラックボール付きで非常に気に入って使っているが、仕様上は「日本語109A配列」ではあるがテンキーレスでキーの配置が若干変則的なため、正しく設定するにはちょっとコツがいる。  
「キーボードの種類を変更」で立ち上がる「キーボード設定アシスタント」では、「左Shiftキーの右隣のキーを押して」で「z つ」キー、「右Shiftキーの左隣のキーを押して」で「＼ ろ」キーを押すことで、「JIS（日本語）」と判定される。しかし「SKB-ERG5BK」では、この「＼ろ」キーが左Shiftキーと「z つ」キーの間に割り込んでいるので、みたまま正直に「＼ ろ」キー、「／ め」キー、と押してしまうと、正しく判定されず、認識に失敗する。  
できることなら、アシスタントをすっ飛ばして直接「キーボードの種類を選択」を立ち上げて「JIS（日本語）」と設定したいところだが、その方法はなさそう。  
面倒くさいが、「キーボード設定アシスタント」で「z つ」、「＼ ろ」と押すしかない。
なお、日本語入力の切り替えは「Ctrl + Alt + Space」である。  
Mac のキーボード配列でいうところの「Ctrl + Option + Space」である。
ウィンドウのキャプチャは「Shift + Win + 4」に続いて「Space」、さらに対象のウィンドウをクリック、の３アクションである。  
Mac のキーボード配列でいうところの「Shift + Comand + 4」である。

## 2.ソフトウェアアップデート
「システム設定 -> 一般 -> ソフトウェアアップデート」で最新の状態にする。  
## 3.Chrome
## 4.Garageband
初回起動時に、「基本サウンドのダウンロード」で2.16GBほどのデータがダウンロードされる。
続けて、メニューの「Garageband -> サウンドライブラリ -> 利用できるすべてのサウンドをダウンロード」とする。  
約15GB のデータがダウンロードされる。  
## 5.Visual Studio Code
zipファイルをダウンロードして、展開し、「アプリケーション」フォルダに移す。  
「ターミナル」を立ち上げて、「git」と入力してReturn。  
git がインストールされていない場合、「今すぐインストールしますか？」と訊いてきてくれるので、「インストール」とする。  

```sh
hogehoge@MBA ~ % git
hogehoge@MBA ~ % git config --global user.name "hogehoge"
hogehoge@MBA ~ % git config --global user.email hogehoge@example.com  
hogehoge@MBA ~ % git config --global credential.helper store  
```  
## 6.OBS Studio
ダウンロードしてインストール。  
1. 「画面収録」の権限をOBSに許可。
2. 「カメラ」へのアクセスを許可。
3. 「マイク」へのアクセスを許可。
4. 「アクセシビリティ」の権限を許可して、フォーカスがOBS以外にあっても、ホットキーを動作させる
なお、これらの権限設定画面は、いずれも「プライバシーとセキュリティ」の中にある。  
## 7.iPod touch (Gen7)をWebカメラにする
ケーブルでつなぐと、iPod touch の画面をキャプチャできる。  
カメラを立ち上げると、Webカメラ的に使える。  
iOS16 以降であれば、「連携カメラ」という機能があるが、iPod touch はiOS15止まりである。