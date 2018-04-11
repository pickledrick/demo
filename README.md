# Sausage Sandwich Service #


## Setup ##

### OSX ###

Ensure Homebew is installed, follow steps at:

[Homebrew](https://brew.sh)

Then:

`brew install kubectl`

`curl -o conf https://raw.githubusercontent.com/pickledrick/demo/master/config`

### Windows ###

Ensure Chocolatey is installed, follow steps at:

[Chocolatey](https://chocolatey.org/install)

Then:

`choco install -y kubernetes-cli curl`

`curl -o conf https://raw.githubusercontent.com/pickledrick/demo/master/config`

`brew install kubectl`

## Deploy ##

### standard ###

`kubectl --kubeconfig=conf -n <your-name> apply /
 -f https://raw.githubusercontent.com/pickledrick/demo/master/k8s/deploy-1.yaml`

### resilient ###

`kubectl --kubeconfig=conf -n <your-name> apply /
-f https://raw.githubusercontent.com/pickledrick/demo/master/k8s/deploy-2.yaml`

