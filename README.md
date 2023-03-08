# Catalinul-ProgramingAssessment
Deploying with Ansible the ToDo app from Docker's tutorial

Video of the controller node with Ansible and the remote VM target [can be found here](https://youtu.be/5JlXS67otDc). 
Unfortunately, I didn't know where I can get an online VM from, in order to just share the link with it. I had to go with VirtualBox and classic VMs.

For both the Ansible VM and for the target VM I have used CentOS 7. I had an image lying around on my computer.

The command I've used to run the playbook is:

'''
sudo ansible-playbook start-app.yml -v
'''



