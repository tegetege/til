# アスタリスクを利用して変数(リスト・辞書)を展開する

配列や辞書などを*(アスタリスク)記号を使って展開することが可能

```
test = [1,2,3]

print([test,4,5])  #[[1, 2, 3], 100, 101]
print([*test,4,5])  #[1, 2, 3, 100, 101]

```

辞書の場合は、アスタリスクを２個利用

```
car = {'TOYOTA':'LEVEN','MITSUBISHI':'FTO'}

print({**car,'MAZDA':'RX-7'})   #{'TOYOTA': 'LEVEN', 'MITSUBISHI': 'FTO', 'MAZDA': 'RX-7'}

```



### 参考サイト
[Python中級者への道しるべ - Qiita](https://qiita.com/papi_tokei/items/2aef9a259fd236d340da#%E5%A4%89%E6%95%B0%E3%81%AE%E5%B1%95%E9%96%8B)
