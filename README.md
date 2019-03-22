# jenkins_role
### AWS
・OS：CENTOS 7
・INSTANCE TYPE：T2.MICRO
・ROOT DEVICE SIZE：12GB

This role is used to install jenkins on AWS. Before you run the playbook, please chenge the domain/ip of the jenkins under /jenkins/vars/main.yml Example: jenkins: domain
Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

# yum install epel-release -y
# yum install ansible -y
# cd /etc/ansible/roles
#  ansible-galaxy init jenkins
# ls jenkins (defaults  files  handlers  meta  README.md  tasks  templates  tests  vars)
# vim  /etc/ansible/roles/jenkins/tasks/main.yml
# ansible-playbook /etc/ansible/playbooks/jenkins_role.yml
