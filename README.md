SystemCommandプラグイン
=====================================

はじめに
--------

本プラグインは、Perlのsystem関数のラッパーです。

インストール
------------

本パッケージに含まれる「plugins」ディレクトリ内のディレクトリ「SystemCommand」を、MovableTypeインストールディレクトリの「plugins」ディレクトリの下にコピーしてください。作業後、MovableTypeのシステム・メニューのプラグイン管理画面を表示し、プラグインの一覧に「SystemCommand」が表示されていることを確認してください。これで設置完了です。

使い方
------

事前準備

1. mt-config.cgiに以下のパラメータを設定してください。

```
SystemCommand 1
```

タグ

例：
```
<mt:system command="/usr/bin/ls | sed 's/$/<br \/>/g'" >
```

モディファイヤ

**command**

system関数経由で利用したいコマンドを設定してください。


**return = "0 | 1"**

返り値を必要とする場合は1を設定してください。(デフォルト:1)


