---
{"dg-publish":true,"permalink":"/permissions/"}
---


**Directory configuration

Two different paths are used for the interfaces:

/wls/maestro/INTERF with the following subdirectories:

| Outbound                | Inbound                | Temporary               | Archive |
| ----------------------- | ---------------------- | ----------------------- | ------- |
| /wls/maestro/INTERF/OUT | /wls/maestro/INTERF/IN | /wls/maestro/INTERF/WRK |/wls/maestro/INTERF/BKP         |

/data/INTERFACE (and subdirectories), it's the alternative path if there are specific requirements for specific interfaces (tipically used to keep certain files in a dedicated path)


**User requirements

One group in common (not necessarily the primary one) between 
1. the SAP user used by the batch processes
2. the SFTP user configured in the PO communication channels.

For example, supposing that "repadm" is the SAP user, whilst "spazio" is the PO user:

```shell
$ groups repadm
repadm : sapsys nadshm sapdata sapinst erpgone
```

```shell
$ groups spazio
spazio : sapdata z1aftp
```

"sapdata" is the primary group of "spazio" user and an additional group of "repadm" user. This is the group the two users have in common.
  
  
**Directory requirements


1. Directory group should always be set to the common one

```shell
$ chgrp -R sapdata /wls/maestro/INTERF
```

2. It’s recommended that for each directory the **setgid** bit is set, in order for files and subdirectories created within to inherit the directory group ownership, rather than the primary group of the file-creating process

```shell
$ chown -R g+s /wls/maestro/INTERF
```

3. Depending also on the umask settings of the users, if ACLs are available it could be useful to set an explicit default ACL, in order to have all the objects created inside a specific directory tree to inherit the "rw" permission for the group. This because sometimes the default umask set for a user do not enforce read/write permission on the group, which in this case is paramount since it's the practical way with which files can be shared between different users. In the below example this is enforced only for the archive directory, but it can be extended to the other as well.

```shell
$ setfacl -R -m -d g:sapdata:rw BKP
```

Result after setting all the permissions:

```shell
$ ls -Alh --time-style=+"" /wls/maestro/INTERF

drwxrwsr-x+ 2 spazio sapdata 2.4M  BKP
drwxrwsr-x   2 spazio sapdata 4.0K   IN
drwxrwsr-x   2 spazio sapdata 240K  OUT
drwxrwsr-x   2 spazio sapdata 4.0K   STOR
drwxrwsr-x   2 spazio sapdata 4.0K   WRK
```
``
