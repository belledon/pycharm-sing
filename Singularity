bootstrap: docker
from: ubuntu:16.04

%runscript
  cd /pycharm-src/pycharm-community-2017.3.2/bin
  ./pycharm.sh

%post
  apt-get update
  apt-get install --no-install-recommends -y wget \
                      openjdk-9-jre \


  mkdir /pycharm-src && cd /pycharm-src
  wget https://download.jetbrains.com/python/pycharm-community-2017.3.2.tar.gz
  tar -xvzf pycharm-community-2017.3.2.tar.gz
  rm pycharm-community-2017.3.2.tar.gz
