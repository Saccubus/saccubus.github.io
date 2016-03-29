# さきゅばす公式サイト

[![Build Status](https://travis-ci.org/Saccubus/saccubus.github.io.svg?branch=master)](https://travis-ci.org/Saccubus/saccubus.github.io)

さきゅばす公式サイトのソースです。[Jekyll](https://jekyllrb.com/)で構築しています。

# Pre requirements

 - [Jekyll](https://jekyllrb.com/docs/installation/)

 ```
 $ gem install jekyll
 ```

# How to build

```
jekyll b
scp -r _site server:/path-to-deploy
```

# ローカルで動かす

```
jekyll s
```
