# aws-sa-tutorial
Aws Solution-Architect-Tutorial 

# How to install Web-server

```
sudo yum install httpd -y

sudo service httpd start
sudo service httpd status

sudo /var/www/html/
sudo vim  /var/www/html/index.html

sudo chkconfig httpd on 
```
# instance meta-data

```

sudo curl http://169.254.169.254/latest/meta-data/public-ipv4
curl http://169.254.169.254/latest/
curl http://169.254.169.254/latest/meta-data
curl http://169.254.169.254/latest/meta-data/ami-id

```
