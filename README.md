# golang-starter

## installation Guide of golang 1.11 for linux distros

$ sudo apt-get update
$ sudo apt-get -y upgrade

Downlaod the golang 1.11 from Offical golang website [Offical Download page](https://golang.org/dl/)

Next, you need to extract the files from the archive downloaded by running the command:

$ sudo tar -xvf go1.10.linux-amd64.tar.gz
Next, move the go folder to the final destination:

$ sudo mv go /usr/local

### Setup GO ENVIRONMENT VARIABLES

In order to be able to use the Go language, the GOROOT, GOPATH and PATH environment variables need to be set up.

GOROOT is the location where Go package is installed on your system, in our case /usr/local/go. Run the following command to set up the variable:

$ export GOROOT=/usr/local/go
GOPATH is the location of your work directory. Run the following command to set up the variable using your own folder:

$ export GOPATH=$HOME/Golang
Next, set up the PATH variable to access go binary system-wide.

$ export PATH=$GOPATH/bin:$GOROOT/bin:$PATH
All three environment variables will be set for your current session only. If you want to make it permanent add the commands in ~/.profile file. You can edit the file using the vi editor.

$ vi ~/.profile

### Verify Installation
To verify the go version just type the following command, if everything went well the go version will be displayed:

$ go version
go version go1.10 linux/amd64

To verify all the go variables, run the following command:

$ go env

GOARCH="amd64"
GOBIN=""
GOEXE=""
GOHOSTARCH="amd64"
GOHOSTOS="linux"
GOOS="linux"
GOPATH="/home/adm/Repositories/admfactory"
GORACE=""
GOROOT="/usr/local/go"
GOTOOLDIR="/usr/local/go/pkg/tool/linux_amd64"
GCCGO="gccgo"
CC="gcc"
GOGCCFLAGS="-fPIC -m64 -pthread -fmessage-length=0 -fdebug-prefix-map=/tmp/go-build698684453=/tmp/go-build -gno-record-gcc-switches"
CXX="g++"
CGO_ENABLED="1"
CGO_CFLAGS="-g -O2"
CGO_CPPFLAGS=""
CGO_CXXFLAGS="-g -O2"
CGO_FFLAGS="-g -O2"
CGO_LDFLAGS="-g -O2"
PKG_CONFIG="pkg-config"



### You are done now.
### Happy Coding!!!

