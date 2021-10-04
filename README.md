NFSserver
=========

NFS server configuration



Role Variables
--------------
The variables required for this role are:
- nfs_setup: true|false : setup nfs server or not
- add_share: true|flase : add shared directory
- shared_dir : the NFS shared directory to be configured
- permissions: Linux permissions for the directory to be created (in Octal format)
- remove_share: true|false : delete shared directory


Example Playbook
----------------


    - hosts: nfs_servers
      roles:
         - { role: hosninabil.nfsserver, shared_dir: /nfstest, permissions: '0755' }

License
-------

Apache-2.0

Author Information
------------------

Nabil Hosni, cloud engineer and opensource enthusiast.
