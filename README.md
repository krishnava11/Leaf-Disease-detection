# PlantDiseaseDetection

It is a plant disease detection project...
cnn.py is used to train and test the model
ui.py is used for finding the disease in the given leaf by the user

PACKAGE REQUIREMENTS
  numpy (pip install numpy)
  tqdm (pip install tqdm)
  TensorFlow
  openCv
  matplotlib
  
  
## Jenkins & EC2 instance Deployment
  
- Requires Ansible 1.2 or newer
- Expects CentOS/RHEL 6 or 7 hosts

These playbooks deploy latest Jenkins Server in jenkins.org and creates a profile with "Ansible_Project",
having Username "admin" and Password "admin@123".
To use them, first edit the group_vars/all file to set any EC2 configuration parameters you need.

Then run the playbook, like this:

	  ansible-playbook -i hosts site.yml
    
When the playbook run completes, you should be able to see the EC2 Instance running and 
Jenkins Server running on the port 8080.

  
  
