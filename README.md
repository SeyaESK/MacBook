M1 MacBook Air SetUp
====

# Node.js
```
$ brew install nodebrew
```

```
$ nodebrew setup
```

```
$ echo 'export PATH=$HOME/.nodebrew/current/bin:$PATH' >> ~/.zshrc
```

- Node.jsの安定版インストール
```
$ nodebrew install stable
```

- インストールされているNode.jsバージョン確認

```
$ nodebrew ls 
```

- Node.js の有効化
```
$ nodebrew use v16.6.2
```

- Node.js確認
```
$ node -v
```