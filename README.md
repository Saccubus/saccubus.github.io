# さきゅばす公式サイト

[![Build Status](https://travis-ci.org/Saccubus/saccubus.github.io.svg?branch=master)](https://travis-ci.org/Saccubus/saccubus.github.io)

[さきゅばす公式サイト](saccubus.osdn.jp)のソースです。[Jekyll](https://jekyllrb.com/)で構築しています。

# Pre requirements

 - [Jekyll](https://jekyllrb.com/docs/installation/)

 ```
 $ gem install jekyll
 ```

# 更新の仕方

リポジトリにpushするとtravis-ciが走って自動で[ウェブサイト](saccubus.osdn.jp)が更新されます。

# ローカルで動かす

push前にプレビューしたいときは次のコマンドを使うと[http://localhost:8080/](http://localhost:8080/)から見れます。ファイルが更新されると自動でサイトが生成され直すので、何度もコマンドを打ち直す必要はありません（その代わりに、ブラウザの更新ボタンを押してください）。

```
jekyll s
```

# ローカルでビルドする

ローカルでビルドするには、次のようにします。

```
jekyll b
scp -r _site server:/path-to-deploy
```
