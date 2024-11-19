 1  docker ps
    2  # For AMD64 / x86_64
    3  [ $(uname -m) = x86_64 ] && curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.25.0/kind-linux-amd64
    4  # For ARM64
    5  ls
    6  ls -l
    7  chmod +x ./kind
    8  ls -;
    9  ls -l
   10  sudo mv ./kind /usr/local/bin/kind
   11  kind
   12  clear
   13  echo "$(cat kubectl.sha256)  kubectl" | sha256sum --check
   14  ls
   15  sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
   16  chmod +x kubectl
   17  mkdir -p ~/.local/bin
   18  mv ./kubectl ~/.local/bin/kubectl
   19  ls
   20  rm kubectl.sha256
   21  ls
   22  kubectl
   23  clear
   24  kind --version
   25  kubectl version
   26  kind create cludter --name=my-cluster
   27  kind create cluter --name=my-cluster
   28  clear
   29  kind create cluster --name=my-cluster
   30  kind get cluster
   31  kind get clusters
   32  docker ps
   33  kind delete cluster --name=my-cluster
   34  mkdir k8s-practice
   35  cd k8s-practice/
   36  vim config.yml
   37  kind create cluster --name=my-cluster --config=config.yml
   38  vim config.yml
   39  kind create cluster --name=my-cluster --config=config.yml
   40  sed -i 's/\t/  /g' config.yml
   41  kind create cluster --name=my-cluster --config=config.yml
   42  vim config.yml
   43  kind create cluster --name=my-cluster --config=config.yml
   44  cat config.yml
   45  vim config.yml
   46  kind create cluster --name=my-cluster --config=config.yml
   47  clear
   48  cat config.yml
   49  vim config.yml
   50  kind create cluster --name=my-cluster --config=config.yml
   51  cat config.yml
   52  kind get cluster
   53  kind get clusters
   54  kubectl get nodes
   55  kubectl get pods
   56  kubectl get ns
   57  kubectl create ns dev
   58  kubectl get ns
   59  kubectl get pods
   60  kubectl run nginx --image=nginx
   61  kubectl get pods
   62  kubectl describe pod/nginx
   63  kind delete cluster --name=my-cluster
   64  history