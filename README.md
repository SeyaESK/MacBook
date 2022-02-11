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

# Python
- pyenvインストール
```
brew install pyenv
```

- zsh設定
```
export PYENV_ROOT="$HOME/.pyenv"
export PATH="$PYENV_ROOT/bin:$PATH"
export PATH="$PYENV_ROOT/shims:$PATH"
eval "$(pyenv init --path)"
eval "$(pyenv init -)"
source ~/.zshrc
```

- PATHの設定を.zshrcに保存しておく

- 確認
```
pyenv install --list
```

- インストール
```
pyenv install 3.9.10
```

- 確認
```
pyenv versions
```

### pyenv Local Global
- Local
  - pyenv localと実行したディレクトリ内だけで、Pythonのバージョンが固定される
- Global
  - ディレクトリを超えて利用されるバージョン

- Local設定
```
pyenv local 3.9.9
```

- Global設定
```
pyenv global 3.9.10
```