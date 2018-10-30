Azure Edge
==========

This role deploys an Azure IoT Edge to a destination VM or machine.

Build Status
------------

[![pipeline status](https://gitlab.eng.vmware.com/vmworld2018/ansible-role-azure-edge/badges/master/pipeline.svg)](https://gitlab.eng.vmware.com/vmworld2018/ansible-role-azure-edge/commits/master)

Requirements
------------

You will need to supply Azure credentials to run this role.  Create an
application principal as described here:
https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-create-service-principal-portal

Role Variables
--------------

TBD.

Dependencies
------------

This role does not explicitly depend on any other roles.

Example Playbook
----------------

Here's an example playbook:

    - hosts: servers
      roles:
         - { role: vmware.azure-edge }

Contributing
------------

The ansible-role-microsoft-azure-edge project team welcomes contributions from the community. If you wish to contribute code and you have not
signed our contributor license agreement (CLA), our bot will update the issue when you open a Pull Request. For any
questions about the CLA process, please refer to our [FAQ](https://cla.vmware.com/faq). For more detailed information,
refer to [CONTRIBUTING.md](CONTRIBUTING.md).

License
-------

MIT

