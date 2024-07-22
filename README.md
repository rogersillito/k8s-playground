# k8s-playground

Local experiments with Kubernetes

## Setup

1. [Enable kubernetes in docker-desktop]([url](https://docs.docker.com/desktop/kubernetes/#install-and-turn-on-kubernetes))
2. Check running via `kubectl cluster-info`
![image](https://github.com/user-attachments/assets/c10d5156-9711-43b7-9357-223ca600482a)
3. Install `ingress-nginx` as per:
   - https://kubernetes.github.io/ingress-nginx/deploy/#docker-desktop
   - https://kubernetes.github.io/ingress-nginx/deploy/#quick-start
     ![image](https://github.com/user-attachments/assets/cbe9b1b6-711c-4666-80a2-6a15ea5fc225)
5. Apply manifests, e.g.  
   `cd manifests`  
   `kubectl apply -f network-multitool.yaml`
