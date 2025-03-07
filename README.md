# 4640-w9-lab-9-complete

Given script folder with import_lab_key:
1) Make lab key

```bash
ssh-keygen -t ed25519 -f ~/.ssh/<name> -C "lab9 key"
```

```bash
./scripts/import_lab_key ~/.ssh/<name>.pub
```

Given ansible folder with Ansible playbook named playbook.yml and needed files:

2) Packer

* packer init . in packer folder to install plugins.
* packer build .

3) Terraform

* terraform init in terraform folder to install plugins.
* terraform plan -out <plan-name>
* terraform <plan-name>
