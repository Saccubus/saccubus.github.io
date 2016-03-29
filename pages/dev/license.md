---
title: License
tags: [develop]
sidebar: home_sidebar
permalink: /dev/license/
summary: このページでは、さきゅばすのライセンスと、使用しているライブラリのライセンス表示を行います。
---

さきゅばすのffmpeg以外のライセンスは、[GPLv3、もしくはそれ以降のバージョン](http://www.gnu.org/licenses/gpl.html)と、[二条項BSDライセンス](http://opensource.org/licenses/BSD-2-Clause)のデュアルライセンスです。[GPLの公式FAQ](http://www.gnu.org/licenses/gpl-faq.html)があなたの疑問に答えてくれるかもしれません。あなたがこのソフトウェアを改変する場合、どちらか一方、もしくは両方を選択することができます。

ただし、ffmpegを改変した部分に関しては、オリジナルのffmpegがGPLですので、GPL v3(or later)です。

# License
 Saccubus is dual licensed under GPL v3 (or any later) or 2-clause BSD license. You can chose one (or both) of them.

## GPL v3
```
 Saccubus
 Copyright (C) 2007- PSI, 2011- orz

 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.

 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.

 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

## 2-clause BSD License

```
 Saccubus
 Copyright (c) 2007- PSI, 2009- orz
 All rights reserved.

 Redistribution and use in source and binary forms,
 with or without modification, are permitted provided that
 the following conditions are met:

 Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer.

 Redistributions in binary form must reproduce the above copyright notice,
 this list of conditions and the following disclaimer in the documentation
 and/or other materials provided with the distribution.

 THIS SOFTWARE IS PROVIDED BY THE AUTHOR "AS IS" AND ANY EXPRESS OR
 IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
 FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE AUTHOR
 BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF
 THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

# 用いているライブラリのライセンス

## FFmpeg
動画変換に用いている[FFmpeg](http://ffmpeg.org/)の本体は、LGPLv2.1でライセンスされますが、本プロジェクトでは他に多数のライブラリを組み込んでいて、配布バイナリのライセンスはGPLv3となっています。詳しくは[FFmpegのLegalページ](http://ffmpeg.org/legal.html)を御覧ください。

## Python
Pythonを組込スクリプトとして利用しています。ライセンスに関しては、[Pythonの該当サイト](http://www.python.org/psf/license/)をご覧ください

## libxml2
[lixml2](http://www.xmlsoft.org/)をコメントの読み込みに使用しています。ライセンスは[MITライセンス](http://opensource.org/licenses/mit-license.html)です。詳しくはlixml2のサイトをご確認下さい。

## cairo
グラフィックエンジンとして[cairo](http://www.cairographics.org/)を用いています。ライセンスはGNU Lesser General Public License (LGPL) version 2.1 or the Mozilla Public License (MPL) version 1.1の二種類ですが、本プロジェクトではLGPLの方を採用しています。

## freetype2
フォントのレンダリングに[freetype2](http://www.freetype.org/index2.html)を用いています。[ライセンスはBSDライクなFreeTypeライセンスとLGPL2ライセンスのデュアルライセンス](http://www.freetype.org/license.html)ですが、本プロジェクトではFreeTypeライセンスの方を採用しています。

## fontconfig
ネイティブのフォントを利用するため、[fontconfig](http://www.freedesktop.org/wiki/Software/fontconfig)を利用しています。ライセンスに関しては[fontconfig](http://cgit.freedesktop.org/fontconfig/tree/COPYING)のサイトをご覧下さい。

## SDL2
画像の表示に[SDL2](http://www.libsdl.org/)を利用しています。[ライセンスはMITライセンス](http://www.libsdl.org/license.php)です。

## ANTLR3 C Runtime Library
ねこまたでニワン語をパースするために、[http://www.antlr.org/api/C/index.html ANTLR3 C Runtime Library]を用いています。BSDライセンスです。

```
 // [The "BSD licence"]
 // Copyright (c) 2005-2009 Jim Idle, Temporal Wave LLC
 // http://www.temporal-wave.com
 // http://www.linkedin.com/in/jimidle
 //
 // All rights reserved.
 //
 // Redistribution and use in source and binary forms, with or without
 // modification, are permitted provided that the following conditions
 // are met:
 // 1. Redistributions of source code must retain the above copyright
 //    notice, this list of conditions and the following disclaimer.
 // 2. Redistributions in binary form must reproduce the above copyright
 //    notice, this list of conditions and the following disclaimer in the
 //    documentation and/or other materials provided with the distribution.
 // 3. The name of the author may not be used to endorse or promote products
 //    derived from this software without specific prior written permission.
 //
 // THIS SOFTWARE IS PROVIDED BY THE AUTHOR ``AS IS'' AND ANY EXPRESS OR
 // IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES
 // OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
 // IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY DIRECT, INDIRECT,
 // INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT
 // NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 // DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 // THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 // (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF
 // THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

## ICU
Unicodeを扱うために、[ICU](http://site.icu-project.org/)を利用しています。ライセンスは[MIT派生](http://source.icu-project.org/repos/icu/icu/trunk/license.html)です。
