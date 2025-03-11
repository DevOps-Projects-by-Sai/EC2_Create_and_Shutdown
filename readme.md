Ansible Realtime project

Task 1
Create three(3) EC2 instances on AWS using Ansible loops

2 Instances with Ubuntu Distribution
1 Instance with Centos Distribution
Hint: Use connection: local on Ansible Control node.

Task 2
Set up passwordless authentication between Ansible control node and newly created instances.

Task 3
Automate the shutdown of Ubuntu Instances only using Ansible Conditionals

Hint: Use when condition on ansible gather_facts

-----------------------------------------------------------------------------------------


Pre-Requistes:

Task1-

1. sudo apt update
2. Install boto3 (pip install boto3), if it fails install python3
3. Install Ansible and Ansible Collections for AWS
4. Setup Vault file and password
5. Write the first_playbook.yaml and run it using "ansible-galaxy first_playbook.yaml --vault-password-file vault.pass"

Task2-

1. You should download the pem file "windows-demo"
ssh-copy-id -f "-o IdentityFile windows-demo" ubuntu@<INSTANCE-PUBLIC-IP>
