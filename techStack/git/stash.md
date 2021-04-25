# git stash 変更を一時的に退避
git-stash - Stash the changes in a dirty working directory away  
stash: こっそりしまう、隠す  

[シチュエーション]
- checkoutせずに作業始めてしまい、別ブランチに行きたい時

```
$ git stash  # 変更状態を一時避難

$ git checkout <別ブランチ>

$git stash pop # 一時避難していた変更状態を元に戻す
``` 
- 作業中に、add-commitをせずに別ブランチに行きたい時
```
# ブランチAで作業中、別の作業が生まれたのでブランチBに行きたい！
$ git stash  # 変更状態を一時避難

$ git checkout <ブランチB>

# ブランチBの作業が完了したのでブランチAに戻る
$ git checkout <ブランチA>

$git stash pop # 一時避難していた変更状態をブランチAで元に戻す
``` 
