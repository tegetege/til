# 日ずけを扱う
### datetime オブジェクト  
日ずけの差を計算する
```
import datetima

today = datetime.date.today()  # datetime.date(2019, 11, 18)
pre_day = datetime.date(2019, 11, 1)

gap = today - pre_date  # 18 days, 00:00:00
print(gap.days) # 18
```


参考サイト  
[Pythonで経過時間や日時（日付・時刻）の差分を測定・算出](https://note.nkmk.me/python-datetime-timedelta-measure-time/)
