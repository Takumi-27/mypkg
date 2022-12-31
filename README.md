# mypkg

## インストール方法

## talker
* 数字をカウントし、countupというトピックを通じてInt16型のメッセージを送信する。

## listener
* countupからInt16型のメッセージを受信し、標準出力する。

## 使用方法および実行結果
　 端末を2つ立ち上げ、talkerとlistenerをそれぞれ実行する。
```
端末1$ ros2 run mypkg talker
端末2$ ros2 run mypkg listener

```

## launch
* launchファイルを使用することで、複数のノードを一度に立ち上げることが出来る。
## 使用環境
* Ubuntu 22.04

## ソフトウェア
* ROS2 humble

## ライセンス
* このソフトウェアパッケージは、3条項BSDライセンスの下、再頒布および使用が許可されます。
* このパッケージのコードは、下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを、本人の許可を得て自身の著作としたものです。
      * [ryuichiueda/my_slides robosys_2022](https://github.com/ryuichiueda/my_slides/tree/master/robosys_2022)

## 謝辞
* 千葉工業大学 先進工学部 未来ロボティクス学科 上田隆一研究室の皆様には心より感謝申し上げます。

© 2022 Takumi Ochiai


