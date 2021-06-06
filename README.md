# geth-installation

wget https://golang.org/dl/go1.16.5.linux-amd64.tar.gz

sudo tar -C /usr/local -xzf go1.16.5.linux-amd64.tar.gz

gedit .bashrc

#for go setting
GOROOT=/usr/local/go
GOPATH=~/.go
PATH=$PATH:$GOROOT/bin:$GOPATH/bin
