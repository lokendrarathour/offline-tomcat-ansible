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
        -centOS 7
Package Require on Base host:
-
	#1.Ansible
	#2.sshpass
Install Ansible on CentOS 7
--
	#sudo yum -y install epel-release && sudo yum -y install ansible
Install SSHPASS on CentOS 7
--
	#sudo yum -y install sshpass

####
Update Host file with your Host Details
-
-
vi hosts
-
	#[host-group]
	#142.44.243.51
	#
	#[local]
	#127.0.0.1


Run following command to execute the ansible Script: 
--
	ansible-playbook -b -vvv -u root configy.yaml -i hosts --ask-pass

