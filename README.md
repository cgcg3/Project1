# Project1
## Elk Stack Project 1
## Automated ELK Stack Deployment
##### The files in this repository were used to configure the network depicted below.
##### Note: The following image link needs to be updated. Replace diagram_filename.png with the name of your diagram image file.
##### These files have been tested and used to generate a live ELK deployment on Azure. They can be used to either recreate the entire deployment pictured above. Alternatively, select portions of the Red Team Network Diagram file may be used to install only certain pieces of it, such as Filebeat.
##### TODO: Enter the playbook file. 
##### This document contains the following details:
- Description of the Topology
- Access Policies
- ELK Configuration
###### - Beats in Use
###### - Machines Being Monitored
- How to Use the Ansible Build
### Description of the Topology
###### The main purpose of this network is to expose a load-balanced and monitored instance of DVWA, the D*mn Vulnerable Web Application.
###### Load balancing ensures that the application will be highly functional, in addition to restricting high traffic to the network.
TODO: What aspect of security do load balancers protect? What is the advantage of a jump box?
###### It keeps the servers from overloading, allowing prime optimization. 
Integrating an ELK server allows users to easily monitor the vulnerable VMs for changes to the network and system logs.
TODO: What does Filebeat watch for?
###### Filebeat works as bridge to monitor and send selected log files to ElasticSearch
TODO: What does Metricbeat record?
###### Metricbeat records the metric data desired and sends it to chosen location by ElasticSearch 
The configuration details of each machine may be found below. Note: Use the Markdown Table Generator to add/remove values from the table.
|  Name   | Funciton | IP Address| Operating System |
| --------|:--------:| ---------:| ----------------:|
| JumpBox | Gateway  | (Private) 10.1.0.4 (Public) 20.114.52.200 | Linux |
| Elk     | Server   | (Private) 10.3.0.4 (Public) 104.41.155.230| Linux |
| Web 1   | Server   | (Private) 10.1.0.5 | Linux |
| Web 2   | Server   | (Private) 10.1.0.6 | Linux |
| Web 3   | Server   | (Private) 10.1.0.7 | Linux |

#### Access Policies
The machines on the internal network are not exposed to the public Internet.
Only the jumpbox machine can accept connections from the Internet. Access to this machine is only allowed from the following IP addresses:
###### 162.226.175.112
Machines within the network can only be accessed by JumpBox.
TODO: Which machine did you allow to access your ELK VM? What was its IP address? JumpBox; 10.1.0.4
A summary of the access policies in place can be found in the table below.
|  Name   | Publicly Accessible | Allowed IP Addresses|
| --------|:-------------------:| -------------------:|
| Jumpbox | Yes                 | 162.226.175.112     |
| Elk     | Yes/No              | 10.1.0.6, 10.1.0.7  |
| Web 1   | No                  | 104.41.155.230      |
| Web 2   | No                  | 104.41.155.230      |
| Web 3   | No                  | 104.41.155.230      |


### Elk Configuration
Ansible was used to automate configuration of the ELK machine. No configuration was performed manually, which is advantageous because...
##### TODO: What is the main advantage of automating configuration with Ansible?
###### Ansible has tools (etc. Playbook) that allow you to automate tasks and configurations across multiple VMs.
##### The playbook implements the following tasks:
##### TODO: In 3-5 bullets, explain the steps of the ELK installation play. E.g., install Docker; download image; etc.
###### SSH into the JumpBox 
###### Start, then attach the desired container
###### “cd” into the correct directory “/etc/ansible/roles”, then create elk-playbook.yml
###### Run this playbook to start it, using command “ansible-playbook”
###### SSH into ELK VM to confirm success 
#### The following screenshot displays the result of running docker ps after successfully configuring the ELK instance.
#### Note: The following image link needs to be updated. Replace docker_ps_output.png with the name of your screenshot image file.
### Target Machines & Beats
##### This ELK server is configured to monitor the following machines:
###### 10.1.0.6	
###### 10.1.0.7
#### TODO: List the IP addresses of the machines you are monitoring
##### We have installed the following Beats on these machines:
###### Filebeat & Metricbeat
#### TODO: Specify which Beats you successfully installed
#### TODO: In 1-2 sentences, explain what kind of data each beat collects, and provide 1 example of what you expect to see. E.g., Winlogbeat collects Windows logs, which we use to track user logon events, etc.
###### Filebeat collects and transports the logs of data from the remote machines. Metricbeat collects the metrics from the machines.
## Using the Playbook
##### In order to use the playbook, you will need to have an Ansible control node already configured. Assuming you have such a control node provisioned:
##### SSH into the control node and follow the steps below:
###### Copy the filebeat-configuration.yml file to /etc/ansible/roles/files.
###### Update the metricbeat-configuration.yml file to include the ELK private IP 
###### Run the playbook, and navigate to http://104.41.155.230:5601 to check that the installation worked as expected.
##### TODO: Answer the following questions to fill in the blanks:
##### Which file is the playbook? Where do you copy it? filebeat-playbook.yml; /etc/ansible/roles
##### Which file do you update to make Ansible run the playbook on a specific machine? /etc/ansible/hosts
##### How do I specify which machine to install the ELK server on versus which to install Filebeat on? Create separate groups to specify. One named “webservers” the other named “elk”
##### _Which URL do you navigate to in order to check that the ELK server is running? http://104.41.155.230:5601/app/kibana

