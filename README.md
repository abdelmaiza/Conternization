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

Pour installer OpenShift en local sur un MacBookPro 16,2, vous pouvez utiliser l'outil minikube pour installer un cluster Kubernetes localement. Ensuite, vous pouvez installer OpenShift sur ce cluster en utilisant la commande oc cluster up. Voici les étapes à suivre:

Installez Homebrew en ouvrant une fenêtre de terminal et en tapant la commande suivante:
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/main/install.sh)"
```

Installez Docker en tapant la commande suivante:
```
brew install docker
```

Installez kubectl en tapant la commande suivante:
```
brew install kubectl
```

Installez minikube en tapant la commande suivante:
```
brew install minikube
```

Démarrez un cluster Kubernetes local avec minikube en tapant la commande suivante:
```
minikube start
```

Installez OpenShift CLI en tapant la commande suivante:
```
brew install openshift-cli
```

Pour installer OpenShift sur votre cluster Kubernetes local, utilisez la commande suivante :
```
oc cluster up --create-machine --image=registry.access.redhat.com/openshift4/ose-cli --version=4.6.1 
```

Connectez-vous à l'interface d'administration OpenShift en tapant la commande suivante :
```
oc login -u developer -p developer
```

Vous devriez maintenant être en mesure d'utiliser OpenShift en local sur votre MacBookPro 16,2.

Notez que cette installation en local peut être utilisée pour des fins de développement uniquement et que les ressources nécessaires pourraient être importantes. Il est donc conseillé de consulter la documentation officielle pour une utilisation en production.
