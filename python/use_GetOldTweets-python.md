# GetOldTweets-python パッケージを利用して古いツイートを取得してくる

導入やパッケージについては[GetOldTweets-python](https://github.com/Jefferson-Henrique/GetOldTweets-python)を
参照すること  
GetOldTweets-python はOAuth認証無しにツイートの内容を取ってくることが可能  
(中身を見ると、スクレイプを利用しているっぽい)  
逆に、アカウントを利用してツイートを投稿することなどはできない  

詳しくは[GetOldTweets-python](https://github.com/Jefferson-Henrique/GetOldTweets-python)のREADME.mdを見る必要があるが  
例えば、次のコードを利用することで  
「2020-01-01以降の"TegeTege_workout"と言うワードが入ったツイート」  
を取得することが可能である

```
import got3
# クエリーが入っているツイートを取ってくる
# オプションで検索範囲の日付が指定できる
tweetCriteria = got3.manager.TweetCriteria().setQuerySearch('TegeTege_workout').setSince('2020-01-01')
tweets = got3.manager.TweetManager.getTweets(tweetCriteria)

for i in range(len(tweets)):
	tweet = tweets[i]
	print(tweet.text)
  

〜〜　出力　〜〜
#tegetege _ workout [みんなで筋肉体操] 腕立て伏せ ～ 厚い胸板をつくる ～ | NHK https:// youtu.be/WndOChZSjTk @YouTube より
#tegetege _ workout [みんなで筋肉体操] 腹筋 2 ～ 続・凹凸ある腹筋をつくる／Crunches ～| NHK https:// youtu.be/cjvgjxIra9k @YouTube より
#tegetege _ workout [みんなで筋肉体操] 腹筋 2 ～ 続・凹凸ある腹筋をつくる／Crunches ～| NHK https:// youtu.be/cjvgjxIra9k @YouTube より
コレを取り入れてみよう #tegetege _ workout https:// twitter.com/karetakoe/stat us/1216984789430886400 …
社食に朝食を食べに行くときは階段で6UP, 6DOWN #tegetege _ workout
#tegetege _ workout pic.twitter.com/UKebtssYvV
正月でなまった身体を鍛え直す #tegetege _ workout [みんなで筋肉体操] 腕立て伏せ ～ 厚い胸板をつくる ～ | NHK https:// youtu.be/WndOChZSjTk @YouTube より
#tegetege _ workout [みんなで筋肉体操] 腹筋 2 ～ 続・凹凸ある腹筋をつくる／Crunches ～| NHK https:// youtu.be/cjvgjxIra9k @YouTube より
```
