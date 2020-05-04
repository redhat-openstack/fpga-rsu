fpga-rsu
=========

This is a standard Ansible role to install OPAE FPGA packages on hosts.


How to install
--------------

ansible-galaxy install git+https://github.com/redhat-openstack/fpga-rsu.git


How to use
----------

This role can be included in playbooks to use as mentioned in below example.

You should download the OPAE FPGA package tarball from intel portal and set the correct values for role parameters.


Role Variables
--------------

* **fpga_rsu_driver_pkg_url**: Path to the downloaded OPAE FPGA package tarball.
  Default to ""

* **fpga_rsu_driver_dir**: Directory location where to untar the package.
  Default to '/usr/share/opae'.


Example Playbook
----------------

Including an example of how to use your role:

```yaml
- hosts: servers
  become: true
  roles:
     - role: fpga-rsu
```

How to contribue
----------------

Patches should be submitted using git review to the GerritHub.


License
-------

Apache 2.0


Author Information
------------------

redhat-openstack
