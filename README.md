# ロボットシステム学 − 課題2
18C1135　鷲尾弘希
## 概要
パブリッシャを1個持つノードcount.pyで変数を定義して＋１しながら表示する。
サブスクライバを1個持つノードtwice.pyでパブリッシャからデータを受け取り、2倍にする。
実行データを二つ並べながら見ることができる。
## 動画
- URL − ~~
## 使用するもの
- Raspberry Pi 4 Model B
  - Ubuntu 20.04 LTS
## 使い方
1. `catkin_ws/src/mypkg`下でリポジトリをクローンしてローカルリポジトリの作成

   ```
   $ git clone https://github.com/nyannkoww/robosys2020_2.git
   ```
2. 以下を入力
   ```
   $ roscore 
   ```
3. 別ターミナルに以下を入力

   ```
   $ rosrun mypkg count.py
   ```
4. 別ターミナルに以下を入力
   ```
   $ rosrun mypkg twice.py
   ```
5. 別ターミナルに以下を入力
   ```
   $ rostopic echo /twice
   ```
6. 別ターミナルに以下を入力
   ```
   $ rostopic echo /count_up
   ```
