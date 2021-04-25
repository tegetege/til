# joinを使ってリストをくっつける

[シチュエーション]  
標準出力で、配列になっているのをくっつけて表示したい  
`['H', 'e', 'l', 'l', 'o', ' ', 'W', 'o', 'r', 'l', 'd']`  
→　`Hello World`

```
#　配列の生成
>>> H = list(input())
TOYOTA LEVEIN
>>> H
['T', 'O', 'Y', 'O', 'T', 'A', ' ', 'L', 'E', 'V', 'E', 'I', 'N']


>>> ''.join(H)
'TOYOTA LEVEIN'

>>> '-'.join(H)
'T-O-Y-O-T-A- -L-E-V-E-I-N'
```
