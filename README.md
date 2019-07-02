this project Contain a docker container with ansible and the modules created

-> execute the follow commands on a server with docker and docker-compose
#git clone https://github.com/mprebello/docker-ansible-modules docker-ansible-modules
#cd docker-ansible-modules/code
#docker-compose build
#docker-compose up -d

PS: all the configuration will remain in /var/data/ansible_ssh/conf

access the server on port 2222 by ssh, user:admin password:admin, need to change the password on the first login
#ssh admin@myipaddress:2222

became root
#sudo -i

change inventory and credentials on /etc/ansible/hosts and /etc/ansible/group_vars

execute a playbook example:
  -> #ansible-playbook /etc/ansible/roles/CommonTasks/job/job-example.yml
