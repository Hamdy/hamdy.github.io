# HA Cluster

- `watch pcs cluster status`

It will change from 
```
Every 2.0s: pcs cluster status                 node1.demo.in: Mon Sep  2 13:33:17 2024

Warning: Unable to read the known-hosts file: No such file or directory: '/var/lib/pcs
d/known-hosts'
Cluster Status:
 Cluster Summary:
   * Stack: corosync (Pacemaker is running)
   * Current DC: node1.demo.in (version 2.1.6-6fdc9deea29) - partition with quorum
   * Last updated: Mon Sep  2 13:33:17 2024 on node1.demo.in
   * Last change:  Mon Sep  2 13:33:16 2024 by hacluster via crmd on node1.demo.in
   * 3 nodes configured
   * 0 resource instances configured
 Node List:
   * Online: [ node1.demo.in node2.demo.in node3.demo.in ]

PCSD Status:
  node1.demo.in: Unable to authenticate
  node2.demo.in: Unable to authenticate
  node3.demo.in: Unable to authenticate
```
to

```
Every 2.0s: pcs cluster status                 node1.demo.in: Mon Sep  2 13:33:59 2024

Cluster Status:
 Cluster Summary:
   * Stack: corosync (Pacemaker is running)
   * Current DC: node1.demo.in (version 2.1.6-6fdc9deea29) - partition with quorum
   * Last updated: Mon Sep  2 13:33:59 2024 on node1.demo.in
   * Last change:  Mon Sep  2 13:33:16 2024 by hacluster via crmd on node1.demo.in
   * 3 nodes configured
   * 0 resource instances configured
 Node List:
   * Online: [ node1.demo.in node2.demo.in node3.demo.in ]

PCSD Status:
  node3.demo.in: Online
  node1.demo.in: Online
  node2.demo.in: Online
```


pcs resource list (list)
pcs resource startu-debug apache (see what is issue if the resource stopped)

corosync-quorumtool
Quorum information

