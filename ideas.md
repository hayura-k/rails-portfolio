- ### youtubeストッカー
繰り返し見たいYoutubeの動画を保存してタグごとに分けて、見たい動画をすぐ取り出すことができるアプリ。

エレベーターピッチ  
```Youtubeストッカー```というサービスは  
```お気に入りのyoutubeの動画を何度もみたいがyoutubeの後で見る機能は追加した順番でしか表示できないという問題```を解決したい  
```お気に入りの動画を何度も見たい```人向けの 
```動画ストックツール```です。  
```繰り返しみたい動画を保存し、それをタグ付けすることで、見たい動画を素早く見る```ことができ、
```普通のストックできるアプリ```とは違って
```知り合い（フォロワー）とかのお気に入りの動画も見ることができる。```  

**つけたい機能**  
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

**できたらつけたい**  
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

[ページ遷移](https://www.figma.com/file/qecis7JP2nyRtF9e8i9GoD/youtube%E3%82%B9%E3%83%88%E3%83%83%E3%82%AB%E3%83%BC?node-id=2%3A5)  
[テーブル設計](https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=%E3%83%9D%E3%83%BC%E3%83%88%E3%83%95%E3%82%A9%E3%83%AA%E3%82%AA.drawio#R7Z1hc6I4GMc%2FjS9vR0BQX1rb7d5cd67T7u1tX3WyEjGzSLwQW91PfwkkiEQtDAIRmensmAABnv%2FDj%2BTJE7ZnTZebewJWi6%2FYhX7P7LubnnXbM01jOGT%2F8optXDEwRYVHkCv22VU8o99QVPZF7Rq5MNzbkWLsU7Tar5zhIIAzulcHCMHvYjfR3Bz7%2B2ddAQ8qFc8z4Ku1%2FyKXLuLakbwLXv8FIm8hz2w443jLEsidxanDBXDxe6rKuutZU4IxjX8tN1Poc9tJu8THfT6yNbkwAgOa54AX1%2Fz7%2B%2FJ%2BbAX3t96L8QXR35M%2FRCtvwF%2BLG16HkITiiulWmoFd%2FIr%2FpOAnr7oJKSBUqGX1WQWzPwUogIRVGFHZ98EqRNHucc0C%2Be4D2OI1lQ3J0s0cbaD7FIvF92W6PbDGeJE3PmeNP4uL4ZuBj7yA%2FZ6xW%2BdnvCEwZNfyAEIq9lCNI%2B8UEgo3qSphrHuIl5CSLdtFbrWFcMJzLVF837lBUrdIuUAiOBCu5yVN79RhP4RABcQyFbGO6sTunCLgP7FHAgReJNm%2BItysLsGrb4B4kIqKFUbcoHdvzGqJ7ZHvT7GPubABDnhLFK%2FERh%2FO5bE%2FMaV4KfUT5kgajUxh37A%2FZpxp%2F5Pds9nlTlnZ2JXZH9%2Bd0CkOQkqYO%2FE2IFP1HXJlD6h60qk%2FlrqgtFZVylqKso9%2FFdM2oh%2FYaVtYtn5Gtuwzh5k5534EsAVyXRjk18PMrUdKgFrtP1Dsz3Zv1v6ScfG%2BN%2BEKzFDgPcRHOhmB7LoE2hx%2FYPp1CmZfBAqzml4ACp2mUeiUVPbsDyJ0kWyvJAft3GI0xcGhYvwALNmvCfNBRp%2Fe1OxN2Ln7wZq3O5kDP4S6c7IWwXTh4qjjYjVcHDfNxXF7uTjKLUZTXJTRiJT14RIgzsBIAkQYHDNYlKxcB%2Bg%2FftCEknWbYZlfRV1gaajRj46WZ6GlYTaNS6NssERjXhr59WgMmGpEY0a2Kwrd1xUIw3dM3F2vsr1MLKCUNlAcdAw8DwPtxhlotwd5g9zmbwx5auQiBD69CszlV0cXzCWzch3mSmJu1DTm5NReCzAnvVJjzMl%2BdApz4A1QQORYOGbdtYQICyimC%2FqGOSZPoOtBObnEDIDo9gn6gCIc3O22xFNQcRIAG29ZNwu69MVDAAN3wtMvWPHuiYn2DX8FwTbawO7hh3xyeOGFFz7Zsni7SW%2B83YqSqodMB5EUPiqRiGrze8r7SBmHFEkqSWSLN7h3HYd0Eud45BhPeYBEpkToOCN1iNdkBsVRO7WVhgaZhrLtxKZR2om8JrnvEo6kThfU6UgbRH%2FIndjvlBux0s6LeOFDJ4otfuJe5dP4obfZlmbeNhzsO0kyxVfU24b98V5DdjbRpWp3yzG5cUHc%2BtjlhpfqclbG5RLgFQZc1nezDVXscqMcEWL9XC4h46e%2BYe3RcWhZJ%2FnIC4%2BQIGa3KJOvnAOPcvqv4%2Bjmv%2BOM22VJl9d%2FkwuSDWU7dRX7r6XGJCjwuvROvtXZl2YwEt3itJONTjnZ%2BbMAc%2FSnNAhSNJ%2Fgmbh1mQzPg%2BJWl%2BGpdl7alOKZuK6%2BgQtLzaC4qiTPAhIdj1Qkkxr1pOWqaRc6ArH5qG1xIB7I86wXiIOyyRcah3ETv9WXhgM1jLuf6qk5GOtRRxsQqu%2BuN%2BRC%2FBpSPPv1yvr0r0QMOru%2BPevLZ5ZuDWy1b28eEtCobsHCZbzKmu%2FbJ65eavVWrU%2Bnrb7K2tS3t%2FV%2Fm9nq2%2Byq%2BvYFJDoxC2nWKpmaIagjEJvv2xcH4qE1XPUCUV1P%2BblpIJ5xGZeVW5DGeKhO8fM%2BIj9mwh8Kj3W95PqEOSbskoLXX3Abp3C0fJ1CAfm0YWXZRZEdK4%2Bx8tC6rnpZqQb928TK%2FIGpxlipRuZTY%2BsOmEU01AWYjjoeAGu64NPzsyhK0k2Bsi22tP%2BJfqNxQLbqoiTOZQwKmo%2BSJA5eKkpySNzqtFUHBW2Kkjj6jwocdVTwT7Q4%2Bc9b3V9fZ4yVFBDqRPi%2F1rkyp%2Bv%2FV4XFvO%2B86rRtdf%2Ff0b%2F%2F76j9f%2F4NxMPBkitZ1VJANm0YWfYDKR0ji8RIamXksOzkqc6EzB%2ByauyrYOr85opgHiQh6qfB1qypa6Nlfgl1oaWpDrRTQa8uOtJLLW%2FK5u5%2FmCCeXWB1PtXUIbSO77jmwyNm%2FjGeLgnipjo4b1N4xNT%2FAx6mOsq%2BqiSSAhLpkhdpXsaKmeY7%2FcWB2HiCuKmOy1sUGDH1XzBjqiNqGRjRHIr16KILBK2yo%2BMOggUiHzUvG2zxKpnEb%2FVFoGUq5mejVFbRtApVIrCALtog8DLyBi4RgYc%2B5VszA8tGPXRmoP5ZA5YamIgZaLWZgWdJEjgTA1lx99%2FExZ8G2f1fe9bd%2Fw%3D%3D)


悩み  
・ タグの名前はユーザーが自分で決めれるようにしたい（今のままではできない気がする）  
・ 機能が少ない気がするが、フォロー機能とかをつけ始めるとSNSっぽくなってしまう（SNSっぽくするとどうしてもユーザーがいないと利用できないので、ツールとして作りたい）  
・ テーブルの数も少なかったりして全体的に大したことないアプリになりそう  
