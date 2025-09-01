# 23時56分に光る謎のデジタル時計(2356_clock)
|時計(公開URL)|サンプル|推奨ウィンドウサイズ|
|-|-|-|
|[数字のみ](https://dj-kata.github.io/obs_misc/2356_clock/index.html)|<img height="70" alt="image" src="https://github.com/user-attachments/assets/fc996677-5671-410f-8f05-661fd3dfa629" />|1390x130|
|[バナー型](https://dj-kata.github.io/obs_misc/2356_clock/cyber_banner_clock.html)|<img height="131" alt="image" src="https://github.com/user-attachments/assets/54153964-113a-4cdf-adf3-beda7d14713e" />|380x220|
|[横長型(少しスリムなレイアウト)](https://dj-kata.github.io/obs_misc/2356_clock/cyber_slim.html)|<img width="236" height="80" alt="image" src="https://github.com/user-attachments/assets/1b4d9adc-205b-41c3-ab59-262256aec81a" />|380x120|
|[横長、ピンク基調](https://dj-kata.github.io/obs_misc/2356_clock/pink.html)|<img height="80" alt="image" src="https://github.com/user-attachments/assets/f377d5c4-3038-4a3a-a095-125edde8914f" />|480x120|

# 使用方法
OBSに設定する場合は以下の通り。
1. ソースの追加(+マーク)→ブラウザを選択
2. URLに使いたいデザインの公開URL(上述)を設定してOKをクリック
3. 余白の調整をする場合、ソースの大きさを上記の推奨値にする
<img width="730" height="859" alt="image" src="https://github.com/user-attachments/assets/b1f8a4b4-e794-4b62-b7b7-20ceb2c393b8" />

# カスタマイズ
ブラウザソースのカスタムCSSでデザインを変更することができます。  
利用できるカスタムプロパティは以下。
```css
/* OBSがデフォルトで挿入する部分 */
body{
    background-color: rgba(0, 0, 0, 0.0); /* 4つ目(不透明度)を1.0に近づけると背景色が濃くなります */
    margin: 0px auto;
    overflow: hidden;
}
/* 本アプリの設定 */
:root{
    --enable-flash: 0;                            /* 1:指定時刻に光る機能を有効にする */
    --flash-hh: 23;                               /* 光る機能の指定時刻(XX)) */
    --flash-mm: 56;                               /* 光る機能の指定時刻(YY)) */
    --color-live: #ff0040;                      /* Liveの部分の色 */
    --color-frame: #0ff;                        /* フレームの色 */
    --color-time: #0ff;                         /* 時刻の色 */
    --color-date: #0f8;                         /* 日付の色 */
    --color-flash: #fa0;                        /* 光る演出の色 */
    --color-scanning-line: #0ff;                /* 走査線の色 */
    --color-shadow1: rgba(0, 255, 255, 0.3);    /* 枠につける影の色1 */
    --color-shadow2: rgba(0, 255, 255, 0.6);    /* 枠につける影の色2 */
    --enable-scanning-line: 1;                    /* 1:走査線を有効にする */
}
```
