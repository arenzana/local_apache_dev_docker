# Run an Apache instance

##Installation

Put files to be served under www and edit apache-config.conf to your heart's content.

```
git clone https://github.com/iarenzana/local_apache_dev_docker.git
cd local_apache_dev_docker
docker build -t apache-instance .
docker run -v ${HOME}/tmp/apache_instance_logs:/var/log/apache2 -p 80:80 -d apache-instance
```
