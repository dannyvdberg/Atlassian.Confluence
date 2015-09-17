## Atlassian Confluence by Avisi

Ansible rols which installs and configures a basic Atlassian Confluence Installation


#### Requirements & Dependencies
- Tested with Ansible 1.9.3 or higher
- Tested with Ubuntu 14.04
- Java 1.8*
- MySQL, PostgreSQL, Oracle, MSS


#### Variables

```yaml
confluence_versie: 5.8.10 										# Version of JIRA Installation
confluence_user: confluence 									# Server user that runs and stops JIRA
confluence_installatie_directory: /opt/atlassian/confluence 	# Default Installation Directory
confluence_data_directory: /opt/application-data/confluence 	# Default Data Directory

confluence_backdoor_connector: "yes"  							# Enter and change yes when you want to use a backdoor connector
confluence_proxy_name: "myconfluence.com" 						# Enter and change your proxyName
confluence_proxy_port: "443" 									# Enter and change your proxyPort
confluence_proxy_scheme: "https"								# Enter and change your proxyScheme
confluence_path: "/mycompany"									#Enter and change  path if you want to use it
mysql_connector: "yes"											# Enter yes when you use MySQL as database

confluence_memory_settings_mn: 1024 							# Edit value for a different memory settings		
confluence_memory_settings_mx: 2048								# Edit value for a different memory settings
```


###Example Playbook
```yaml
---
 - hosts: webservers
   roles:
   - dannyvdberg.Atlassian.JIRA
```


###Author Information
- Author:		Danny van den Berg
- Company:		Avisi


###Feedback, bug-reports, requests, ....
Feedback is welcome! Please send a e-mail to ddvandenberg@gmail.com


