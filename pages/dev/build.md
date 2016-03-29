---
title: How to build
tags: [develop]
sidebar: home_sidebar
permalink: /dev/build/
summary: さきゅばすのビルド方法を説明します。
---

まずは何はなくともビルドです。ビルドはLinuxの方がずっと楽です。（他の大半のソフトと同じように）Windowsでは結構大変なので覚悟してね。

# 必要なツール
 - g++
 - python3
 - pkg-config

## pkg-config
　ライブラリの管理をpkg-configに頼りきっています。WindowsとLinuxで同時にビルドできるようにするためにはこれが一番楽そうだったので…。必要なライブラリをインストールする **前** にインストールしてください。そうでないと、pkg-configで管理されないことがあります。

　pkg-configのビルドはかなり大変なので、次のgtkのサイトからバイナリをDLしてきてください。

 - [GTK+](http://www.gtk.org/download/index.php)

## 必要なライブラリ

以下のライブラリのビルドが必要です。

 - [google test](http://code.google.com/p/googletest/)
 - [ICU](http://site.icu-project.org/)
 - [しなもん](https://github.com/donut-lang/Cinamo)
 - [cairo](http://cairographics.org/)
 - [freetype2](http://www.freetype.org/freetype2/)
 - [fontconfig](http://www.freedesktop.org/wiki/Software/fontconfig/)
 - [SDL2](http://www.libsdl.org/hg.php)
 - [antlr3c](http://www.antlr3.org/download/C/)

# ビルド

## しなもん

共用ライブラリである、しなもんのビルドを行いましょう。

```bash
 git clone git://github.com/donut-lang/Cinamo.git
 sh bld.sh all
```

## ffmpeg
　このページで書くには奥が深すぎて書ききれないので丸投げします。

　[お気に入りの動画を携帯で見よう](http://blog.k-tai-douga.com/)というサイトに、Windows向けのビルド情報がたくさんのっているので、こちらを参考にして下さい。さきゅばす改造部分は内部の奥深くなので、ビルドする分にはふつうのFFmpegと差はありません。

## さきゅばす
　さきゅばすのビルドには、上記のねこまたに必要なライブラリに加え、次が必要です。

* [Python](http://www.python.org/)
* [libxml2](http://xmlsoft.org/)
* [cairo](http://cairographics.org/)
* [Freetype2](http://www.freetype.org/)
* [Fontconfig](http://www.freedesktop.org/wiki/Software/fontconfig)
* [SDL2](http://www.libsdl.org/)

　さらに、「ねこまた」をライブラリとして使います。こちらは発見に失敗する可能性が非常に高いです。失敗した場合は手動で設定お願いします。静的リンクである関係で、antlr3cのライブラリを再度設定しなければならないかもしれません。

　ビルドした後、ビルドしたライブラリに「Saccubus.dll」と「SaccubusCLI.exe」が出来上がれば成功です。

## さきゅばすフロント
　このモジュールはPythonで書かれているため、ビルドは必要ありません。

　実行するには、Python3が必要です。Windows向けには[Python公式サイト](http://www.python.org/)からインストーラーが入手できます。
