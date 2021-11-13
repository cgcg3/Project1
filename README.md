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
[Diagram](https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1#R7V1tc6M4Ev41rrr9YEqI94%2BJk8zszcxedjK1u%2FcphW3ZZoORD%2FDEmV9%2FEkg2SMLGNthkB1clNg0IUD%2F9qNVqiYExWm4%2BxP5q8QVPUTiAYLoZGHcDCC3DJf%2Bp4C0XOKaVC%2BZxMM1F%2Bk7wFPxATAiYdB1MUVI6MMU4TINVWTjBUYQmaUnmxzF%2BLR82w2H5qit%2FjiTB08QPZemfwTRd5FIXOjv5RxTMF%2FzKuu3le5Y%2BP5g9SbLwp%2Fi1IDLuB8YoxjjNfy03IxTSuuP1kp%2F3ULF3e2MxitI6J3yyvK9rcPPb738Fv341kvT%2Bk%2F1hyEr57odr9sDsZtM3XgPBMqui20W6DIlEJz%2BZ6C5Yzsn1wmBM%2Fk%2FCYPXsxyn5GaH0FccvQUT3jkK8nj6P8HK1TlH8rEN3Q%2F60Fd0pPgC%2FGxSnaFMQsQf6gPASpfEbOYTttR1WuQxdBtt83alK5%2FW%2FKKrJYkKfwWO%2BLXpXg%2BQHq0R1habw5ttq8%2Fz12%2BgWGLPfbP3295ehJ9UfmhJAsU0cpws8x5Ef3u%2BktzFeR1NESwVka3fMZ4xXrMb%2FRmn6xqzDX6e4rI%2F8mvRCldhgogSv4wnaAwim%2F9SP5yjdc5yj1kuMQj8Nvpfv45xK3neT%2B1BLrG2VQ1RCL4VXQCz8JgzmEZGltJa30s%2F%2BGIWPOAnSANO9Y5ymeEkOCOmOW3%2FyMs%2F0NcIhjrNrGbPsw%2B3iJlnlRESV6fONWbChGt6aziJNKYPd0IogxjONoBYQDpsFBAmxNiFXhA9TP%2FXJF5Un5Pt1QcRUp8MgySoymAxf0Xi4wElKbG2YoJg8BD2SovuBMSKaDuchHqNhc1YHTadkdbquMjtXYXZc2DgijPqImIVoc0NbBqINFE3Zz7tJ6CdJMCHChIA%2FlcUFBJUNtrJGBYOU67NYX0BFU1xY26zYNR5xQO5lqzDTLNOkRH85LbCzim2IUJBtCwXpQkE5b0gFZTrdPvjpataNa9Ar0Wv89hc9X7P45n9ZcdnG3aa09VbcekRxQB4bxUw4w1Fa4A4ARiOwF0UHKdusSdl2TVRehsNNyWKDiPBb5jSAR0wdCeACSd2EolLBGFES%2FPDH2QEZ5RL9Jbkq6W6fsfyE1CtVgkT%2Fy2A6zXCyoqjNHtO6HVh3VFdBGHJdRThCGTnE%2BAUJwjLCJA0D8PCwT8P1mZcYrmaVLBDaCu7VFVwCG%2FB4lIq0JEX%2BKilSQcfvUZGHTPWIJtTumhp1q0vUOgQacJuk11KjzrR9OuUadd1kt1Ocax%2F2kvA6DYOI2AXvTtPKm%2FrJYqvlg46y2r%2BWzLeAAu6aLTdzGkTQ%2FNfE0Jjn9Rxif%2Fo89kM%2FmmTnFW2ZaPjBci3DJHJy6jRAO%2B0zJbdoxLqjl4zYsDzJiHk4oGjDDmxJv%2FDaNqxbRslB0jwXdsNJcmoarNe0wWanEuLx3woHsBaq0mG3dCGu4QIBHHmJjTrXzmF2SF5QOlkMKvq2BUzITbBk%2F7xnTnXNsKXDiuDSMpn4iHz%2FlkeWnp%2FQZB0H6dvzB4LeVfI8yrlCS77P2zV5A%2BiCA6YyesORjb6JiJO64bavYfTNW2jjTWVFX9grm5bFHZ9LdWGdLqmrwN0AOGXutqF1Cnd3HgEWyNolb%2FspG7RtXjam4fa0e9jTEox2a8TXIl1odsmKTze5dtwdmXSFuKHB3eIL2ZjXfRv7I4jTtR8%2Bf%2FEnC9IBa9%2BmKA1aoPCxyyoyZROzdc2zFVbmtOXaXGU07eg6v7T1WEAYRqmwHmXLV27sTMvRHM%2BT2sIDAwONOUNulxSsGiFqOG7kXItvL%2BvTwBqRpsLYG6vXbZhJL%2BuLyh%2F9lHBrlEkgMLYBXJ6UAc%2BP3h4zXGcpQrNWM4N1NizrznZPHawTCjLF2HHbIKgRUOhBUGHAFhRA4J0IAt0VKF8qqgIG1TGrxoFSowvUA6UKKA2xhWmVg9nmhbvBsIaPfi0QHOUESGlYRa9AmTNmXxlAGhScQl71J7Q4B8s6mm0qbtupvFQlwr1Dp7QTV%2BdJiSVk22HKADegyascc%2Fb%2F1jQflKDLMCcAeF5RVDAFLhxv89GGrJAbCon5%2BF90KIY2%2BOSeAbSs4u9fioXac%2FrNIzsDmoeL1yt%2Bg%2BSB83vMD5MsUh7Frz9ML473KzrW5QwA5ZC9Ymi%2Fzfi%2FIwBIZ0UUjNVTGGtrw%2FaGKoO3B9e7BJfuiN1zSxGEuSy8YPfh9Rn7U7JzmyLQo6smukzj2uRVI233n5SEJPuvlXo9GEpiEZaDCQ3cgtsOOUG3ISdSKsi1a3mQjblrcmbqaZTHeSc%2FN1n5Uas0%2BMeX7ABq0%2BA1m1YA7v4z%2BnT%2Fld%2FBOBbviRyV35YkLjPngSegBw9zsqO3rturDb2VjPaFRyJ7d48BvN1v3flle05W3sxfBuFbfmZ%2BDP9v%2B8tVXudZ3leC5hiRHetA2lV90gKF3xHl9iPO8ePAD6uPT%2FwooXMwgtmeIlarEG1rhRjlEv99zG0Xn3XPydl%2F2r4NWZNGK5HOFXkJ0mGcETs%2Fag%2F6duCjOQtcUYYCejrQdC1rXfbiqtPmc76V%2FOT%2BhelYUvfag5rjSD6Gckqe0ZqTISeovwtAcj6HPZ%2F3fH4VPrd7Pv%2BZ%2BdyVwqW2BTVoXJvPVcOKB0BVDY99GDaM2Yx2UcVzA6ruiHIHeHr6eIBlJbS9Z1hVz4Gmn2yWW4xTn80IGXpNQRFKgTEehy3A0FWgsL3QRZ0xy26lshwRfTgcVeh4IkuN1CebR0YulOvEQ7mVvHU%2BMRUmXn789u2xZ6YqZmpqNEg3hf6Oo%2BzvqOb2t8ZMZo01XS48kE4VYBgVtFSph45kWOgCBTnimgd1A5tiQQbcoaUzuTimasCnR8%2Fp2XxCfo4DbE0%2FMTIulmVAQ%2BtcMpdZZ0ynB9Dp9ANOpB8ZifVcqQtCRxWp6zB0ms0NN%2Buuz3Id3Blih%2F5k1hILuj7uVNnqFw5T7XP3ZzM6PUc%2B9%2BbHOkbbgGE0TugXm0dEymKz9n6mXkCl9R0xLQqKjaxiZRbjog599%2FLoT2tRD0YVego8LynWELHLrtNqeqvZvez99%2B3wCWt%2FOM6JqBML2uZ2dafh7V7O%2F%2FuGDtA1bo4cPWLAtDZnuWB%2FQVdHD6%2B0Hj0NhSpEjTu70b5z0dM97uHTnXr0NMU91n6N%2F4OgAxXQuXB%2FsXbyDqTJOxU9R%2FCVQBGCb8hfZhssRgHBB2GaRkW%2BxN6OI8VltkZge71HwX4eHrJ%2BsspW9lOA2Dncvk6AXX1QXLFf1WkEmukIDa9xnlXxQ%2FBslqBzxyOVsw6rQdzpvB6eFkfP6dPi%2BrS4y6fFOX1a3PuODyr4XvKrjklztmw5Gam1nDgll6umrAh6Ov41LhP2zhb6Romn7N0S8ttbzqpKQ3h7i8Vd0QNJXeISB41V4zvNFL%2F%2F%2FKmtxrDTz91z2bkGaAkpcboieUm1Cn1rRNa9oQ6hvuu8ZKk4ztEv%2BHHJ7rqyto8bnzj3PUCHAXI1xQvDWdJ6YHW1Lq1OLo5QtD1Dt3q8vtPt1b%2FXy9Utpp3GP%2FO2%2BiZKAtpi%2FHStVtMTDQ1X4YG3NUhfTelHQ7Iqs%2BNikGRrZ9xu184ANIea0OGAvrsHhz8fNM%2FrHFryHFjFCkG6c0locrY%2Bzqnqm7kLNnNqvakitL3j8p41%2Bj7jNBZwNFheHdw0gWYZhXWjbYnkCBV6ineAWvKgcnNMVyOBuJP162puefTI0pUziUjlOaaiTp0W67TGUs5drFMdipi1ecJ7WyAlm7vXeeecsXsnunH%2Ffw%3D%3D)
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
##### Which file is the playbook? Where do you copy it? filebeat-playbook.yml; 
###### /etc/ansible/roles
##### Which file do you update to make Ansible run the playbook on a specific machine? 
###### /etc/ansible/hosts
##### How do I specify which machine to install the ELK server on versus which to install Filebeat on? 
###### Create separate groups to specify. One named “webservers” the other named “elk”
##### Which URL do you navigate to in order to check that the ELK server is running? 
###### http://104.41.155.230:5601/app/kibana

