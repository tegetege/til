# eval と exec

## はじめに
競プロ過去問を解くのに
https://atcoder.jp/contests/abc050/tasks/abc050_a

eval()を使ったこの回答がかっこよかったので、
https://atcoder.jp/contests/abc050/submissions/9134181

eval とexec をまとめる

## eval とは
`eval`は第1引数を`式として評価`
```
>>> eval('1+2')
3

>>> x = 1
>>> eval('x+1')
2

# 第1引数に文(代入文)を入れるとエラー
>>> eval('a=1+2')
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
  File "<string>", line 1
    a=1+2
     ^
SyntaxError: invalid syntax

```

## exec とは
`exec`は第1引数を`文として実行`
```
>>> exec('a = 1 + 2')
>>> exec('print(a)')
3
```


## リンク
[eval](https://docs.python.org/ja/3/library/functions.html#eval)  
[exec](https://docs.python.org/ja/3/library/functions.html#exec)
