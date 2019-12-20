# PhantomJS + Selenium

## 설치 및 세팅

### docker cli

```dockerfile
docker pull ubuntu:16.04
docker run -it ubuntu:16.04
```

### ubuntu

```
apt-get update
apt-get install -y python3 python3-pip
pip3 install selenium
pip3 install beautifulsoup4
apt-get install -y wget libfontconfig
mkdir -p /home/root/src && cd $_
wget https://bitbucket.org/ariya/phantomjs/downloads/phantomjs-2.1.1-linux-x86_64.tar.bz2
tar jxvf phantomjs-2.1.1-linux-x86_64.tar.bz2
ls
cd phantomjs-2.1.1-linux-x86_64/bin/
ls
cp phantomjs /usr/local/bin/
apt-get install -y fonts-nanum*
exit
```

### docker cli

```dockerfile
docker ps -a
docker commit <컨테이너아이디> ubuntu-phantomjs
docker run -i -t -v /d/sample:/sample -e ko_KR.UTF-8 -e PYTHONIOENCODING=utf_8 ubuntu-phantomjs /bin/bash
cd /sample/
```

> selenium에서 더이상 phantomjs를 지원하지 않습니다.

