//to see selinux config file
cat /etc/selinux/config




//to check selinux status

sudo getenforce

sudo sestatus 




//to disable selinux

sudo sed -i s/^SELINUX=.*$/SELINUX=disabled/ /etc/selinux/config

sudo setenforce disabled





//to load selinux security policy

sudo sed -i s/^SELINUX=.*$/SELINUX=enforcing/ /etc/selinux/config

sudo setenforce enforcing




//to be logged in the audit log

sudo sed -i s/^SELINUX=.*$/SELINUX=permissive/ /etc/selinux/config

sudo setenforce permissive




sudo reboot
