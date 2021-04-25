# timedeltaオプジェクトを利用して日付を計算したい

timedeltaオブジェクトを利用すれば2つの日付や時間間の差、2つの時間を計算した結果などが出せる  

```
from datetime import timedelta

>>> week = timedelta(days=7)
>>> today = datetime.date.today() # 2020/02/18

>>> one_week_ago = today - week
datetime.date(2020, 2, 11)
```
参考リンク
Python docs datetime :
https://docs.python.org/ja/3/library/datetime.html#examples-of-usage-timedelta
