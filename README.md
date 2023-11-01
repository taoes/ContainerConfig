# k8s-config
link
command: 
- kubeadm init --apiserver-advertise-address $(hostname -i) --pod-network-cidr 10.5.0.0/16
- kubectl apply -f https://raw.githubusercontent.com/cloudnativelabs/kube-router/master/daemonset/kubeadm-kuberouter.yaml

kubeadm join 192.168.0.18:6443 --token wz6xfv.9a8ie2kzrp95d24z --discovery-token-ca-cert-hash sha256:9b4866132e21db78b7a3ccc46c2e0e42e09d6ee85e74ccef89bbd18ab0a82961