# nginx-proxy

ラズパイで動作せているロボットエンジンを localhost 接続させるための nginx プロキシー。

ロボットエンジンをラズパイで稼働させておき、ホストのPCからプロキシーを起動して下記のURLで接続する。

http://localhost:3090/browser-speech
http://localhost:3090/scenario-editor

chrome の音声認識は https か localhost でしか稼働しないため、ラズパイで動作しているサーバーに直接接続しても音声認識できない。
プロキシーを使って localhost 接続することで音声認識可能になる。
