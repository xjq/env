FROM ubuntu
RUN apt-get update \
    && apt-get install -y git python \
    && git clone -b manyuser https://github.com/shadowsocksrr/shadowsocksr.git
COPY shadowsocks.json shadowsocks.json
EXPOSE 1080
CMD "python shadowsocksr/shadowsocks/local.py -c shadowsocks.json -d start" 
