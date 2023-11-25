Ansible for setup insight production environment

Step bootstrap
1. bootstrap create user for ansible and remove root login

Step provision
1. create user for deployment
2. setup essential software
3. setup deployment
4. setup nginx
5. bla bla bla


How To Use
Production
1. Run `ansible-playbook setup.yml` this will setup server (user) for the first time. This will run to all hosts
2. Setup production run `ansible-playbook playbook.yml`

Group vars for password are encrypted by ansible-vault

created password with
`python3 -c 'import crypt;print(crypt.crypt("mypassword"))'`