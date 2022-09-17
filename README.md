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
# Varun's Blog
- https://varunmanik1.medium.com/a-simple-machine-learning-step-by-step-tutorial-with-the-help-of-amazon-translate-lambda-api-1cc200bf2212

# References

1. https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instancedata-add-user-data.html
2. https://aws.amazon.com/certification/certified-solutions-architect-associate/
3. https://docs.aws.amazon.com/AWSEC2/latest/WindowsGuide/connecting_to_windows_instance.html
4. https://en.wikipedia.org/wiki/Hypervisor
5. https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-using-volumes.html
6. https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/recognize-expanded-volume-linux.html
7. https://www.w3schools.com/html/default.asp
