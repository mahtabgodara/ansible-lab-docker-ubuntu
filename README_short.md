Install Docker for Mac

Download and install from: https://hub.docker.com/editions/community/docker-ce-desktop-mac 

OR 

https://guavusnetwork-my.sharepoint.com/:f:/r/personal/mahtab_singh_guavus_com/Documents/training-mat/ansible/Docker4Mac?csf=1&e=LF1buJ

mkdir -p ~/ansible/lab-setup/
cd ~/ansible/lab-setup/

git clone https://github.com/mahtabgodara/ansible-lab-docker-ubuntu.git

cd ansible-lab-docker-ubuntu

docker-compose up -d --build

docker exec -it master01 bash

ping -c 2 web1

ssh-agent bash

ssh-add master_key

As **passphrase** enter: `12345`

ansible-playbook -i inventory ping_all.yml

Type: `yes` (four times)



