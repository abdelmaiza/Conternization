# Conternization
command
 - docker : show all options
 - docker pull : pull image from docker hub
 - docker images : list all images
 - docker rmi (ID Image) : remove image 
 - docker run (Image Name) : pull image if not exist and run container
 - docker ps -a : list all container stoped and running 
 - docker ps : list all running container
 - docker rm  (ID Container) : remove container


Install OpenShift : 
Pour installer OpenShift sur un MacBookPro 16,2 en utilisant la ligne de commande, vous devrez d'abord installer les outils nécessaires, comme Docker et Kubernetes. 

Vous pouvez utiliser Homebrew pour installer ces outils.

Installez Homebrew en ouvrant une fenêtre de terminal et en tapant la commande suivante:
 - /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/main/install.sh)"
 
Installez Docker en tapant la commande suivante:
 - brew install docker

Installez Kubernetes en tapant la commande suivante:
 - brew install kubectl
 
Installez minikube en tapant la commande suivante:
 - brew install minikube
 
Installez OpenShift en tapant la commande suivante:
 - brew install openshift-cli
 
Pour démarrer un cluster OpenShift localement, utilisez la commande suivante:
 - oc cluster up

Vous devriez maintenant être en mesure d'utiliser OpenShift sur votre MacBookPro 16,2 en utilisant la ligne de commande.
