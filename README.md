# Spring Devenv
## Description 
Use `vagrant` + `ansible` to rapidly set a spring-boot development VM (based on Ubuntu 16.04). 
## Usage
1. clone the project with submodule option: `git clone --recurse-submodules https://github.com/ryanhhtan/spring-devenv.git`.
2. put the required credential files to the submodule. 
- .vault_pass (password to decrypt vault)
- keys directory (contains id_rsa, id_rsa.pub, github gpg kye, etc)
3. spin up the VM `vagrant up`
4. login the VM by `vagrant ssh`, then `cd /vagrant/ansible_module/` and run `ansible-playbook playbook-primary.yml -i inventory`
5. exit and re-login with `vagrant ssh` or `ssh vagrant@<ip_address_of_the_VM>`  
