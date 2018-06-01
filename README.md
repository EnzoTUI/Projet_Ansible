# Wildfly-server
Création d'un serveur wildfly  dans un conteneur LXC avec ansible

Pour créer un serveur wildfly, il faut suivre les étapes suivantes :


* Vérifier que le conteneur est accessible en ssh. Cette étape est obligatoire pour valider
  l'empreinte du serveur.
  
    ssh [IP du conteneur]

* Modifier l'inventaire Ansible. Pour cela, éditez le fichier inventory.ini et ajoutez l'adresse
  IP du conteneur dans le groupe ci-server

* Lancer le playbook Ansible à l'aide du script :

    ./01_run_playbook.sh

* Vous pouvez accéder au serveur wildfly à partir d'un navigateur Web à l'adresse :

    http://[ip conteneur]:8080
