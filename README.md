# NonMouse
There is no moue, but there is. 

Webカメラで自分の手元を写すことで、あたかも実態のないマウスが出来上がっているかのように見えるプログラムです。  

## Installation
### 1. Install Mediapipe　　
以下の公式ドキュメントに従って、Mediapipeのインストール
https://google.github.io/mediapipe/getting_started/install.html#installing-on-macos

### 2. Install pynput
```sh:Install
% pip install pynput  
```

## Usage
### run
NonMouseフォルダーをダウンロード、解凍する。
```sh
% cd ~/.../NonMouse
% python3 app.py
```
### argument
`python app.py --device 1`などというふうに引数を取れる。 
> * --device  
カメラデバイス番号の指定  
デフォルト：0  
>* --width  
カメラキャプチャ時の横幅  
デフォルト：960  
>* --height  
カメラキャプチャ時の縦幅  
デフォルト：540  
>* --min_detection_confidence  
検出信頼値の閾値  
デフォルト：0.7  
>* --min_tracking_confidence  
トラッキング信頼値の閾値  
デフォルト：0.5  
>* --use_brect  
外接矩形を描画するか否か  
デフォルト：指定なし  

### hands movement
* 人差し指の先端がマウスカーソルに対応。

* 人指し指の指先と中指の指先をつけると、マウスカーソルの動きが止まる。

* 親指の指先と人差し指の第２関節をくっつけると左クリック、離すと左クリックのリリース
