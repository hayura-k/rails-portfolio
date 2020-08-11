- ### youtubeのsnsバージョン
エレベーターピッチ  
```Youtubeストッカー```というサービスは  
```お気に入りのyoutubeの動画を何度もみたいがyoutubeの後で見る機能は追加した順番でしか表示できないという問題```を解決したい  
```お気に入りの動画を何度も見たい```人向けの 
```動画ストックツール```です。  
```繰り返しみたい動画を保存し、それをタグ付けすることで、見たい動画を素早く見る```ことができ、
```普通のストックできるアプリ```とは違って
```知り合い（フォロワー）とかのお気に入りの動画も見ることができる。```  

- つけたい機能  
ログイン前  
・ ログイン機能(sorcery)  
・ twitter認証(OAuth)  
・ パスワード再設定  
・ ユーザー登録(名前、メールアドレス、パスワード、ユーザー画像)  
・ ゲストログイン  
ログイン後  
・ 取得動画一覧表示  
・ プロフィール編集（名前、ユーザー画像のみ）  
・ Youtube動画検索（API）  
・ 取得動画保存  
・ タグづけ機能  
・ 取得している動画の検索機能(フォームオブジェクトで設計)  
・ ページネーション  
・ Fontawesome  

できたらつけたい  
・ Rspecでテスト  
・ 他のユーザーを名前で検索する  
・ フォロー機能  
・ いいね機能  
. チャット機能  

インフラ  
・ heroku + S3 + MySQL  
バックエンド  
・ Rails  
フロント  
・slim + UiKit + jquery?  

使用するgem  
・ sorcery  
・ google-api-client 0.9.20  
・ slim-rails  
・ html2slim  
・ rubocop ・ rubocop-rails  
・ pry-rails ・ pry-byebug  
・ annotate  
・ carrierwave  
・ mini_magick  
・ font-awesome-sass  
・ faker  
・ kaminari  
・ yarn  
・ i18n  
後は必要に応じて随時入れる。

trubolinks使用しない・test・helper・css・jsの自動生成禁止

