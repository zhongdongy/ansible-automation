# Ansible Automation Scripts

## Before Use
Please make sure you have inventories prepared before use. Let's say your inventory is kept inside `~/.ansible/inventory/all.yaml`, then type the following command to run `playbook-name` playbook:

```bash
ansible-playbook -i ~/.ansible/inventory/all.yaml playbook-name.yaml
```

**Note**: if you are using bare SSH username/password to access inventory hosts, please make sure `sshpass` program is installed. This is not provided by default, so you need to manually install it. For example, on macOS, you can use:

```bash
brew install hudochenkov/sshpass/sshpass
```

## Table of Scripts

Script Name | Server Names | Note
:--|:--|:--
blog-deploy.yaml | blog_server | Pull content from repository (*) and use git to deploy

*: The repo is set to https://gitee.com/zhongdongy/zhongdongy.git, which is my blog site.
