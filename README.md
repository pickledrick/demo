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

[Chocolatey](https://chocolatey.org/install#installing-chocolatey)

Then:

`choco install -y kubernetes-cli curl`

`curl -o conf https://raw.githubusercontent.com/pickledrick/demo/master/config`


## Demo ##

### create namespace ###

`kubectl create ns <your-name>`

### basic ###

#### deploy ####

`kubectl --kubeconfig=conf -n <your-name> apply -f https://raw.githubusercontent.com/pickledrick/demo/master/k8s/deploy.yaml`

### run ###

`k -n <your-name> scale deploy sss --replicas=1`

#### visualize ####

[Grafana](http://ab06a209f3e5e11e8bf9b0217645aafb-463719993.eu-west-1.elb.amazonaws.com)

`admin:admin`

### resilient ###

#### deploy ####

`kubectl --kubeconfig=conf -n <your-name> apply -f https://raw.githubusercontent.com/pickledrick/demo/master/k8s/deploy-resil.yaml`

#### visualize ####

[Grafana](http://ab06a209f3e5e11e8bf9b0217645aafb-463719993.eu-west-1.elb.amazonaws.com)
`admin:admin`