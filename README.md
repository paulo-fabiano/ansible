# Projeto Ansible

Este projeto é uma estrutura inicial para orquestração com Ansible.

## Estrutura

- `ansible.cfg`: configuração do Ansible
- `inventory/hosts.ini`: inventário de hosts
- `group_vars/all.yml`: variáveis globais
- `playbooks/site.yml`: playbook principal
- `playbooks/services.yml`: playbook para apenas os serviços
- `roles/common`: tarefas básicas de configuração
- `roles/webserver`: provisiona NGINX
- `roles/database`: provisiona PostgreSQL

## Uso

Executar o playbook principal:

```bash
ansible-playbook playbooks/site.yml
```

Executar somente os serviços:

```bash
ansible-playbook playbooks/services.yml
```
