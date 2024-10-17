# percona-mysql-ha

### steps to deploy

1 create playbook 

example in examples/playbook.yml

2 create inventory

example in examples/hosts

3 create vars

example in examples/vars.yml, examples/host_vars.yml

4 deploy

```sh
ansible-playbook mysql-cluster.yml -i inventories/lt/hosts --vault-password-file ../vault_pass  -vvv  -u user
```

5 change bootstrap var value

```
bootstrap: false
```
