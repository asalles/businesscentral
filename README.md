This is playbook to create the Business Central, which it's a integral part of LATAM Red Hat Forum 2016. 
It must run inside OpenShift as "system:admin" and Gogs must be running with the following content:

[PENDING: ORIGINAL CONTENT TO BRMS]

...which it's going to be used as:
http://demo:r3dh4t1!@gogs:3000/demo/brms.git

Before running, check the following variables and change accordingly: 

This should be an existing user already created on OpenShift. 
username: demo  

Name of the Project (OpenShift's NameSpace) that it will be created.
If one already exists with this name, it's going to be deleted first. 
openshift_namespace: business-central

This would be the domain added to each service
domain_route_postfix: cloudapps.forum.rhtechofficelatam.com

!!!! IMPORTANT: Before running this scripts, it's important that you download the following files from http://access.redhat.com

JBoss EAP 6.4.0 Installer
https://access.redhat.com/jbossnetwork/restricted/softwareDownload.html?softwareId=37383
file: jboss-eap-6.4.0-installer.jar

JBoss EAP 6.4.7 Patch
https://access.redhat.com/jbossnetwork/restricted/softwareDownload.html?softwareId=43071
file: jboss-eap-6.4.7-patch.zip

JBoss BRMS 6.3.0 GA Installer
https://access.redhat.com/jbossnetwork/restricted/softwareDownload.html?softwareId=43631
file: jboss-brms-6.3.0.GA-installer.jar

Those files must be in the following directory: businesscentral/templates/rhcs-bc/installs
