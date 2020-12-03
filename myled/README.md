# Name
LED_driver


# Features

ロボットシステム学の講義で作成したデバイスドライバに変更を加えて以下のように動作するようにしました。


・LEDを3個使用し入力された値に応じて、二進数の0~7までを点灯の切り替えにより表現します。


# Demo


デモムービーはこちらのURLからご覧ください。https://youtu.be/1kebJaBuN5U


# Requirement
Raspberry Pi 4 Model B


os:Ubuntu 20.04.1 LTS


ブレットボード


LED(3個)


100Ω抵抗(3個)


ジャンパー線 オス--メス(6本)


# Build

リポジトリをクローンし、そのディレクトリでmakeしてください。その後以下の順でコマンドを打ち込んでください。


$ sudo insmod myled.ko


$ sudo chmod 666 /dev/myled0


$ echo 0 > /dev/myled0


echo 0 の0を0～7までの数字に変えて実行してください。


# Author

Yuusaku Sugiyama

ベースとなったプログラムの開発者：Associate Professor : Ryuichi Ueda.


一緒に考えた人：Tatsuki Saito.


# License

GNU General Pubilc License v3.0
