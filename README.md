# 30m-timer
30分タイマーの bash スクリプトです。

## What?
* 30分後に PC をサスペンドして終了します。
* 開始時と終了の1分前に音声が鳴ります。
* バックグラウンドで実行後にターミナルは終了します。

## Why?
* 甥っ子に PC を貸すときに、時間制限をして強制的に終了させる機能が欲しかったためです。
* そのため、ターミナルを閉じたら終了してしまわないように、バックグラウンドで実行させることにしました。

## How?
音声再生用に mpv が必要です。  
timer ディレクトリに音声ファイルがあります。  
timer ディレクトリは、 $HOME ディレクトリに置くことにしています。

* sudo apt install mpv
* cp -r timer/ $HOME
* chmod +x 30m-timer
* sudo cp 30m-timer /usr/local/bin
* 30m-timer

## 参考
* 音: [効果音ラボ](https://soundeffect-lab.info/)
