# About

This is a skeleton of Go workspace. There are two script which should be sourced. 

* Assuming we use Go 1.7, installed at GODEVTOOLS_HOME

```
GODEVTOOLS_HOME=/opt/software/go-dev-tools

GO_HOME=$GODEVTOOLS_HOME/go/go1.7.0
LITEIDE_HOME=$GODEVTOOLS_HOME/liteide
GOTOOLS=$GODEVTOOLS_HOME/go-tools

export GOROOT=$GO_HOME
export GOOS=linux
export GOARCH=amd64
export GOHOSTOS=linux
export GOHOSTARCH=amd64

# https://golang.org/cmd/go/#hdr-GOPATH_environment_variable
# a)    If you don't set your GOBIN env variable, 
#       you get the Go compiler binaries going in 
#       GOROOT/bin whereas the your binaries are going 
#       in GOPATH/bin. (I personally like this separation of 
#       binaries.)
# (b)   If you set your GOBIN to anything, then both the Go 
#       binaries and your binaries are going to GOBIN.
#export GOBIN=$GOROOT/bin

export PATH=$PATH:$GO_HOME/bin:$LITEIDE_HOME/bin:$GOTOOLS

alias go=colorgo
```

* [env.sh](env.sh)
