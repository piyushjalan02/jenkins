1. java -DJENKINS_HOME=/usr/lib/jenkins -jar jenkins.war --httpPort=9090
(To run Jenkins on different Port)

2. SDK working directory: (To Update the Android SDK)

Cd /var/lib/jenkins/tools/android-sdk/
./android list sdk --all
./android update sdk -u -a -t 118

3. Project workspaces:

/var/lib/jenkins/jenkinsworkspace
service jenkins status/stop/start

4. Poll SCM Varible:- For setting up the Cron for autobuild

5. AutoCommit Message with the Mail:- ${CHANGES format:"%m"}

6. If we don't need to add path of the repositories, then ${CHANGES, showPaths=false, format="%m"} and in case there is no change from last commit in that case it will show "No changes".

7. Gredlew Issue on Jenkins:
Gredlew is a type of tool which help to create our software and provides all required libraries needed for project.

We need to commit all three files for gredles:
Gredlew
Gredlew.properties
Gredlew.jar 

Note that all three file should be at the mentioned branch and must be committed.

WE MUST DO:-
1. Plugin Installed:-
a. Keychains and Provisioning Profiles Management (Add Keychains,Code Signing Identity, Provisioning Profiles Directory Path)
2. Manage Node --> Add a new node
3. Launch Method = Launch agent via Java Web Start
4. Launch Java Applet from Slave machine
5. Fix a port on ranosys.net server for JNLP Agent and allow access of it through firewall
6.On Slave machine Xcode must be installed.
