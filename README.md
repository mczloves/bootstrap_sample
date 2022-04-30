# よりもいMAP
![README](https://user-images.githubusercontent.com/88571910/165759864-601b73f4-343d-42ec-a762-5271de5fd82a.png)


アニメ「宇宙よりも遠い場所」の「聖地巡礼」をサポートするアプリです。

- **宇宙よりも遠い場所とは？**<br>
 女子高生四人が宇宙よりも遠い場所『南極』を目指す青春アニメです。[公式サイト](http://yorimoi.com) 

- **聖地巡礼とは？**<br>
 アニメの舞台やモデルとなった場所をファンが訪れること。

## URL 
http://yorimoi-seichi-map.com <br>
トップページからゲストログイン可能です。

## 作成背景

「宇宙よりも遠い場所」の舞台となる、群馬県館林市は「行きたい聖地88選」に４年連続で選出。<br>
館林市は地域活性化として、アニメと公式で連携しているため訪れるファンが多い。

私も作品のファンなので実際に聖地巡礼した際に課題を見つけました。
### ~ 課題 ~
1. 聖地巡礼する際に、多くの人は有志の方が配布している紙の地図を持って回っている。<br>
そのため「道に迷う」「効率よく回れず時間がかかる」　※実際の地図を貼る
2. 配布マップではどんな聖地があるのか分かりづらい。
3. 感想の共有ができない。
4. 遠方に住んでいる方は現地に行きにくい。

**それなら自分が専用のアプリを作ろう…！！**<br>

### ~ 課題解決 ~
聖地巡礼をする方に喜んでいただくために、下記の方法で課題解決を目指しました。<br>
1. MAPを見ることで迷うことなく効率よく聖地巡礼できる。
2. 画像付きで聖地をリスト化することで、どんな聖地があるのかを分かりやすく見ることができる。
3. 感想投稿、写真投稿、いいね、コメントができることにより、感想を共有できる。
4. 遠方にお住まいの方もストリートビューで聖地を見ることができる。　

## こだわった点
アプリを開発するにあたって実際に聖地巡礼をしている方にお声がけして、6名の方に使用していただきフィードバックをもらいました。
フィードバックを書く
（例）
例えばアプリの特性上スマホで使用することがほとんどなので、よく使う喫煙本数の登録ボタンは右の親指で押しやすい位置に配置にすること、減煙のモチベーション維持のために節約額を表示することなど、一人で黙々と作成していたら気づかないユーザー目線のアドバイスを多く反映してきました。



## アプリ紹介

### アプリ全体　　
- スマホでの使用が主であるためレスポンシブデザインを意識した
- 非ログインでも利用可能にしています。(「感想投稿」「コメント」時のみログインページへ）
- fontawesomeのアイコンを使用しアプリの機能を分かりやすく表示した。

### ①トップページ
 - アプリの使用方法が直感的に分かることを意識して作成しました。
 - 「ログイン」「ゲストログイン」「新規登録」ボタン　※非ログイン時のみ表示されます
 - 各機能へのリンクボタン配置

![README_1](https://user-images.githubusercontent.com/88571910/165893097-78151d3c-83fb-45d6-bdf7-731e429acda5.gif)

### ②MAP表示ページ
- 聖地をピンで表示。クリックすると聖地の情報とGoogleMapへのリンクがあります。
- 訪れた聖地を投稿できるように、感想投稿へのリンクを設置しています。

![README_2](https://user-images.githubusercontent.com/88571910/165894108-9841cd7c-acef-4080-b942-8846686268a9.gif)

### ③聖地リストページ
- どのような聖地があるのかをリスト化しています。
- PCでは3カラム,タブレットでは2カラム,スマホでは1カラムで一覧表示します。

![README_3](https://user-images.githubusercontent.com/88571910/165899799-164ae25d-8efb-406e-bddc-16e17bb26aea.gif)

### ④聖地リスト詳細ページ
- アニメと聖地の比較画像、聖地の情報をみることができます。
- 遠方に住んでいる方向けにストリートビューを表示しています。
- リストからピンポイントで行きたい場所を選べるようにするため、GoogleMapへのリンクを設置しています。
- 聖地に対して写真付きでコメントができます。

![README_4](https://user-images.githubusercontent.com/88571910/165959501-26e5eb1c-11e7-45de-9ad7-e4d1aa3cf4fc.gif)

### ⑤感想一覧ページ
- 聖地巡礼をした方の感想をPCでは3カラム,タブレットでは2カラム,スマホでは1カラムで表示します。
- ユーザーが投稿した際、画像の登録がないとレイアウトが見づらくなってしまうため、画像の登録がない場合はデフォルト画像を表示させました。


### ⑥感想詳細ページ
- 感想に対して「いいね」「コメント」をすることができます。

![README_5](https://user-images.githubusercontent.com/88571910/166092042-0936f0d2-eb50-4aab-837b-e39370fe822c.gif)

## 使用技術
- 言語：Ruby : (2.7.3)
- フレームワーク : Ruby on Rails (6.1.4.1)
- フロントエンド : HTML/Scss/JavaScript
- DB : PostgreSQL
- インフラ : AWS（VPC・EC2・RDS・IAM・Route53）
- ソースコード管理 : GitHub
- 開発環境 : MacOS/VisualStudioCode


## 機能一覧
- MAP表示　（GoogleMapsJavaScript　API）
* 感想投稿機能
 * 画像投稿機能
 * いいね機能
 * コメント機能
* 聖地リスト表示
 * 聖地に対するコメント機能
 * 聖地に対する画像投稿機能
 * ストリートビュー機能
- ログイン・ログアウト機能（devise）
- ユーザー登録・編集機能（devise）
- 画像投稿機能（carrierwave/mini-magick）
- 日本語化（rails-i18n）
- エラー・フラッシュ表示機能
- レスポンシブデザイン（Bootstrap）
- 管理画面（ActiveAdmin）
- ページネーション（kaminari）
- フォーマッター（Rubocop）

## 追加予定機能


- 感想投稿のTwitterシェア
- テスト(Rspec)を記述

## ER図
https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1#R7V1bc%2BK4Ev41VO15GMp34DGQzGRrk3PmZGZnJk8pByvgGmOztnIhv37l%2B0WCSGBskDSVqsFCNKb7kz6p1d0e6LPV25fQXi9vAwd4A01x3gb65UDTVF0do%2F%2Filk3aYo21tGERuk7WqWz45r6DrFHJWp9dB0S1jjAIPOiu643zwPfBHNba7DAMXuvdngKv%2Fq1rewGwhm9z28Nbf7oOXKatY21Utl8Dd7HMv1m1Juk7KzvvnP2SaGk7wWulSb8a6LMwCGD6avU2A16svFwv6ec%2Bb3m3uLEQ%2BJDmA%2Ff%2Fe7nY%2FLoIxtGP%2B5%2FXq3%2BW9s%2FvnzIpL7b3nP3g5wiEUXbHcJOrAd38On4J7ce4aRpBO4SZtXQFNSD9Q9v1QYga1OTa8%2Bx15Cbd05al6zk39iZ4hrmg%2FGr65L4B5y41VtwX2e0GCYsvY%2BFPSPi37Gbit23PXfjo9Rz99PgbpyGI0L3c2BHMeuDKyX8pCCF4qzRlyvoCghWA4QZ1yd61cghmyFWt7Pq1xIE6ztqWVQyYWaOdYW9RyC7Ng15kFmKwloZZa7eh7mK8TZdB6L7H5vEydVaNl1y%2FuivP9hGQbafRNA2SgZsYwfW8WeAFsYX9wAeYkeNOThisv9vhAsCsYR24Pkz0YE7RH9LMTBmaAxPd6wxdq%2BU1%2Bou7h3AW%2BBEMEZhiGQDZ9BXEdp3CYJ0J9cBTLj%2FM9B6%2FfgwgDFZbEbBzAHwMiwwGOiUK9GOBQMdA8PWvrTBAvx%2B6tneHpkbbX3ip0ZKZ0i6NRrAsUdeFfpuKb47PAKnzyUsmu6XrOMCnt4dGbY%2BKAXRG%2FWfCSq0wS7M9NPH4NkQD5Nl3IsyoxX3ub2cDs7PrDP9AowIsQPifni2ez8Bp32m0tueuv7hJP2k1IGF2BYm37UPUbBUiVOI6wIgpCYGKEJQjEgLtsuBohGDRg6CbyQE4bi7vQDYwqY3BOxuMMCP79iq%2B1T%2FQ0EBT78kTQicoEI4AxpIAeieASd8EMOGXAMbUxuCdAHJvRMXKYGW7nhgUQI8D4ShAxX14kgO65gBV65sEVAbn4LmxgEpvD%2B5pAHf%2Fre0oeg1CRwwmYMCCeFSA%2BwzXQQTlcU46Q%2B95nlOcRbY%2FZ0v%2FXfsHOgY1Mk7lREfFPXg8Hemo0otXqAJ347mOiGc6DJgQj8WlU6%2F9DR0zK%2FR%2BrKPibr3PfbNCi1s66dkrzrdxz14chPXgJju6EDwBpMs5iE6eH7qBg3B8oEkH3wnwQe%2BnPLnVeXTwMWznuWcD3MEHXegJctTP7tcRiAdw757kgc55oP%2BTHo3Ba3h2REBvD%2B6JAPcKxl75WH%2BICpB2INdEQA8E4YjAYFgJSiI4GhGYfROBgS8VuSGCAuOSCAxCJsgqTlsUYkfAAASeieD26vfl9%2FulcRc8eteT98VM%2FfGLkCIkeWA3D2AooqaG7Tww7pAHiDA43%2F3AB%2BbYDnquWYD4s%2FHdgOf%2BBtHDHH1jsiM4l1PkTtDAMxWQaZLikAD4zkVcEqE07RKuvEEeo4VuDeTzPa79TD5wavUSdo5DkmrythB4NnRfQE34DvV%2FjXmjNGwhJ4%2FhsRoqj4LncA6yT5XqZhcEE%2FbCBLVmN3zyTsb1biIfCBGyN540bEMbqVX46NrfcjEkWwq95GKI2DPoY4FOJWLPwOO4eIrYK1AuN98GHowlZsQeAyaEW3yZ0iHbukOWnRV6j9gzcX8sRxF7BcglKZjkPBuhIvYY4CAeH8i8nhPgg94j9kx8s8gTH8i0nkIV%2BHZQuAhuBjiIxwf4JnIerFbAl6m5JD%2BfQXuidrxKqyZDTR2hGZzBz2fS53icip8v31Jy6ucrUC4p3MLPz8T08zFgQjget6Sfr%2FV9HTsr9O7ns7j28xUgl6RgST8fCxzE4wPp5zsBPujdz2dx7eezpJ%2BvUIX087HAQTw%2BkJV7ToAP%2Bs%2FQtRi8h2dHB7JwT%2FFMBtw7%2BBgPRyHyshhwIBwPjGiC8Z0FyF12SNMu3NwlIfGBf1W%2Bkzr2UiJQtUEtYL8SzX91t7L9zaAZxI%2FEhptf6OKTMlSUSd5yH7891EZ63nD5Vv3A5aZ69RWELlJHctqUNL65MBapIoladl0TiK5LefHFpnLRlIZjLdNcGr6%2FixbSfjCnsm398sJSLHkLqkKAUdF4YOaC0Tjs0vKBxJq5YDbr2Y4aQD9y5sKYIvuYEb7JuucjUJcAVEc1AI71DwBYHQ7auDocUIuq7z0eWkS1RgnrvDzCycDaHNXRaDSPZmlhbTUE6U1BR4b1hCKp9rBZOQMwAqyqVwCsDlXDYJ5Ba6BOB0Qxx%2B%2BD5%2F2xmxdm%2FxC7eaTIyWC3qAS%2BacyszMlkDUFGU9CxsUux%2F2xvRaFpB6OtHAuaPqmNBeWjybzVeZcau7k3%2FHSw28yR2zsRshmE08yhOzJ2C4VUwButAxkhlRhn32dRa81FYXvliRVZlrT1EKlyEJxPjJSqaBgQeAqSKoEuPV6qgm%2F6xAyTYkGFcP4vVZGViVo%2FCNmDG3qPlFKV861NRGEQWay01AUeAyHOA6pZkCAgGeBRE5IMuieD3sOkVIUhPOL8yGBEbRD%2ByQCPf8gPxnmvW82CA56p4PZH5F9cXX6f3d%2F%2BXq5Gn5fX0%2F9%2Fkh6jUyCCTuOjiDjAHUbnyAM7IS4UCxA1gXuKbMcJQRRxtyc4EAg808CW0zb8qEcSQQ9E0PsTDFSVYUlwwlTwAcyFIoMtusA5X6CHGLBAgWc6cGev2p9%2FP91PLl7%2BWvmb6ez6v1%2BoSldLNjg%2BG3T5HAMyEPjYF%2BwGuVBcQFYF4Qw5poIHjTsyOBQK4nGBPDg%2BBS4o4s364wI%2BDo53g1xyAeF5Cs%2BhJwgPyEPjxHtGeqyP3BKw0sBeTzZLmWE7DRhdnhSQcHC%2BO4J9HmbFPwkQfza%2BH0CjAgD48OKCVy64oEUw8EwFz%2F4%2FP9eTR%2Ft9qpvW6vXu5u19QqCCOC3kIS68InNDBpUkszxxhxT1ORrhtixm8kNmbaLJGGZtodmbjICdo%2BCgvBASCtqgbuId47P6mWaF7IS4UFs4oiYIT6fmPSPkQETsoHCDcYR%2BQOE04jqAiCyTeIhTrx0%2BoF0VHI0PeCmSuBPhkg7wYP9kuc5picQDwSAcE8gCif0zASkRpFMmwLMDOGICIcsjkoGJR3nyXC33QDQIRwUsoZ%2BSC47EBcRckE7JgBAYyg0XqPT24J4McHdg9gi8AQ8HPG1CQTwmkAniJ8AEpGSQbpmAj%2FTw3RCXTKDi2z8%2BM0EOBYJ4PCBL7xJjAU6m2Kg2ngwzGxVVQifDSfWfUZdJW33UUOIS9ZV%2FVu1rTM0cWuPy3cadt1ealIxLivOrdsrqKsORyYSjAtCKNaoBurzusn5uA6n1grrb1yn9Idow6njGqo3TAlgfG7sAjJVD3wJZBBR7U%2BmWLTMPAzUxvIziETXHrN5fAWu8Tu68bv8WvO4D%2FrQmdH8YVtV8SVXULx8PJ6PKpLwfpFU0Kw%2FrkvXWnjGBLsMggNXuob1e3gYOiHv8Cw%3D%3D
