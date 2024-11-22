clear
    2  sudo apt-get update
    3  clear
    4  sudo apt-get install docker.io
    5  clear
    6  docker ps
    7  $USER
    8  printenv
    9  clear
   10  sudo usermod -aG docker $USER && newgrp docker
   11  clear
   12  [ $(uname -m) = x86_64 ] && curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.25.0/kind-linux-amd64
   13  clear
   14  ls
   15  ls -l
   16  chmod +x ./kind
   17  ls -l
   18  ls
   19  sudo mv ./kind /usr/local/bin/kind
   20  clear
   21  ls
   22  kind
   23  clear
   24  echo "$(cat kubectl.sha256)  kubectl" | sha256sum --check
   25  clear
   26  ls
   27  sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
   28  clear
   29  chmod +x kubectl
   30  mkdir -p ~/.local/bin
   31  mv ./kubectl ~/.local/bin/kubectl
   32  ls
   33  rm kubectl.sha256
   34  clear
   35  kubectl
   36  clear
   37  kind
   38  kubectl
   39  clear
   40  kind --version
   41  kubectl --version
   42  kubectl -version
   43  kubectl -v
   44  kubectl version
   45  clear
   46  kubectl version
   47  kind --version
   48  clear
   49  kind create cluster --name=my-cluster
   50  kind get clusters
   51  clear
   52  docker ps
   53  clear
   54  kubectl get nodes
   55  kind delete cluster --name=my-cluster
   56  clear
   57  ls
   58  mkdir k8s-practice
   59  cd k8s-practice/
   60  clear
   61  ls
   62  vim config.yml
   63  kind --version
   64  vim config.yml
   65  clear
   66  kind create cluster --name=my-cluster --config=config.yml
   67  clear
   68  kind get clusters
   69  clear
   70  kubectl get nodes
   71  clear
   72  kubect get nodes
   73  kubectl get nodes
   74  clear
   75  kubectl get pods
   76  kubect get namesapce
   77  kubectl get namesapce
   78  kubectl get namesapces
   79  kubectl get ns
   80  kubectl create ns dev
   81  kubectl get ns
   82  kubectl delete ns dev
   83  clear
   84  kubectl get pods
   85  kubectl run nginx --image=nginx
   86  kubectl get pods
   87  kubectl describe pod/nginx
   88  kubect delete cluster --name=my-cluster
   89  kind delete cluster --name=my-cluster
   90  clear
   91  kubectl set image nginx-deployment nginx-container=nginx:1.16.1 -n nginx
   92  kubectl set image deplyment/nginx-deployment nginx-container=nginx:1.16.1 -n nginx
   93  kubectl set image deployment/nginx-deployment nginx-container=nginx:1.16.1 -n nginx
   94  kubectl set image deployment/nginx-deployment nginx-container=nginx:1.14.1 -n nginx
   95  docker ps
   96  docker stop 5c78560ac0bc && docker rm 5c78560ac0bc
   97  docker ps
   98  clear
   99  docker ps
  100  docker stop 5a84b2e9a97e && docker rm 5a84b2e9a97e
  101  clear
  102  git clone https://github.com/LondheShubham153/django-notes-app.git
  103  clear
  104  ls
  105  cd django-notes-app/
  106  clear
  107  ls
  108  cd notesapp/
  109  ls
  110  vim settings.py
  111  cd ..
  112  git checkout dev
  113  clear
  114  vim notesapp/settings.py
  115  ls
  116  vim Dockerfile
  117  docker build -t notes-app .
  118  clear
  119  docker run -d -p 8000:8000 notes-app:latest
  120  docker login -u trainwithshubham
  121  clear
  122  docker image tag notes-app:latest trainwithshubham/notes-app:latest
  123  docker push trainwithshubham/notes-app:latest
  124  clear
  125  ls
  126  mkdir k8s
  127  cd k8s/
  128  ls
  129  vim deployment.yml
  130  vim namespace.yml
  131  cat deployment.yml
  132  clear
  133  vim service.yml
  134  kubectl apply -f .
  135  clear
  136  kubectl get all -n notes
  137  clear
  138  kubectl get all -n notes
  139  clear
  140  kubectl port-forward service/notes-app-service -n notes 8000:8000 --address=0.0.0.0
  141  docker ps
  142  docker stop b596f26cf9b8 && docker rm b596f26cf9b8
  143  clear
  144  kubectl port-forward service/notes-app-service -n notes 8000:8000 --address=0.0.0.0
  145  kubectl port-forward service/notes-app-service -n notes 8000:8000 --address=0.0.0.0 &
  146  clear
  147  history



docker ps 
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
   65  shutdown 
   66  sleep 
   67  poweroff 
   68  shutdown 
   69  shutdown ? 
   70  shutdown --help 
   71  shutdown -p 
   72  shutdown --p 
   73  shut down --p 
   74  shut down 
   75  exit 
   76  clear 
   77  sudo apt-get update 
   78  sudo apt-get upgrade 
   79  docker ps 
   80  clea 
   81  clear 
   82  sudo apt install docker.io -y 
   83  docker ps 
   84  sudo usermod -aG docker $USER && newgrp docker 
   85  exit 
   86  ls 
   87  kubectl get nodes 
   88  kubectl get ns 
   89  ls 
   90  mkdir nginx 
   91  cd nginx/ 
   92  vim namespace.yml 
   93  kubectl apply -f namespace.yml 
   94  kubectl delete -f namespace.yml 
   95  ls 
   96  vim pod.yml 
   97  kubectl apply -f pod.yml --dry-run=client 
   98  cat pod.yml 
   99  vim pod.yml 
  100  kubectl apply -f pod.yml --dry-run=client 
  101  vim pod.yml 
  102  kubectl apply -f pod.yml --dry-run=client 
  103  cat pod.yml 
  104  vim pod.yml 
  105  kubectl apply -f pod.yml --dry-run=client 
  106  vim pod.yml 
  107  kubectl apply -f pod.yml --dry-run=client 
  108  kubectl apply -f pod.yml 
  109  kubectl apply -f pod.yml --dry-run=client 
  110  kubectl apply -f pod.yml --dry-run=server 
  111  kubectl apply -f pod.yml --dry-run=client 
  112  clear 
  113  kubectl get -ns 
  114  kubectl get ns 
  115  kubectl get pod 
  116  vim pod.yml 
  117  kubectl apply -f pod.yml --dry-run=client 
  118  ls 
  119  cat pod.yml 
  120  clear 
  121  ls 
  122  cat pod.yml 
  123  kubectl apply -f pod.yml --dry-run=client 
  124  kubectl apply -f pod.yml 
  125  ls 
  126  cd nginx/ 
  127  ls 
  128  kubectl apply -f pod.yml 
  129  cat pod.yml 
  130  vim pod.yml 
  131  kubectl apply -f pod.yml 
  132  vim pod.yml 
  133  kubectl apply -f pod.yml 
  134  cat pod.yml 
  135  kubectl apply -f pod.yml --dry-run=client 
  136  kubectl apply -f pod.yml 
  137  clear 
  138  vim pod.yml 
  139  kubectl apply -f pod.yml 
  140  kubectl create namespace nginx 
  141  kubectl apply -f pod.yml 
  142  kubectl get pods 
  143  kubectl get pods -n nginx 
  144  vim Deployment.yml 
  145

145  kubectl get pods -n nginx 
  146  kubectl delete -f pod.yml 
  147  cat Deployment.yml 
  148  kubectl apply -f Deployment.yml --dry-run=client 
  149  vim Deployment.yml 
  150  kubectl apply -f Deployment.yml --dry-run=client 
  151  vim Deployment.yml 
  152  kubectl apply -f Deployment.yml --dry-run=client 
  153  kubectl apply -f Deployment.yml -n nginx 
  154  kubectl apply -f Deployment.yml 
  155  cat Deployment.yml 
  156  vim Deployment.yml 
  157  kubectl apply -f Deployment.yml 
  158  vim Deployment.yml 
  159  kubectl apply -f Deployment.yml 
  160  vim Deployment.yml 
  161  kubectl apply -f Deployment.yml 
  162  vim Deployment.yml 
  163  kubectl apply -f Deployment.yml 
  164  vim Deployment.yml 
  165  kubectl apply -f Deployment.yml 
  166  vim Deployment.yml 
  167  kubectl apply -f Deployment.yml 
  168  vim Deployment.yml 
  169  kubectl apply -f Deployment.yml 
  170  vim Deployment.yml 
  171  kubectl apply -f Deployment.yml 
  172  cat Deployment.yml 
  173  vim Deployment.yml 
  174  kubectl apply -f Deployment.yml 
  175  kubectl apply -f Deployment.yml -n nginx 
  176  kubectl apply -f Deployment.yml --dry-run=client 
  177  cat Deployment.yml 
  178  kubectl apply -f Deployment.yml --dry-run=client 
  179  vim Deployment.yml 
  180  kubectl apply -f Deployment.yml --dry-run=client 
  181  vim Deployment.yml 
  182  kubectl apply -f Deployment.yml --dry-run=client 
  183  kubectl apply -f Deployment.yml 
  184  vim Deployment.yml 
  185  kubectl apply -f Deployment.yml 
  186  vim Deployment.yml 
  187  kubectl apply -f Deployment.yml 
  188  vim Deployment.yml 
  189  kubectl apply -f Deployment.yml 
  190  vim Deployment.yml 
  191  kubectl apply -f Deployment.yml 
  192  vim Deployment.yml 
  193  kubectl apply -f Deployment.yml 
  194  vim Deployment.yml 
  195  kubectl apply -f Deployment.yml 
  196  cat Deployment.yml 
  197  vim Deployment.yml 
  198  kubectl apply -f Deployment.yml 
  199  vim Deploy.yml 
  200  kubectl apply -f Deploy.yml 
  201  kubectl apply -f Deployment.yml 
  202  ls 
  203  rm Deploy.yml 
  204  docker ps 
  205  kubectl get ns 
  206  sudo apt-get update] 
  207  sudo apt-get update 
  208  clear 
  209  sudo apt-get upgrade 
  210  tree 
  211  clear 
  212  ls 
  213  sudo apt-get install tree 
  214  tree 
  215  clear 
  216  docker ps 
  217  kubectl get nodes 
  218  ls 
  219  kubectl get nodes 
  220  cd nginx/ 
  221  ls 
  222  kubectl apply -f Deployment.yml 
  223  kubectl apply -f Deployment.yml --dry-run=client 
  224  cat Deployment.yml 
  225  kubectl get ns 
  226  clear 
  227  vim Deployment.yml 
  228  kubectl apply -f Deployment.yml --dry-run=client 
  229  cat Deployment.yml 
  230  vim Deployment.yml 
  231  kubectl apply -f Deployment.yml --dry-run=client 
  232  ls 
  233  rm Deployment.yml 
  234  ls 
  235  mkdir deployment.yml 
  236  ls 
  237  vim deployment.yml/ 
  238  vim deployment.yml 
  239  ls 
  240  rm deployment.yml/ 
  241  rm deployment.yml 
  242  ls 
  243  vim deployment.yml 
  244  kubectl apply -f deployment.yml --dry-run=client 
  245  kubectl apply -f deployment.ym 
  246  kubectl apply -f deployment.yml 
  247  clear 
  248  docker ps 
  249  kubectl get pods 
  250  kubectl get ms 
  251  kubectl get ns 
  252  kubectl get deployment -n nginx 
  253  kubectl get pods -n nginx 
  254  vim deployment.yml 
  255  kubectl apply -f deployment.yml 
  256  kubectl get pods -n nginx 
  257  vim deployment.yml 
  258  kubectl apply -f deployment.yml 
  259  kubectl get pods -n nginx 
  260  kubectl delete pod nginx nginx-deployment-5bb578c96b-vddxj -n nginx 
  261  kubectl delete pod 5bb578c96b-vddxj -n nginx 
  262  vim deployment.yml 
  263  kubectl delete pod nginx-deployment-5bb578c96b-sfqw6 -n 
  264  kubectl delete pod nginx-deployment-5bb578c96b-sfqw6 -n nginx 
  265  kubectl get pods -n nginx 
  266  clear 
  267  kubectl scale deployment.yml nginx-deployment -n nginx --replicas=5 
  268  kubectl scale deployment.yml deployment -n nginx --replicas=5 
  269  kubectl scale deployment.yml nginx-deployment -n

nginx --replicas=5 
  270  ls 
  271  kubectl get pods -n 
  272  kubectl get pod -n 
  273  vim deployment.yml 
  274  kubectl apply -f deployment.yml 
  275  kubectl scale deployment.yml nginx-deployment -n nginx --replicas=2 
  276  cat deployment.yml 
  277  clear 
  278  vim deployment.yml 
  279  vim pod.yml 
  280  kubectl apply -f pod.yml 
  281  kubectl apply -f deployment.yml 
  282  kubectl get deployment -n nginx 
  283  kubectl delete nginx-deployment -n nginx 
  284  kubectl delete deployment.yml -n nginx 
  285  kubectl delete deployment -n nginx 
  286  kubectl delete deployment nginx-deployment -n nginx 
  287  kubectl apply deployment.yml 
  288  kubectl apply -f deployment.yml 
  289  vim deployment.yml 
  290  kubectl apply -f deployment.yml 
  291  vim deployment.yml 
  292  kubectl apply -f deployment.yml 
  293  vim deployment.yml 
  294  kubectl apply -f deployment.yml 
  295  vim deployment.yml 
  296  kubectl apply -f deployment.yml 
  297  vim deployment.yml 
  298  kubectl apply -f deployment.yml 
  299  vim deployment.yml 
  300  kubectl apply -f deployment.yml 
  301  clear 
  302  kubectl delete -f pod.yml -f deployment.yml 
  303  kubectl apply -f deployment.yml 
  304  kubectl get pods -n nginx 
  305  kubectl describe pod nginx-deployment-565b9b7fdd-c2jwn -n nginx 
  306  kubectl set image deployment/nginx-deployment nginx-container=nginx:1.14.2 -n nginx 
  307  cat deployment.yml 
  308  kubectl set image deployment/nginx-deployment nginx-containers=nginx:1.14.2 -n nginx 
  309  kubectl set image deployment/nginx-deployment nginx=nginx:1.14.2 -n nginx 
  310  kubectl get pods 
  311  kubectl get pod 
  312  kubectl get pods -n nginx 
  313  clear 
  314  kubectl get pods -n nginx 
  315  kubectl exec --stdin --tty nginx-deployment-789c774d76-49qh6 -n nginx --/bin/bash 
  316  kubectl exec --stdin --tty nginx-deployment-789c774d76-49qh6 -n nginx -- /bin/bash 
  317  ls 
  318  vim service.yml 
  319  kubectl apply -f service.yml 
  320  vim service.yml 
  321  kubectl apply -f service.yml 
  322  vim service.yml 
  323  kubectl apply -f service.yml 
  324  vim service.yml 
  325  kubectl apply -f service.yml 
  326  kubectl get pods -n nginx 
  327  kubectl get service -n nginx 
  328  vim service.yml 
  329  kubectl apply -f service.yml 
  330  kubectl get svc -n nginx 
  331  docker ps 
  332  kubectl port-forward service/nginx-service -n nginx 80:80 --address=0.0.0.0 
  333  vim service.yml 
  334  kubectl port-forward service/nginx-service -n nginx 80:80 --address=0.0.0.0 
  335  kubectl port-forward service/nginx-service -n nginx 80:80 
  336  vim service.yml 
  337  sudo kubectl port-forward service/nginx-service -n nginx 80:80 
  338  sudo su 
  339  vim service.yml 
  340  sudo sysctl -w net.ipv4.ip_unprivileged_port_start=0 
  341  kubectl get svc -n nginx 
  342  sudo kubectl port-forward service/nginx-service -n nginx 80:80 
  343  cat service.yml 
  344  vim service.yml 
  345  kubectl port-forword service/nginx-service -n nginx 80:81 --address=0.0.0.0 
  346  kubectlport-forward service/nginx-service -n nginx 80:81 --address=0.0.0.0 
  347  kubectl port-forward service/nginx-service -n nginx 80:81 --address=0.0.0.0 
  348  vim service.yml 
  349  kubectl port-forward service/nginx-service -n nginx 80:81 --address=0.0.0.0 
  350  sudo kubectl port-forward service/nginx-service -n nginx 80:81 --address=0.0.0.0 
  351  kubectl cluster-info 
  352  sudo systemctl restart kube-apiserver 
  353  sudo kubectl port-forward service/nginx-service -n nginx 80:81 --address=0.0.0.0 & 
  354  kubectl port-forward service/nginx-service -n nginx 80:81 --address=0.0.0.0 & 
  355  clear 
  356  kubectl port-forward service/nginx-service -n nginx 80:81 --address=0.0.0.0 & 
  357  clear 
  358  cd .. 
  359  mkdir nodejs && cp -r nginx/*.* nodejs 
  360  ls 
  361  cd nodejs/ 
  362  ls 
  363  vim deployment.yml 
  364  vim namespace.yml 
  365  vim pod.yml 
  366  vim deployment.yml 
  367  vim pod.yml 
  368  vim service.yml 
  369  kubectl apply -f namespace.yml -f deployment.yml -f

service.yml 
  370  kubectl port-forword service/nodejs-service -n nodejs 8000:800 --address=0.0.0.0 
  371  kubectl port-forward service/nodejs-service -n nodejs 8000:800 --address=0.0.0.0 
  372  kubectl port-forward service/nodejs-service -n nodejs 8000:8000 --address=0.0.0.0 
  373  sudo netstat -tuln 
  374  sudo lsof -i :8080 
  375  sudo netstat -tuln 
  376  kubectl port-forward service/nodejs-service -n nodejs 8000:8000 --address=0.0.0.0 
  377  sudo systemctl restart networking 
  378  sudo netstat -tuln 
  379  clear 
  380  kubectl port-forward service/nodejs-service -n nodejs 8000:8000 --address=0.0.0.0 
  381  clear 
  382  kubectl get services -n nodejs 
  383  kubectl get pods -n nodejs -l app=nodejs 
  384  kubectl describe service nodejs-service -n nodejs 
  385  kubectl port-forward service/nodejs-service -n nodejs 8000:8000 --address=0.0.0.0 --v=9 
  386  sudo lsof -i :8000 
  387  sudo kill -9 <PID> 
  388  sudo kill -9 
  389  kubectl get pods -n nodejs 
  390  kubectl get pod 
  391  kubectl get pods 
  392  kubectl get pods -n 
  393  kubectl port-forward service/nodejs-service -n nodejs 8000:8000 
  394  sudo systemctl restart kubelet 
  395  sudo systemctl restart kubectl 
  396  kubectl port-forward service/nodejs-service -n nodejs 8000:8000 --address=0.0.0.0 
  397  ls 
  398  cat namespace.yml 
  399  kubectl get pods -n nodejs 
  400  clear 
  401  kubectl get namespace.yml 
  402  ls 
  403  vim namespace.yml 
  404  kubectl apply -f namespace.yml 
  405  kubectl apply -f deployment.yml -n nodejs 
  406  vim deployment.yml 
  407  kubectl apply -f deployment.yml -n nodejs 
  408  kubectl apply -f namespace.yml -n nodejs 
  409  kubectl apply -f service.yml -n nodejs 
  410  kubectl get all -n nodejs 
  411  kubectl get pods -n nodejs 
  412  kubectl port-forward service/nodejs-service -n nodejs 8000:8000 --address=0.0.0.0 
  413  history


Kind advance ----------------------------------------------------------------------------------------------------

Here’s a cleaned-up, duplicate-free list of commands extracted from your history: 
 
--- 
 
### Docker Commands 
1. docker ps 
2. docker kill 
3. sudo apt install docker.io -y 
4. sudo usermod -aG docker $USER && newgrp docker 
 
--- 
 
### KIND Commands 
5. curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.25.0/kind-linux-amd64 
6. chmod +x ./kind 
7. sudo mv ./kind /usr/local/bin/kind 
8. kind --version 
9. kind create cluster --name=my-cluster 
10. kind get clusters 
11. kind delete cluster --name=my-cluster 
12. kind create cluster --name=my-cluster --config=config.yml 
 
--- 
 
### Kubectl Commands 
13. kubectl version 
14. kubectl get nodes 
15. kubectl get ns 
16. kubectl create ns dev 
17. kubectl get pods 
18. kubectl run nginx --image=nginx 
19. kubectl describe pod/nginx 
20. kubectl apply -f namespace.yml 
21. kubectl delete -f namespace.yml 
22. kubectl apply -f pod.yml --dry-run=client 
23. kubectl apply -f pod.yml 
24. kubectl apply -f pod.yml --dry-run=server 
25. kubectl create namespace nginx 
26. kubectl get pods -n nginx 
27. kubectl apply -f Deployment.yml 
28. kubectl delete -f pod.yml 
29. kubectl apply -f Deployment.yml --dry-run=client 
30. kubectl scale deployment nginx-deployment -n nginx --replicas=5 
31. kubectl delete pod nginx-deployment-5bb578c96b-sfqw6 -n nginx 
 
--- 
 
### System Management 
32. sudo apt-get update 
33. sudo apt-get upgrade 
34. sudo apt-get install tree 
35. tree 
 
--- 
 
### File & Directory Management 
36. mkdir k8s-practice 
37. cd k8s-practice/ 
38. vim config.yml 
39. cat config.yml 
40. rm Deploy.yml 
41. mkdir nginx 
42. cd nginx/ 
43. vim namespace.yml 
44. vim pod.yml 
45. vim Deployment.yml 
46. cat Deployment.yml 
 
--- 
 
### Miscellaneous 
47. echo "$(cat kubectl.sha256)  kubectl" | sha256sum --check 
48. sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl 
49. ls 
50. clear 
