# gardener

Bootstrap a (virtual) server and apply some basic security precautions. The setup process was only tested with Debian so far. 

## Prerequisite 

The Debian OS must be installed and a sshd server supporting public key authentication must be setup accordingly.

## (Virtual) server setup

Following packages will be installed and configured: 

- user  
  - authorize public ssh keys 
  - added to sudoers
- sshd 
  - publickey (SSH key)
  - Disable root login 
  - Only allow specified user to login 
- fail2ban 
- logwatch 
- ufw
- nginx
  - provide a static webiste 
  - allow access via https  
