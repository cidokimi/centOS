//to install firewalld

sudo yum install -y firewalld

sudo systemctl enable firewalld

sudo systemctl restart firewalld

sudo systemctl reload firewalld

sudo systemctl start firewalld

sudo systemctl stop firewalld

sudo firewall-cmd --state



//to see which zone is selected

sudo firewall-cmd --get-default-zone

sudo firewall-cmd --help



//to list for all zones

sudo firewall-cmd --list-all-zones



//to list for open ports

sudo firewall-cmd –-list-ports



//to list for all services

sudo firewall-cmd --list-services



//to open tcp port 6443 

sudo firewall-cmd --permanent --add-port=6443/tcp



//to open udp port 5180

sudo firewall-cmd --permanent --add-port=5180/udp



//to save the configurations that you do and get access

sudo firewall-cmd --reload
