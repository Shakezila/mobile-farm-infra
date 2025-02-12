# Mobile Farm Infrastructure

This repository contains scripts and configurations for deploying a mobile farm using Appium, Selenium Grid, STF, and Ansible.

## Repository Structure

```
mobile-farm-infra/  
│── ansible/               # Ansible Playbooks  
│   ├── setup_env.yml      # Environment setup  
│   ├── install_stf.yml    # STF installation  
│   ├── install_grid.yml   # Selenium Grid installation  
│── vagrant/               # Vagrant configurations  
│   ├── Vagrantfile        # VM configuration  
│── docker/                # Docker files  
│   ├── hub/               # Image for Selenium Grid Hub  
│   ├── node/              # Image for Appium Node  
│── scripts/               # Useful scripts  
│   ├── check_devices.sh   # Check connected devices  
│── .github/               # CI/CD files for GitHub Actions  
│   ├── workflows/         # Deployment automation  
│── README.md              # Documentation  
```

## Installation and Setup

### 1. Deploy the Virtual Machine
```bash
cd vagrant
vagrant up
```

### 2. Set Up the Environment with Ansible
```bash
cd ansible
ansible-playbook -i inventory setup_env.yml
```

### 3. Check Connected Devices
```bash
cd scripts
./check_devices.sh
```

## Contacts
If you have any questions or suggestions, create an issue in the repository!

