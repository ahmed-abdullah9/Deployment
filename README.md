# Deployment

# This is the Final Project of Full Stack Development


Public ip : 104.248.217.106
Port: 2200 

The complete URL to hosted web application :>  104.248.217.106.xip.io

  To login
      ssh grader@104.248.217.106 -p 2200 -i ~/.ssh/grader
      
  # Config :> 
      Configure the Uncomplicated Firewall (UFW) to only allow incoming connections for SSH (port 2200), HTTP (port 80), and NTP (port 123).

  sudo ufw allow 2200/tcp
  
  sudo ufw allow 80/tcp
  
  sudo ufw allow 123/tcp
  
  sudo ufw enable
  
  Adding user :> 
    sudo adduser grader
    
  Give grader the permission to sudo:>
  
      sudo vim /etc/sudoers.d/grader
      
      add text: grader ALL=(ALL) NOPASSWD:ALL

# installations : 
sudo apt install python-pip


sudo pip install --upgrade pip

sudo pip install Flask

sudo pip install httplib2

sudo pip install requests

sudo pip install oauth2client

sudo pip install sqlalchemy


Resources 
https://www.digitalocean.com/docs/droplets/how-to/create/
