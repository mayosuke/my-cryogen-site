{:title  "herokuでネイキッドドメインを使う"
 :layout :post
 :tags   ["heroku"]}

mayosuke.jpは2015年6月から2016年1月までheroku上で動かしていた。

herokuはアプリにネイキッドドメインの割り当てを許可していないが、
ググると割り当てる方法が幾つか見つかった。
その中で、以下のブログに書いてある、
DozensというサービスとDNS割り当てのためのherokuアプリを組み合わせる方法を試すことにした。

[Herokuでネイキッドドメイン（ルートドメイン）を利用する方法 - LS1qJの日記](http://ls1qj.hatenablog.com/entry/2014/07/06/134108)

Dozensのアカウントを取得してherokuアプリをデプロイするところまではすんなりできたが、
デプロイしたアプリはエラーでちゃんと動いていなかった。
アプリをデバッグする手間が惜しかったので、
結局、同じDozensを利用した以下のサイトの方法を採用した。

[Herokuアプリのルートドメイン設定（Dozens + VALUE DOMAIN） | memobits](http://m.designbits.jp/14121021/)


## 他に参考にした情報

* [Custom Domains | Heroku Dev Center](https://devcenter.heroku.com/articles/custom-domains)
* [The Limitations of DNS A-Records | Heroku Dev Center](https://devcenter.heroku.com/articles/apex-domains)
* [DNSを自由に簡単に。Dozens（ダズンズ）](https://dozens.jp/)
* [CloudFlare使ってHerokuでルートドメイン使おう - PILOG](http://xoyip.hatenablog.com/entry/2014/05/03/192920)
* [お名前.comを使ってHerokuのルートドメインを設定する - Qiita](http://qiita.com/numa08/items/d4ad9454f0baefc8c784)
* [Herokuでルートドメインを使用する - Qiita](http://qiita.com/Oakbow/items/8f76ca074f51fc3bd89c)
* [Express - herokuにルートドメインを無料で設定する - Qiita](http://qiita.com/Tkashiro/items/8249455477bbb5333118)
* [GWS - Gehirn Web Services　ゲヒルンウェブサービス](http://www.gehirn.jp/)
