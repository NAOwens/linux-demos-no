linux-demos-no Project
=========

Contains various playbooks to manage linux hosts.

Requirements
------------

leapp.yml and rhelupdate.yml assume that the host is registered to Satellite server.
register_to_sat.yml can be used for the initial registering of a host to Satellite.

Variables
--------------

survey_hostname is provided in AAP as the host you want to run the playbook against.

sat_register_vars.yml uses a vars file vars/sat_register_vars.yml which contains the activation key defined in satellite and its curl command needed to register the host ie: RHEL7_AK: "curl command"

Dependencies
------------

The project uses collections:
 - ansible.builtin

Project Playbooks
----------------
leapp.yml - used to do leapp upgrade from rhel7-to-rhel8 or rhel8-to-rhel9

register_to_sat.yml - used to register host to satellite if new build or if snapshot restored and host needs to be re-registered to satellite

image_bldr_inst.yml - used to install on-prem image builder

rhelupdate.yml - update rhel minor version

License
-------

GPL

Author Information
------------------

Norman Owens