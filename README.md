Version: "1.0.0"
Git Hub Repo location:

https://github.com/wardcomm/windows_update

Role Name
=========
 An Ansible Galaxy Role:
 -- windows updates

Role Variables
--------------

patching_windows_reboot_allowed: true
patching_windows_update_allowed: true
patching_windows_reboot_timeout: 3600
patching_windows_categories:
  - CriticalUpdates
  - SecurityUpdates
  - DefinitionUpdates
  - UpdateRollups
  - Updates
  - ServicePacks
  - FeaturePacks

Dependencies
------------

no deps

Example Playbook
----------------

- hosts: all
  vars_files:
    - vars/main.yml
  roles:
    - { role: wardcomm.windows_updates }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
