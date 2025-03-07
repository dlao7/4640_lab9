# 4640-w9-lab-9-complete

Given script folder with import_lab_key:
1. Make lab key

```bash
ssh-keygen -t ed25519 -f ~/.ssh/<name> -C "lab9 key"
```

```bash
./scripts/import_lab_key ~/.ssh/<name>.pub
```

Given ansible folder with Ansible playbook named playbook.yml and needed files:

2. Packer

    In packer folder:

    1. Install plugins in ~/.config/packer/plugins.
    ```bash
    packer init .
    ```

    2. Build Packer image, loading all packer files (configuration and variables files).
    ```bash
    packer build .
    ```

3. Terraform

    In terraform folder:

    1. Install plugins.
    ```bash
    terraform init
    ```

    2. Create Terraform plan.
    ```bash
    terraform plan -out <plan-name>
    ```

    3. Apply Terraform plan.
    ```bash
    terraform <plan-name>
    ```
