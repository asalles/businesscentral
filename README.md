This is playbook to create the Business Central, which it's a integral part of LATAM Red Hat Forum 2016. 
Before running, check the following variables and change accordingly: 

This should be an existing user already created on OpenShift. 
username: demo  

Name of the Project (OpenShift's NameSpace) that it will be created.
If one already exists with this name, it's going to be deleted first. 
openshift_namespace: business-central

This would be the domain added to each service
domain_route_postfix: cloudapps.forum.rhtechofficelatam.com
