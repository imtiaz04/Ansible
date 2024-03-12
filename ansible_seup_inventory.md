Ansible is a configuration management tool
It works as master and worker architecture model wher master containes inventory and run the activities on the worker nodes with ssh.
Ansible playbooks is written in YAML files
Ansible used "push based configuration "mode which differs from cheff and puuet which works as "pull based configuration" model where we need agents that extra effort need where as in ansible only Master server/inventory need to be installed ansible
Taging is powerfull concept in ansible to group & manage tasks easyly.
 can Organize inventories with environment based like production# inventory file for production servers, staging server files, testing server files....
 first on mater server need to create repository with below command
 
 ![image](https://github.com/imtiaz04/Ansible/assets/85178565/df1a249c-dec4-4204-9f24-d65335c2d922)

 
then update and install ansible

![image](https://github.com/imtiaz04/Ansible/assets/85178565/e5c361a2-d8a9-4543-adce-08683ad52cfe)

![image](https://github.com/imtiaz04/Ansible/assets/85178565/2543c074-7f41-41e6-b3d9-feb58cbb00a6)

![image](https://github.com/imtiaz04/Ansible/assets/85178565/a69c596c-026a-415b-baee-82d2ffc24a5b)

open editor nano and add server list 

![image](https://github.com/imtiaz04/Ansible/assets/85178565/361f76eb-2c1d-4614-952c-6aea40ff073b)

After that need to copy the pem file from local to ec2 master server using 'scp' command

![image](https://github.com/imtiaz04/Ansible/assets/85178565/5575c890-8500-4e49-9209-96e5b6769da2)

can verify once transfer the pem file it wil access all the worker nodes

![image](https://github.com/imtiaz04/Ansible/assets/85178565/7839ded8-99ca-46ca-9fe7-f5543ad9a86b)

need to add in inventory file variables with [servers:vars] so that using pem file private key worker nodes can connect

![image](https://github.com/imtiaz04/Ansible/assets/85178565/393ba566-cb1c-461d-a0dc-7ef7bdc98f09)


we can check the disc spaces on worker nodes

![image](https://github.com/imtiaz04/Ansible/assets/85178565/5deefaee-946a-4059-b719-3a6670155169)

can update all servers all @once

![image](https://github.com/imtiaz04/Ansible/assets/85178565/4101a2e1-4e93-483f-8c68-417948574a81)











