<h1 align="center">🛠️</br>Animus</h1>
<p align="center">
  EXIA Year 3 - Automation (Ansible, Dockerfile) - 4 Person Group Project - 2020
</p>


---
## Overview
### Project goal 
Automate the configuration of Debian-based Linux servers. Several servers needed to be configured for Snmp and to run Docker with two web servers on containers (one with Apache listening on port 80 and the other with Tomcat listening on port 8080).

### Repo Content
* **Snmp:** Ansible Playbook to install and configure SNMP.
* **Webservers:** Ansible Playbook and Dockerfiles to install and configure Docker and the two containers with webservers (`Apache port 80`and `Tomcat port 8080`).


---
## Get Started
1. Add `[SNMP]`, `[WEB]` and the corresponding `Debian-based` hosts you want to configure in `/etc/ansible/hosts` on your Ansible server.
2. If you have git, you can clone the repo with this command (or you can directly download it as Zip):
    ```sh
    git clone https://github.com/Caldei/EXIA-Automation-Animus.git
    ```
3. Launch the Snmp playbook:
    ```sh
    ansible-playbook ./EXIA-Automation-Animus/Snmp/snmp_playbook.yml
    ```
4. Launch the Webservers playbook:
    ```sh
    ansible-playbook ./EXIA-Automation-Animus/Webservers/webservers_playbook.yml
    ```
5. Visit the websites and use Snmp!

---
## Snmp Playbook Visual
<p align="center">
  <img src=https://i.ibb.co/rQ4W9Wz/Webservers-Playbook-Visual.png alt="Snmp Playbook Visual" width="600">
</p>

