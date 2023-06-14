# centos7 install docker

# remove docker
sudo yum remove docker \
                  docker-client \
                  docker-client-latest \
                  docker-common \
                  docker-latest \
                  docker-latest-logrotate \
                  docker-logrotate \
                  docker-engine

# set up repository
sudo yum install -y yum-utils
sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo


# install the latest version
sudo yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin


# daemon.json
{
  "registry-mirrors": [
    "https://docker.m.daocloud.io"
  ]
}


