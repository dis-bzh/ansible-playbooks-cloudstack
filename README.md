
## Install Ansible

## Prepare python venv

```bash
sudo mkdir -p /opt/dev/venv

sudo chown -R $USERNAME:$USERNAME /opt/dev

python3 -m venv /opt/dev/venv/ansible
```
Maybe you should install python venv module first depending on your distribution

## Use venv

```bash
source /opt/dev/venv/ansible/bin/activate
```

## Upgrade pip and install Ansible

```bash
pip install --upgrade pip

pip install ansible~=12.2
```

## Install Ansible dependencies

```bash
ansible-galaxy install -r requirements.yml
```
ou GIT_SSH_COMMAND="ssh -i ~/.ssh/id_ed25519" ansible-galaxy install -r requirements.yml pour utiliser une clé SSH spécifique