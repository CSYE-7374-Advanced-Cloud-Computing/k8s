# k8s

Branch -- Assignment3

Team Details:

1) Hemal Gadhiya -- 001460577
2) Paavan Gopala -- 001813403

Details regarding Ansible Playbooks for create and delete Kubernetes Cluster:

a) To create the kubernetes cluster, we make use of Anisble Playbook to achieve the tasks:
Run the command: --> ansible-playbook setup-k8s-cluster.yaml -i dev -vvvv

b) To delete the kubernetes cluster, we make use of Ansible Playbook to achieve the tasks:
Run the command: ansible-playbook delete-k8s-cluster.yaml -i dev -vvvv --extra-vars '{"cluster_name":"k8s.dev.paavangopala.me", "state_store":"s3://k8s-dev-paavangopala-state-store"}'

c) To get all nodes and master nodes, run the following command:
   --> kubectl get nodes

d) To validate the cluster, run the following command:
   --> kops validate cluster --name=k8s.dev.paavangopala.me --state=s3://k8s-dev-paavangopala-state-store
