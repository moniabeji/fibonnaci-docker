# Building a multi container application (react, postgres redis, expres nginx)

## Install settings
```
# install nodejs
yum install -y gcc-c++ make
curl -sL https://rpm.nodesource.com/setup_12.x | sudo -E bash -
Step 2 – Install Node.js on CentOS
After adding a yum repository in your system lets install Node.js package. NPM will also be installed with node.js. This command will also install many other dependent packages on your system.
sudo yum install nodejs

how to update version of node:
sudo npm cache clean -f
sudo npm install -g n
sudo n stable


# install docker compose
https://docs.docker.com/compose/install/
sudo curl -L "https://github.com/docker/compose/releases/download/1.25.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose

# install react app
npx create-react-app client


```

# ERROS IN some installation
```
 ****sudo: docker-compose: command not found
 https://docs.docker.com/compose/install/
 If the command docker-compose fails after installation, check your path. You can also create a symbolic link to /usr/bin or any other directory in your path.

 For example:
 sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose

 ***fixlink to old node version
 rm -f /bin/node
 ln -s /usr/local/bin/node /bin/node
 n stable

 ***fix create react app
 export PATH=/usr/local/bin:$PATH
```