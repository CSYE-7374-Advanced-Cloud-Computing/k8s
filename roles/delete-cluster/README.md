Branch -- Assignment3

Team Details:

Hemal Gadhiya -- 001460577
Paavan Gopala -- 001813403
Details regarding Ansible Playbooks for deleting Kubernetes Cluster:

a) To delete the kubernetes cluster, we make use of Ansible Playbook to achieve the tasks: Run the command: ansible-playbook delete-k8s-cluster.yaml -i dev -vvvv --extra-vars '{"cluster_name":"k8s.dev.paavangopala.me", "state_store":"s3://k8s-dev-paavangopala-state-store"}'
