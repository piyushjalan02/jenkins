# jenkins
Master-Slave Concept:

Every time when we need to create build for Ios, We must connect the Slave first. When we request for a build the request actually goes to 
slave and uses xcode of slave machine for build the IPA. After creating the IPA successfully it will store IPA in output directory as 
mentioned in configuration.

Master
Jenkins Master Server
URL:- http://example.com:9999/
JNLP Port:- 7072

Slave (Where xcode is installed and running.)
Local mac Machine(192.168.1.98)
Working Directory :- /var/jenkins
Output Directory :- /Users/ranosys/.jenkins/workspace/${JOB_NAME}/
Ipa File Pattern:- Project_Name-${JOB_NAME}-${BUILD_NUMBER}-${BUILD_DATE}
