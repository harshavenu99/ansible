# ansible


Pre-requisites

Ansible Vault ENV variable needs to be set on the ansible-controller so that when the cert.key is commited to the CI server, it's encrypted. Hence the usage of "decrypt: yes" in the task module

To execute the play book for masters

ansible-playbook -i inventory.yml playbook.myl --tags masters


To execute the play book for workers

ansible-playbook -i inventory.yml playbook.myl --tags workers
