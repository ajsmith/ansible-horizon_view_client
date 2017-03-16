========================================
VMware Horizon Client Setup with Ansible
========================================

Installation of the VMware Horizon Client on Fedora/RHEL is quite a horrible
experience, so here are some Ansible resources to help make it not so bad.


Getting Started
===============

#.  Create an inventory file containing the hosts that you want to install the
    Horizon client to::

      $ cat << EOF >inventory.cfg
      myhost
      EOF

#.  Run the "install.yml" playbook::

      $ ansible-playbook install.yml

If everything goes as planned, then you should have the Horizon client
installed now!

You can start the client on the host as so::

  $ vmware-view
