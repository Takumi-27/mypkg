# mypkg   [![test](https://github.com/Takumi-27/mypkg/actions/workflows/test.yml/badge.svg)](https://github.com/Takumi-27/mypkg/actions/workflows/test.yml)
* このリポジトリはROS2のパッケージであり、talker・listener・talk_listen.launchという名前のノードが含まれている。

## talker
* 数字をカウントし、countupというトピックを通じてInt16型のメッセージを送信する。

## listener
* countupからInt16型のメッセージを受信し、標準出力する。

## 使用方法および実行結果
　 端末を2つ立ち上げ、talkerとlistenerをそれぞれ実行する。
```
端末1$ ros2 run mypkg talker
端末2$ ros2 run mypkg listener
[INFO] [1672465105.340123900] [listener]: Listen: 0
[INFO] [1672465105.829812200] [listener]: Listen: 1
[INFO] [1672465106.329438600] [listener]: Listen: 2
・・・
```

## talk_listen.launch
* launchファイルを使用することで、talkerとlistenerを一度に立ち上げることが出来る。

## 使用方法および実行結果
```
$ ros2 launch mypkg talk_listen.launch.py
[listener-2] [INFO] [1672465415.758183600] [listener]: Listen: 0
[listener-2] [INFO] [1672465416.247063200] [listener]: Listen: 1
[listener-2] [INFO] [1672465416.747884500] [listener]: Listen: 2
・・・
```

## 動作確認済み環境
* Ubuntu 20.04・22.04

## ソフトウェア
* ROS2 humble

## ライセンス
* このソフトウェアパッケージは、3条項BSDライセンスの下、再頒布および使用が許可されます。
* このパッケージのコードは、下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを、本人の許可を得て自身の著作としたものです。
      * [ryuichiueda/my_slides robosys_2022](https://github.com/ryuichiueda/my_slides/tree/master/robosys_2022)

## 謝辞
* 千葉工業大学 先進工学部 未来ロボティクス学科 上田隆一研究室の皆様には心より感謝申し上げます。

© 2022 Takumi Ochiai


