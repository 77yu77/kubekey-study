## 安装go环境

wget https://golang.google.cn/dl/go1.18.1.linux-amd64.tar.gz

tar -xzf go1.18.1.linux-amd64.tar.gz -C /usr/local

export PATH=$PATH:/usr/local/go/bin

echo "export PATH=$PATH:/usr/local/go/bin" >> ~/.bashrc

go env -w GO111MODULE=on

go env -w GOPROXY=https://goproxy.cn,direct

go mod tidy

## 安装cobra

go get -u github.com/spf13/cobra/cobra

