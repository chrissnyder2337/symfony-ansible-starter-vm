# Ansible provisioning

Adding and Updating Galaxy roles
From time to time, third party roles need to be added or updated to enable new functionality or fix bugs. 
To update a role (e.g. geerlingguy.apache), find the role's version setting inside requirements.yml, 
bump the version to the required or latest version of the role, then run the following command in the 
same directory as this README file:

$ ansible-galaxy install -r requirements.yml --force

Then commit the updated requirements.yml file and the new and updated files within the roles directory.