# Ansible-Automation-Infrastructure

System engineers, System Admin, DevOps engineers use automation to:

- Maintain consistency across servers

- Enforce configuration standards

- Deploy applications or services

- Perform repetitive tasks without human error

  # Ansible Dev Automation

This project sets up a full Ansible Development environment using Vmware and Rocky Linux 8. It covers:

- Ansible control node + 3 worker nodes
- SSH key authentication setup
- Real-world automation tasks using Ansible

## 🖥️ Infrastructure

| Hostname       | Role          | IP Address      |
|----------------|---------------|------------------|
| ansible-master | Control Node  | 192.168.56.10 |
| worker1        | Managed Node  | 192.168.56.11 |
| worker2        | Managed Node  | 192.168.56.12 |
| worker3        | Managed Node  | 192.168.56.13 |

## 📂 Playbooks

- `users.yml`: Add users
- `firewall.yml`: Configure firewalld
- `motd.yml`: Customize login banner
- `cronjobs.yml`: Setup system update cron job

## ⚙️ Run Playbooks

``ansible-playbook -i inventory/hosts.ini playbooks/users.yml``

**All systems should be** 
- Rocky Linux 8 Minimal
- user: ansible
- SSH enabled
