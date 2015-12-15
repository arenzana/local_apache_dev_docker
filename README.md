# Run an Apache instance

##Installation

Put files under www and edit apache-config.conf

```
docker build -t apache-instance .
docker run -v /tmp:/var/log/apache2 -p 80:80 -d apache-instance
```
