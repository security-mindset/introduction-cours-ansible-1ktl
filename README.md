# Installation Ansible

# Créer une clé ssh
ssh-keygen -t rsa -b 4096 -C "contact@security-mindset.fr"

#Copier votre clé sur le serveur 
echo "VOTRE_CLE" >> ~/.ssh/authorized_keys

# Pour les instances EC2 avec keypair
sudo chmod 400 1000techLeader.pem

ssh -i 1000techLeader.pem ubuntu@34.229.78.91
# Inventaires


# 