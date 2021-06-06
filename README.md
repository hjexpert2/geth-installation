# geth-installation

wget https://golang.org/dl/go1.16.5.linux-amd64.tar.gz

sudo tar -C /usr/local -xzf go1.16.5.linux-amd64.tar.gz

gedit .bashrc

#for go setting
GOROOT=/usr/local/go
GOPATH=~/.go
PATH=$PATH:$GOROOT/bin:$GOPATH/bin


sudo update-alternatives --install "/usr/bin/go" "go" "/usr/local/go/bin/go" 0
sudo update-alternatives --set go /usr/local/go/bin/go

go version


git clone https://github.com/ethereum/go-ethereum.git

cd go-ethereum/

make

sudo cp build/bin/geth /usr/local/bin/

geth version


