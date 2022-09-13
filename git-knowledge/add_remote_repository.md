# Gitリポジトリにリモートリポジトリを追加する

## 今回の前提
githubを使用

## 方法
1. github上で、リポジトリを作成しておく
- `create repository`から作成可能
  - 中身は空でもOK
  
2. `git remote add <name> <url>`を実行する
- nameは原則`origin`
- urlには、1. で作成したリポジトリのurlを入れる

無事に追加できたら`git remote`で正しくリモートリポジトリが設定されたか確認する
```
     ~/documents/SelfProjects/til master*
       ❯ git remote -v
         origin  https://github.com/bluepegasusyk/til (fetch)
           origin  https://github.com/bluepegasusyk/til (push)
```

- `-v`オプションをつけることで、fetch/push両方の対応するURLが表示される
