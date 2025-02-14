# DroidKaigi公式アプリのOSS成功要因
- YAPC::ASIA HACHIOJI
- @konifar
- konifar画像
- 7/2(土)

# @konifar
- GitHubの画像

# Androidエンジニアの人？(挙手アイコン)

# OSSに興味がある人？(挙手アイコン)
> 自慢は少しにする

# DroidKaigi
- 2/18(土) - 19(日)
- Androidの大きなイベント
- DroidKaigiの画像

# 公式アプリ
- 公式アプリの画像
- 公式アプリのURL

# 前夜祭のような凄まじい盛り上がり

# 35人ものContributors
- 画像

# 184 PRs、114 Issues
- 画像

# (パンチカード)
- 画像

# (Code frequency)
- 画像
- 終わってからも続いている

# 韓国語サポート
- 画像

# 継続的なライブラリのアップデート
- 画像
- Thanks @shaunkawano!

# 今回のOSSで失敗したこと、やってよかったことの話をします
> すべて考えてやっていたわけではない。今思えばあれがよかったなぁと思えることをいくつか整理したので話します。
> OSSってなんかこわいと思ってる人が、コードを公開してみようかなと思える話をします。

# DroidKaigiアプリのOSS成功要因

1. Issueとマイルストーンを活用する
> welcomecontributorラベル
> Issueの粒度を小さくする
> 締め切りの意識を持たせる
> waffle.io
> ツールは増やさない
> できないこともおくせず書いておくこと
> 勢い大事。仕事じゃないから

- contributionの敷居を下げる
> contributorsページを作った
> ReadMeの整理
> Issueの整理
> もちろん英語じゃなくてもいい

- 英語でやりとりする
> 意外に優しい世界になる
> 海外の人も来る。Well done sirのエピソード
> 海外からの連絡も来る

- レビューを高速に回す
> テストを捨てる判断
> いつでも見てるアピール
> 迷わないパッケージ構成
> CI、Deploygate
> gfxさんの時の失敗

- 様々な手段で広く周知する
> ブログ
> Android Arsenal
> Google+
> Twitter、Facebook

# 1. Issueとマイルストーンを活用する

# マイルストーン
- 締め切りの意識を明確にする

# welcomecontributorラベル
- どれをやったらいいかがひと目でわかる
- welcome感が出て取りやすい

# waffle.io（カンバン）
- Issueの可視化
- タスク管理ツールはあんまり増やさない


# 勢いのfun issue
- 勢いで楽しそうなことを書いとく
- 仕事じゃないのでゆるくやる


# 何をいつまでにやればいいかを明確にすることでとっつきやすくなる
> そこからさらにとっつきやすくするために次の話

# 2. contributionの敷居を下げる

# ReadMeの整理
- どういう構造なのかを簡単に書いておくだけでもだいぶ違う

# Issueの粒度を小さく
- 15分くらいでできそうなものも書いとく
- 自分でもできそう？と思ってもらう

# Issueの棚卸し
- welcomecontributorラベルの貼り直し
- 古いIssueのクローズ
- 常に最新に保つことで混乱をなくす
- 簡単な細々したものもIssueにざっと書き出しておく

# 自分にできないことも書いておく
- (画像)
- 自分でできないことのリスト

# Contributorsページ
- 圧倒的感謝を形にする
- 実はこれもContributorの方が作ってくれた


# 私でもできそう、なんか楽しそう、contributionしたいと思ってもらえる
> けど、ここまで見てきたものは英語で、それってとっつきにくいんじゃないの？という人もいそう。

# 3. 英語でやりとりする

# 英語縛りでやさしい世界

# きっかけ
- プラグインのWell done sir!の画像
- めちゃくちゃテンションが上がった

# (DroidKaigiのやりとりの画像1)

# (DroidKaigiのやりとりの画像2)

# 日本語の時よりみんなやさしい気がする…？

# +α 海外からの連絡
- 韓国語の翻訳サポート
- インドのカンファレンスの公式アプリとしてForkさせてくれとの連絡


# レビューを高速に回す

# いつでも見てる感を出す
- 簡単なIssueだと1分もかからない
- 間違ったら直せばいい

# レビュー放置の失敗とまなび
- gfxさんの時の失敗画像
- 判断に迷う時、何もしないのが一番ダメ
- PRなら、とりあえずマージかクローズかを明確に
- 今判断できなければその旨をコメントにしてクローズしておくのが得策

# 厳密にやらない

# 環境の構築
CI、Deployは自動化しておく
コーディングルール、チェックスタイル、機械的なレビューも自動化しておけばよかった

# 迷わないパッケージ構成
(画像)
- Androidではベストなパッケージ構成というのがない。
- MVVM、MVP、はたまたDDDなど、設計によってわかりやすいそれぞれパッケージ構成が変わってる印象
- どれが正解とかはない。

# 例えば
機能ごとに分ける
レイヤーごとに分ける
などいっぱいあるが、contributorが迷わない構成を心がけることにした

> 例えばさっきのcontributorページ、新しくパッケージを切っていいのかなと迷う。パッケージを新しく切ることにわりと迷うこともある。その結果、レビューでこれはこっちのパッケージに入れてくださいみたいになるのもめんどくさい。

# レビューを高速に回すことでスピード感を保つ
- OSSは長期間のモチベーションを保つのがわりと難しい
- contributorには圧倒的感謝を持って速攻のレビューをする

> けどそもそもそんなに人集まらないんだけど？という話があります。最後にそのへんをさらいます。

# 様々な手段で広く周知する

# 何もいわなかったら人は来ない

# Star数の貢献度（Androidの場合）
1. Android Arsenal
2. Google+
3. Twitter、Facebook、ブログ

# Android Arsenal
- AndroidのライブラリやOSSアプリを紹介するサービス
- iOSもRailsも、ある程度コミュニティの大きいフレームワーク・言語なら何かしらあると思う。

# Google+
- Androidだからというのもあるが、わりといろんな人に届く
- 特に海外の人は結構使ってる

# Twitter、Facebook
- DroidKaigiの公式Twitterで周知してもらえたのはでかかった（ラッキー）
- 日本だとTwitterやブログでも結構広められる。とりあえず書いてみた方がいい

# 広めるの怖い？
- (おれのTweet画像)
- すげえ叩かれるんじゃないかな
- コード見られるの恥ずかしい

# 安心してください、皆そんなに見てません

# ちゃんと見てくれてる人は優しい
- PR送ってくれるような人は大丈夫
- 言われたら直せばいいんです
- 自分の手が届かなかった実装をぶっこまれるのが醍醐味

# 不安なのはわかる。ただトライしてみるのが吉と言いたい


# +α

# Q. いつ仕事するのか？

# A. 毎日してました

# Twitterの画像

# 睡眠は取らないとダメ
- Contributorの人にもっとお任せすればよかったかも
- 楽しくてついつい見てしまっていたので苦ではなかった

# まとめ

# OSSはこわい？

# 気持ちはわかる

# とりあえず公開してみるとよいかもしれない

# OSSで皆でものを作るの楽しいし学びがある

# いい感じの画像

# ありがとうございました
