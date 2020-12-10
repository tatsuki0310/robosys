# Name

LED_systemdriver


# Features

ロボットシステム学の講義で作成したデバイスドライバに変更を加えて以下のように動作するようにしました。

LEDを2個使用し、入力した数字によって光るLEDを変える。


# Demo

実演動画はこちらのURLからご覧下さい。https://youtu.be/2MLjiUqOI6c


# circuit

青色のLEDをGPIO24、赤色のLEDをGPIO25を+に接続し、-をGNDに接続します。


# Requirement

Raspberry Pi 4 Model B

os:Ubuntu 20.04.1 LTS

ブレットボード

LED(2個)

ジャンパー線 オス-メス(4本)


# Build

リポジトリをクローンし、そのディレクトリでmakeしてください。その後以下の順でコマンドを打ち込んでください。

```
$ sudo insmod myled.ko
```

```
$ sudo chmod 666 /dev/myled0
```

```
& echo 0 > /dev/myled0
```

echo 0 の0を0～3までの数字に変えて実行してください。


# Author

Tatsuki Saito

ベースとなったプログラムの開発者：Associate Professor : Ryuichi Ueda.

協力 Yusaku Sugiyama


# COPYING

GNU General Pubilc License v3.0


