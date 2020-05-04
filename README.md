# ELK_Ansible_Playbook
A Vagrant file to spin up 3 instances of Ubuntu (based of GeerlingGuy's Ubuntu box), and then an Ansible playbook to install and configure ElasticSearch on one, Kibana on one and Logstash on one.

v1 - playbook.yml
A playbook that installs the ELK stack across 3 computers and places FileBeat onto the computer running Logstash. See: https://geektechstuff.com/2020/05/01/creating-an-elk-stack-via-an-ansible-playbook-v1/ for further details.
