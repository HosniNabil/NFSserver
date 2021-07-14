NFSserver
=========

NFS server configuration



Role Variables
--------------
The variables required for this role are:
- shared_dir : the NFS shared directory to be configured
- permissions: Linux permissions for the directory to be created (in Octal format)


Example Playbook
----------------


    - hosts: nfs_servers
      roles:
         - { role: hosninabil.NFSserver, shared_dir: nfstest, permissions: '0755' }

License
-------

Apache-2.0

Author Information
------------------

Nabil Hosni, cloud engineer and opensource enthusiast.
