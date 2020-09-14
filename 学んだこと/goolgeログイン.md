goolgeログインはなかったので、これを参考にした。

[SorceryでSlackでログインを実装する – t4traw\.net](https://t4traw.net/2019/05/15-120000/)

[deviseなしで Google OAuth 認証のサインインの実装 \- Qiita](https://qiita.com/daijiro_maeyama/items/8b672ec0721d43f2d044)

[【Rails】SorceryでTwitter認証 \- Qiita](https://qiita.com/aiandrox/items/5435c8b285c7dc0c455f)

### 本番環境での注意

本番環境では、リダイレクトURLがlocalhostに設定されているため、ローカルの設定のままだとログインできない。

#### 解決策

本番環境用のコールバックURLを設定すればいいだけだ。普通に設定した場合は、下記のようになる。  
config/initializers/sorcery.rb  
```rb
config.google.callback_url = if Rails.env == production
                              'https://www.youtube-stocker.com/oauth/callback?provider=google'
                             else 
                              'http://localhost:3000/oauth/callback?provider=google'
                             end
```

このように書いてもいいが、**config**と言うgemを使えば、わざわざif文で条件分岐させる必要がない。
configを使用した場合は、**config/settings/development.yml**と**config/settings/production.yml**に下記のように書く。  

development.yml
```yml
google:
  callback_url: http://localhost:3000/oauth/callback?provider=google
```

production.yml  
```yml
google:
  callback_url: https://自分のアプリ名/oauth/callback?provider=google
```

このように書くこととで、sorcery.rbには、下記の記述だけで済む。  
```rb
config.google.callback_url = Settings.google.callback_url
```

**参考記事**
[RailsでFacebookとGoogleのOAuth連携。SNS認証の方法 \- Qiita](https://qiita.com/nakanishi03/items/2dfe8b8431a044a01bc6)  
[【Rails】Sorcery で Twitter 認証 \[2\]｜Artefact｜note](https://note.com/artefactnote/n/ne0089a217489)


自分のアプリ名はお名前ドットコムなどのサービスでドメインを取得することができるので、それも利用して独自ドメインを取得する。  

[独自ドメインをherokuに設定しSSL化もおこなう \| 👑おすすめのプログラミングスクール比較！最短で上達するなら？](https://pg-happy.jp/domain-heroku-ssl.html)

記事の通りにやっていけばうまくいく。ドメインを取得した後、DNAサーバーの設定までちゃんと行わなければならない。





