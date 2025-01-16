Steps:

1- Créer une pair de clé --> 1000techLeader.pem
Je télécharge et modfie les droits
sudo chmod 400 1000techLeader.pem

2- Créer une instance EC2 utilisant cette paire de clé

3- Se connecter sur le serveur
ssh -i CHEMIN_VERS/1000techLeader.pem utilisateur@IP_PUBLIC

4- Construire notre inventaire 

5- testez notre inventaire 
ansible -i inventaire.ini all -m ping
ansible -i inventaire.ini serveur1 -m ping
6- Ecrire nos premiers playbooks

7 - Jouer le playbook
ansible-playbook -i ../inventaire.ini cp.yml 
ansible-playbook -i ../inventaire.ini -e host=serveur1  cp.yml