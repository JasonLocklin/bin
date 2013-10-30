~/bin
=====

Just a repository of short bash and python scripts for simplifying various tasks.



Other Command Line Notes:
========================

Bash
----
Looping:

    for f in *.txt; do echo "$f"; done


Rsync
-----

Parallel Rsync (sort of):

    rsync /source/[0-9]* root@1.1.1.1:/source_backup/
    rsync /source/[a-h]* root@1.1.1.1:/source_backup/
    rsync /source/[i-p]* root@1.1.1.1:/source_backup/
    rsync /source/[q-z]* root@1.1.1.1:/source_backup/


SSH
---

Proxy

    ssh -N -D 9999 -Nf user@host

Server fingerprint

    ssh-keygen -l -f /etc/ssh/ssh_host_dsa_key
    ssh-keygen -l -f /etc/ssh/ssh_host_ecdsa_key
    ssh-keygen -l -f /etc/ssh/ssh_host_rsa_key

