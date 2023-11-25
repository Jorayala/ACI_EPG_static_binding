# ACI_EPG_static_binding

### Create a virtual environment

```
python3 -m venv ANSIBLE_ACI
source ANSIBLE_ACI/bin/activate
cd ANSIBLE_ACI/
```

### Installing Ansible For Ubuntu/Debian

```
sudo apt update
sudo apt install software-properties-common
sudo apt-add-repository --yes --update ppa:ansible/ansible
sudo apt install ansible
```

### Clone the repo

```
git clone https://github.com/thetechguy-it/ACI_EPG_static_binding.git
```

### Run the playbook

After changing the "credentials.yml" and "epgs_csv" files, you can run the playbook. I recommend you to test it in the Cisco Sabdbox before pushing in the production:

```
ansible-playbook epg_bind.yml
```
