# CI-example
This repository will store code for the continuous integration using Jenkins and Ansible

# Run Sonar Scan

```
mvn sonar:sonar -Dsonar.projectKey=com.ansible -Dsonar.host.url=http://localhost:9000  -Dsonar.login=admin -Dsonar.password=admin

```================================================================================================================================================
This pipeline was designed to do continuos deployment on a monolithic environment .
Ansible is using ssh connection to deploy tha application to the different hosts.
We defined our ansible playbook in jenkins 
we configure our jenkins to install the ansible plugins .
we hook our jenkins to our github repo using webhook such that ones there is a push ,
our jenkins pipeline will run.
