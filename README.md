### Introduction
Fork of a very basic ETH pool with support for Memcache and MySQL

### Supported clients
This code is intended to support Genoil's ethminer port, both getWork and some hacked form of stratum support.

### Pull requests & possible optimizations
If you find any issues with the pool software please feel free to issue a pull request.

### Setup guide using Ubuntu 15.10 (Wily Werewolf)
* Install and configure Go<br />
*Check the latest version of GoLang here:* https://golang.org/dl/
```bash
cd ~
curl -O https://storage.googleapis.com/golang/go1.6.2.linux-amd64.tar.gz
tar xzf go1.6.2.linux-amd64.tar.gz
mkdir gomodules
echo "export GOROOT=$HOME/go" >> .profile
echo "export PATH=$PATH:$GOROOT/bin" >> .profile
echo "export GOPATH=$HOME/gomodules" >> .profile
```

* Clone the repo
`git clone https://github.com/davembg/ethpool-core.git`

* Grab the dependencies
```bash
go get github.com/ethereum/go-ethereum/common
go get github.com/gorilla/mux
go get github.com/kklis/gomemcache
go get github.com/go-sql-driver/mysql
```
* { incomplete }
