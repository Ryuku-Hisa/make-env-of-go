# make-env-of-go
goの環境構築をgo envでやるやつを自動化したい


-memo-

`goの環境構築をするスぺニット`
```
export GOENV_ROOT="$HOME/.goenv"
if [ -e $GOENV_ROOT ]; then
  export PATH="$GOENV_ROOT/bin:$PATH"
  eval "$(goenv init -)"
  export PATH="$GOROOT/bin:$PATH"
  export PATH="$PATH:$GOPATH/bin"
fi
```
