# Sausage Sandwich Service #


## Setup ##

### OSX ###

Ensure Homebew is installed, follow steps at:

`https://brew.sh`

`brew install kubectl`

`curl -o conf https://raw.githubusercontent.com/pickledrick/demo/master/config`

### Windows ###

Ensure Chocolatey is installed, follow steps at:

`https://chocolatey.org/install`

`choco install -y kubernetes-cli curl`

`curl -o conf https://raw.githubusercontent.com/pickledrick/demo/master/config`

`brew install kubectl`

## Standard ##

### Deploy ###

`kubectl -n <your-name> apply -f https://raw.githubusercontent.com/pickledrick/demo/master/k8s/deploy-1.yaml`

## Resilient ##

### Deploy ###

`kubectl -n <your-name> apply -f https://raw.githubusercontent.com/pickledrick/demo/master/k8s/deploy-2.yaml`

