# weblogic_server_ansible_vagrant
Provision Weblogic Server with Ansible and Vagrant

# Setup
1. Install VirtualBox - see https://www.virtualbox.org
2. Install Vagrant - see http://www.vagrantup.com/downloads
3. Install Ansible - see http://docs.ansible.com/intro_installation.html. According to the official website, the preferred way to install Ansible on a Mac is via pip (http://docs.ansible.com/ansible/intro_installation.html#latest-releases-via-pip). However, I encountered some errors and so I did `brew install ansible`.
4. Download Weblogic Server generic installer from http://www.oracle.com/technetwork/middleware/weblogic/downloads/index.html to `wls_vm/ansible/roles/wls/files/fmw_12.1.3.0.0_wls.jar`.
5. Download Oracle JDK from `http://www.oracle.com/technetwork/java/javase/downloads/index.html` to `wls_vm/ansible/roles/jdk/files/jdk-8u60-linux-x64.rpm`
6. Run `vagrant up` to bring up the VM.
7. Run `vagrant provision` to re-provision the VM.
