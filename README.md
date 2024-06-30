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

linux-demos-no Project Playbook
----------------

License
-------

GPL

Author Information
------------------

An optional section for the project authors to include contact information, or a website (HTML is not allowed).
