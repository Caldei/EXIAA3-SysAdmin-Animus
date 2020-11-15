# EXIAA3-SysAdmin-AnimusExtendus

Ce repo fait partie du projet Animus Extendus. Il contient :
1. Les Playbooks Ansible et les Dockerfiles nécessaires au déploiement du Site Vitrine et de l’Intranet d’Animus sur un Serveur Linux avec des conteneurs Docker.
2. Les Playbooks Ansible nécessaires au à l'installation de SNMP sur des Serveurs Linux (Debian).



# 1. WEB : Déploiement du Site Vitrine et de l’Intranet

## 1.1 Prérequis
* Préparer le Serveur de Déploiement Linux (testé avec Debian).
* Installer Ansible sur un autre Serveur Linux (testé avec Debian).

## 1.2 Installation et Utilisation des Playbook
* Sur le Serveur Ansible se placer dans le dossier d'Ansible (```cd /etc/ansible```).
* Ajouter ```[WEB]``` suivit de l'IP du Serveur de Déploiment dans le fichier ```hosts``` présent dans ce dossier.
* Cloner ce repo dans le dossier (```git clone https://github.com/Caldei/EXIAA3-SysAdmin-Animus.git```).
* Lancer le Playbook (```ansible-playbook EXIAA3-SysAdmin-Animus/WEB/Ansible/web.yml```).
* Enjoy :)


## 1.3 Infos complémentaires
* Site Vitrine : Apache - Port 80
* Site Intranet : Nginx - Port 8080


# 2. SNMP : Installation et configuration de SNMP

## 1.1 Prérequis
* Préparer les Serveurs Linux (Debian) où doit être installé SNMP.
* Installer Ansible sur un autre Serveur Linux (testé avec Debian).

## 1.2 Installation et Utilisation des Playbook
* Sur le Serveur Ansible se placer dans le dossier d'Ansible (```cd /etc/ansible```).
* Ajouter ```[SNMP]``` suivit de l'IP des les Serveurs Linux où doit être installé SNMP dans le fichier ```hosts``` présent dans ce dossier.
* Cloner ce repo dans le dossier (```git clone https://github.com/Caldei/EXIAA3-SysAdmin-Animus.git```).
* Lancer le Playbook (```ansible-playbook EXIAA3-SysAdmin-Animus/SNMP/Ansible/snmp.yml```).
* Enjoy :)
