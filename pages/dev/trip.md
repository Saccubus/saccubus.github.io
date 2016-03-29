---
title: さきゅばすの歩き方
tags: [develop]
sidebar: home_sidebar
permalink: /dev/trip/
summary: さきゅばすのソースコードについて説明します。
---

さきゅばすは2.0以降、とても複雑な構造になってしまいました。

このページでは、さきゅばすのモジュール構造などを書きます。

# 全体のアーキテクチャ

さきゅばすは、次の図のように中心となるffmpegと周囲のモジュールで構成されています。

<img src="/images/overview.png" width="400">

# SaccubusFront

　このモジュールは、GUIとダウンローダの２つのモジュールに大きく別れています。

　GUIは設定の管理やユーザの変換指示受付け、FFmpegのプロセス起動、一度に実行する変換プロセス数の管理などを行います。
