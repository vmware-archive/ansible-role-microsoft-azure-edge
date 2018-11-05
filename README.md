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

The ansible-role-microsoft-azure-edge project team welcomes contributions from the community. Before you start working with ansible-role-microsoft-azure-edge, please read our [Developer Certificate of Origin](https://cla.vmware.com/dco). All contributions to this repository must be signed as described on that page. Your signature certifies that you wrote the patch or have the right to pass it on as an open-source patch. For more detailed information, refer to [CONTRIBUTING.md](CONTRIBUTING.md).

License
-------

MIT

