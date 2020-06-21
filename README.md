# TestDocker

sudo apt update
sudo apt upgrade

#ganti nama host
sudo hostnamectl set-hostname pi-manager

#Get the tool or update
curl -SLsf https://get.k3sup.dev | sudo sh

#Start a new cluster
k3sup install --ip $SERVER_IP --user pi
Join an agent/worker into the cluster

k3sup join --ip $AGENT_IP --server-ip $SERVER_IP --user pi
Install OpenFaaS on ARMHF, ARM64 or a PC/VM

k3sup app install openfaas [--load-balancer] [--basic-auth]
