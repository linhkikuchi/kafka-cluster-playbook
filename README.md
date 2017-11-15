# KAFKA PLAYBOOK

This is a playbook to set up an apache kafka cluster in STG/PRD

TO RUN THE PLAYBOOK

```
ansible-playbook kafka.yml -i kafka.hosts -u root --extra-vars "server=stage keystore_pass=password"
ansible-playbook kafka.yml -i kafka.hosts -u root --extra-vars "server=prod keystore_pass=password"
```
extra-vars
- server=stage, to play only stage servers
- server=kafka, to play all servers
- server=server1, to play only prod server1