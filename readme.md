This role contains tasks to:

Install basic packages required
	Move required packages to hosts
	Install Tomcat
	configure Tomcat
	Start Tomcat
	
Prerequisite:
--
Operating System Tested on:
-
        -centOS
Package Require on Base host:
-
1.Ansible
2.sshpass
###### CentOS  ######
sudo yum -y install epel-release && sudo yum -y install ansible

--

Run following command to execute the ansible Script: 
--
ansible-playbook -b -vvv -u root configy.yaml -i hosts --ask-pass

