# CKA Docker 1.12.6

Ansible 二进制部署 Docker

├── defaults
│   └── main.yml
├── files
│   ├── docker
│   ├── docker-containerd
│   ├── docker-containerd-ctr
│   ├── docker-containerd-shim
│   ├── docker-proxy
│   ├── docker-runc
│   └── dockerd
├── handlers
│   └── main.yaml
├── meta
│   └── main.yaml
├── tasks
│   └── main.yaml
├── templates
│   └── docker.j2
├── tests
│   ├── cluster.yaml
│   ├── inventory
│   ├── roles
│   │   └── docker -> ../../
│   └── test.yaml
└── vars
    └── main.yml

## 部署方式

cd tests
ansible-playbook -i inventory cluster.yaml
 
