## ロボットシステム学　課題2

第10回で作成したROSのパッケージをベースに、オリジナリティーある改造をし、GitHubに置く
---

## オリジナリティーある改造
ROSのtopic通信を利用し、publishからデータを送信(インターネットの回線と想定)、subscriberで想定したデータ量になるまで受信する(特定のアプリダウンロードをする想定)というプログラムを作成しました。

改良したプログラムのURL
 * publish
https://github.com/kanekoNK/mypkg/blob/main/scripts/pub.py
 * subscriber
https://github.com/kanekoNK/mypkg/blob/main/scripts/sub.py
 * データを可視化させるための文字列を入力したCSVファイル
https://github.com/kanekoNK/mypkg/blob/main/scripts/log.csv
---

## 実際に動かす手順
 * 自身のcatkin_ws内のsrcに移動
 * git cloan https://github.com/kanekoNK/mypkg.git
 * cd  ~/catkin_ws/src/mypkg
 * 端末１　roscore　
 * 端末２　rosrun mypkg pub.py
 * 端末３　rosrun mypkg sub.py
 
---
## 実際に動かした動画
https://youtu.be/hMVFuafjlzk
