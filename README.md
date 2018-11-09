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

The primary variable required is ```azure_edge_name```, which will be injected
into configuration files as the identity of this edge.  If this role is run in
same playbook as the Azure IoT role, other variables will be inherited from
host vars discovered by that role.  If this role is run at a different time,
the following variables are required.

``` yaml
# Name of the IoT hub
azure_iot_hub_name: azure-iot-hub-name

# This would typically be set as a host variable, on the particular host
# that is to be configured as the edge.
azure_edge_name: azure-edge-name

# Map of known data. Normally this would be discovered by the
# azure-iot role, but can be specified as vars as well.
azure_groups:
  azure-edge-name:  # this should be the real edge name configured in portal
    primaryKey: primary-key # the primary key available in the portal
```

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
