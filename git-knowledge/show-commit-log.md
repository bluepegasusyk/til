# コミット履歴を表示する

`git log`コマンドを使用する
- 以下のように、comment等合わせたcommit履歴を見ることができる
```
  $ git log
  commit ca82a6dff817ec66f44342007202690a93763949
  Author: Scott Chacon <schacon@gee-mail.com>
  Date:   Mon Mar 17 21:52:11 2008 -0700
  
      changed the version number
      
      commit 085bb3bcb608e1e8451d4b2432f8ecbe6306e7e7
      Author: Scott Chacon <schacon@gee-mail.com>
      Date:   Sat Mar 15 16:40:33 2008 -0700
      
          removed unnecessary test
          
          commit a11bef06a3f659402fe7563abf99ad00de2209e6
          Author: Scott Chacon <schacon@gee-mail.com>
          Date:   Sat Mar 15 10:31:28 2008 -0700
          
              first commit
```

## -pオプション

-pオプションを付けることで、各コミットでの変更点を表示できる

```
  ❯ git log -p
  commit e08ee7fb0fc9280bbc9d73eaead444eb51a0562d (HEAD -> maste
  Author: Kana Yamazaki <bluepegasusyk@gmail.com>
  Date:   Wed Sep 14 00:17:27 2022 +0900
  
      リモートリポジトリの追加について
      
      diff --git a/git-knowledge/add_remote_repository.md b/git-know
      new file mode 100644
      index 0000000..196c76f
      --- /dev/null
      +++ b/git-knowledge/add_remote_repository.md
      @@ -0,0 +1,23 @@
      +# Gitリポジトリにリモートリポジトリを追加する
      +
      +## 今回の前提
      +githubを使用
      +
      +## 方法
      +1. github上で、リポジトリを作成しておく
      +- `create repository`から作成可能
      +  - 中身は空でもOK
      +
      +2. `git remote add <name> <url>`を実行する
      +- nameは原則`origin`
      +- urlには、1. で作成したリポジトリのurlを入れる
      +
      +無事に追加できたら`git remote`で正しくリモートリポジトリが設
      +```
        +     ~/documents/SelfProjects/til master*
        +       ❯ git remote -v
        +         origin  https://github.com/bluepegasusyk/til (fetch)
        +           origin  https://github.com/bluepegasusyk/til (push
        +````)
      `)
```
