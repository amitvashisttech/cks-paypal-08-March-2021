# In the following demo will be setting up 3 Node Kubernetes Cluster ( 1 Master & 2 Workers ) 

## For this demo will be required to have following tools installed. 
1.	Virtual Box
2.	Vagrant 
3.	Cmder / Git Bash 

## First clone this repository on your windows machine.

```
git clone https://github.com/amitvashisttech/cks-paypal-08-March-2021.git
``` 

## You can skip the below steps in case you have a cloud instances. 

## Now provision three virtual machines with following commands:

```
cd cks-paypal-08-March-2021/Kubernetes/
vagrant.exe up

vagrant.exe status
Current machine states:

master                    running (virtualbox)
worker1                   running (virtualbox)
worker2                   running (virtualbox)
```

## Login to master node & clone the repo after that execute install-kubernetes.sh. 

```
vagrant.exe ssh master
sudo su - 
git clone To https://github.com/amitvashisttech/cks-paypal-08-March-2021.git
cd cks-paypal-08-March-2021/00-Setup
sh Docker/00-Setup/install-docker.sh
```
