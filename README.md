## Install_Docker
Install Docker on Linux ( CentOS 9 )


Install yum-utils package, which provides utilities for managing Yum repositories and packages.
```
sudo yum install -y yum-utils
```

Add the Docker CE repository to the Yum configuration manager.
```
sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
```

Install Docker CE, Docker CLI, containerd.io, docker-buildx-plugin, and docker-compose-plugin using Yum.
```
sudo yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin -y
```

Check the status of the Docker service using systemctl.
```
systemctl enable docker.service
systemctl start docker.service
systemctl status docker.service
```

Run the "hello-world" Docker container to verify the Docker installation.
```
sudo docker run hello-world
```
