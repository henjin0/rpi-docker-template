# ライセンスについて
[LICENSE](./LICENSE) ファイルをご参照ください。

# はじめに
先にこのあたりを参考にdockerならびにdocker-composeをインストールしておく。
- [Raspberry pi に Docker ＆ docker-compose をインストールする方法](https://qiita.com/zono_0/items/30f2460acf2e8873024d)
- [Raspberry Piにdockerとdocker-composeを入れてみた](https://qiita.com/hoshi621/items/7906274326ef3013a73d)

もしRaspberry pi Camera(V2.1にて確認済み)を使用する場合には/etc/udev/rules.d/99-camera.rulesに下記を追加する。(アクセス権限を増やす。)

`SUBSYSTEM=="vchiq",MODE="0666"`

# dockerイメージ、コンテナ作成コマンド
`cd template`

`docker-compose up`

# dockerコンテナ実行コマンド
`docker-compose run rpi`

# dockerコンテナ一掃コマンド(参考)
`docker ps -qa | xargs docker rm`

# dockerイメージ一掃コマンド(参考)
`docker images -qa | xargs docker rmi`

