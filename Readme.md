# Git Init
a new file was created cd'ed into and intialise with as a git repository as shown with syntax below
git img
![init](./img/Git%20init.png)
# Extracting file from the web
A website Template from Tooplate was download and extracted into the MarketPeak_Ecommerce directory. see image below
![unzip](./img/unzip%20syntax.png)
![Unzipimg](./img/rename%20unzip.png)

# Editing the index.html file in VScode
the template downloaded from tooplate wass edited to suit MarketPeak Ecommerce using VScode
![Market.web](./img/editing%20template%20using%20vscode.png)

[.htmlfile](./index.html)

# Pushing codes to git
a MarketPeak_Ecommerce repository was created on github, the initialise local repository was staged, commited and pushed to github
![init](./img/git%20repo.png)
![init](./img/initial%20commit.png)
![init](./img/git%20push%20syntax.png)



# Creating an EC2 Instance
an EC2 instance was created on AWS
![Ec2](./img/EC2%20aws.png)
![Ec2 syntax](./img/konect2Ec2%20syntax.png)

# cloning git repo to EC2 

MarketPeak's repo on github was cloned to the EC2 server using http as shown in pictures below
![http](./img/cloning%20on%20github.png)
![init](./img/cloning%20syntax.png)

# Setting Apache2 on EC2
apache2 was configured on the EC2 instance using these commanads

    * sudo apt update -y
    * sudo apt install apache2

![init](./img/installing%20apache.png)

## it was then started and enabled using
    * sudo systemctl start apache2
    * sudo systemctl enable apache2
    * sudo systemctl status

![apache](./img/setting%20up%20apache.png)
![apache2](./img/setting%20up%20apache.png2.png)

## preparing the web directory
the apache web directory was cleared and replace with MarketPeak Ecommerce's files using

    * sudo rm -rf /var/www/html/*
    * sudo cp -r ~/MarketPeak/_Ecommerce/* /var/www/html

the apache2 was then reloaded using 
    * sudo systemctl reload apache2

as shwon ![aperld](./img/setting%20up%20apache.png2.png)

# Accessing the we from Browser
MarketPeak's browser couldn't be access using the public IP address, hence the EC2 instances security was configured by setting up an http for port 80 as shown

![port](./img/setting%20up%20port%20on%20aws.png)
![init](./img/inbound%20rule.png)

# Image of MarketPeach's website on Browser
see image below
![img](./img/mktpeak.png)