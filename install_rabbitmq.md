
# erlang
```shell
cd /opt
yum install -y make gcc gcc-c++ kernel-devel m4 ncurses-devel openssl-devel unixODBC-devel
wget https://github.com/erlang/otp/releases/download/OTP-27.3.2/otp_src_27.3.2.tar.gz
tar -xzvf otp_src_27.3.2.tar.gz
cd otp_src_27.3.2
./configure --prefix=/usr/local/erlang --without-javac
make 
make install

/usr/local/erlang/bin/erl -version
echo 'export PATH=$PATH:/usr/local/erlang/bin' >> ~/.bashrc
source ~/.bashrc
```

# rabbitmq
```shell
cd /opt
wget https://github.com/rabbitmq/rabbitmq-server/releases/download/v4.0.8/rabbitmq-server-generic-unix-4.0.8.tar.xz
# wget https://github.com/rabbitmq/rabbitmq-server/releases/download/v4.0.8/rabbitmq-server_4.0.8-1.debian.tar.xz
# wget https://github.com/rabbitmq/rabbitmq-server/releases/download/v4.0.8/rabbitmq-server_4.0.8-1_all.deb
tar -xvf rabbitmq-server-generic-unix-4.0.8.tar.xz
mv rabbimt_server_4.0.8 /usr/local/rabbitmq
echo 'export PATH=$PATH:/usr/local/rabbitmq/sbin' >> ~/.bashrc
source ~/.bashrc
```
```
# https://raw.githubusercontent.com/rabbitmq/rabbitmq-server/refs/heads/main/deps/rabbit/docs/rabbitmq.conf.example
# https://raw.githubusercontent.com/rabbitmq/rabbitmq-server/refs/heads/main/deps/rabbit/docs/rabbitmq-server.service.example
```
