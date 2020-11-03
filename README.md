# EXIAA3-SysAdmin-AnimusExtendus

Ce repo fait partie du projet Animus Extendus. Il contient les Playbooks et les Dockerfiles nécessaires au déploiement du Site Vitrine et de l’Intranet d’Animus sur un Serveur Linux avec des conteneurs Docker..


## Prérequis

* Préparer le Serveur de Déploiement Linux (testé avec Debian).
* Installer Ansible sur un autre Serveur Linux (testé avec Debian).


## Installation et Utilisation du Playbook

* Sur le Serveur Ansible se placer dans le dossier d'Ansible (```cd /etc/ansible```).
* Ajouter le Serveur de Déploiment dans le fichier hosts présent dans ce dossier.
* Cloner ce repo dans le dossier (```git clone https://github.com/Caldei/EXIAA3-SysAdmin-Animus.git```).
* Lancer le Playbook (```ansible-playbook EXIAA3-SysAdmin-Animus/Ansible/web.yml```).
* Enjoy :)


## Infos complémentaires

* Site Vitrine : Apache - Port 80
* Site Intranet : Nginx - Port 8080
