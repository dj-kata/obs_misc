# 23時56分に光る謎のデジタル時計(2356_clock)説明書
- 公開URL  
https://dj-kata.github.io/obs_misc/2356_clock/index.html

## これは何？
OBS配信などに使えるデジタル時計風HTMLです。
<img width="883" height="178" alt="image" src="https://github.com/user-attachments/assets/fc996677-5671-410f-8f05-661fd3dfa629" />

23時56分やXX時23分56秒になると以下のように色が変わる演出があります。
<img width="1383" height="173" alt="image" src="https://github.com/user-attachments/assets/bd0c3709-1d40-4865-8db2-1b690bad9ef3" />

## 使い方
OBSに設定する場合は以下の通り。
1. ソースの追加(+マーク)→ブラウザを選択
2. URLに```https://dj-kata.github.io/obs_misc/2356_clock/index.html```を設定してOKをクリック
3. 余白の調整をする場合、ソースの大きさを幅1390、高さ130にする
<img width="730" height="859" alt="image" src="https://github.com/user-attachments/assets/b1f8a4b4-e794-4b62-b7b7-20ceb2c393b8" />

## カスタマイズ
ブラウザソースのカスタムCSSでデザインを変更することができます。  
利用できるカスタムプロパティは以下。
```css
body{
    background-color: rgba(0, 0, 0, 0.0); /* 4つ目(不透明度)を1.0に近づけると背景色が濃くなります */
    margin: 0px auto;
    overflow: hidden;
}
:root{
    --color-main: #aaf; /* 基本のフォント色 */
    --color-flash: #f72; /* 光っているときのフォント色 */
    --color-bg: #333; /* 背景部分のフォント色 */
    --shadow-main: 0px 0px 20px #0aafe6; /* 基本のフォントの影 */
    --shadow-flash: 0px 0px 20px #e6770a; /* 光っているときのフォントの影 */
}
```

例えば、背景を黒(透明度10%)、基本フォントを緑色系、光る演出を赤色系に変えたい場合は以下のカスタムCSSを設定すればできます。
```css
body { background-color: rgba(0, 0, 0, 0.9); margin: 0px auto; overflow: hidden; }
:root{
    --color-main: #aaf;
    --color-flash: #f00;
    --color-bg: #333;
    --shadow-main: 0px 0px 20px #0aafe6;
    --shadow-flash: 0px 0px 20px #ff7777;
}
```
<img width="832" height="958" alt="image" src="https://github.com/user-attachments/assets/920cf1b7-ae42-4330-abe7-b35e6da3c203" />

## その他
個人利用・商用問わず自由にお使いください。概要欄などにURLを記載してもらえると喜びます。
```
23時56分に光る謎のデジタル時計
https://github.com/dj-kata/obs_misc/tree/main/2356_clock
```

数字のフォントについては、DSEG14を利用させてもらっています。
https://www.keshikan.net/fonts.html
