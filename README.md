Azure Edge
==========

This role deploys an Azure IoT Edge to a destination VM or machine.

Build Status
------------

[![pipeline status](https://travis-ci.org/vmware/ansible-role-microsoft-azure-edge.svg?branch=master)](https://travis-ci.org/vmware/ansible-role-microsoft-azure-edge)

Requirements
------------

This role deploys the code for an Azure Edge to the target instance, but the
server side definition must have already been created and configured in the
Azure Portal (or automated with [Azure Iot](https://github.com/vmware/ansible-role-microsoft-azure-edge) ).

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
