
This is an everyday basic 4 node BGP based Ansible automation demo. 

Requirements are a management VM, 4 Cumulus VX VM's configured as 2 leaf and 2 spine. Runs on VirtualBox.

- cumulus-config.yml - configures the 4 node demo. when this playbook runs to completion, the demo is operational.
- cfgshow.yml & cfgshow (bash script) - meant to show various configurations of the 4 VX VM's.
- bgpshow.yml - takes the bgp commands that are in the cfgshow bash script and seperates them as a sep playbook
- clean.yml - removes the configurations, resets the VX VM's back to their basic defaults
- update.yml - runs apt-get update

Subdirectories have supporting configuration files specific to those VM's.
