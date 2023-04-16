rnodec.os_baseline
=========

This ansible role handles the basic configuration of a brand new node used in the rnodec rke2 cluster.  Handles things like:

* system update
* ssh hardening
* configuring local users

Requirements
------------

A linux server

Role Variables
--------------

* os_baseline_sshd_port: anything other than 22
* os_baseline_admin_users: list of local user accounts to set up.  These accounts will be authorized to ssh via pubkey authentication and be added to sudoers.

Dependencies
------------

None


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: rnodec.os_baseline }

Author Information
------------------

RnodeC - rnodec.io
