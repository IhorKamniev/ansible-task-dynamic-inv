# ansible-task-dynamic-inv
Using dynamic inventory based on tags instead of hosts file

Preconditions:
    
    1. Provision instances with tag "name" and value "uat"

Setup:

    1. Move "inventory" directory and "ansible.cfg" file to /etc/ansible
    2. Specify AWS credentials in aws_ec2.yaml
    3. Specify path to private key in "group_vars/tag_name_uat
    4. Run command:
    $ ansible-playbook dynamic_inv_playbook.yml
