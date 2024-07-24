# k8s-playground

Local experiments with Kubernetes

## Setup

1. [Enable kubernetes in docker-desktop]([url](https://docs.docker.com/desktop/kubernetes/#install-and-turn-on-kubernetes))
2. Get kubectl (& add to your cli path): https://kubernetes.io/docs/tasks/tools/#kubectl
3. Check running via `kubectl cluster-info`  
   (`%USERPROFILE%\.kube\config` should have been set up for you)
![image](https://github.com/user-attachments/assets/c10d5156-9711-43b7-9357-223ca600482a)
4. Install `ingress-nginx` as per:
   - https://kubernetes.github.io/ingress-nginx/deploy/#docker-desktop
   - https://kubernetes.github.io/ingress-nginx/deploy/#quick-start
     ![image](https://github.com/user-attachments/assets/cbe9b1b6-711c-4666-80a2-6a15ea5fc225)
5. Apply manifests, e.g.  
   `cd manifests`  
   `kubectl apply -f network-multitool.yaml`
6. Update `c:\Windows\System32\Drivers\etc\hosts` add line:  
   `127.0.0.1 k8s-playground.local`

