# tomcatScripts-Middleware-
This repository contains tomcat native and custom installation and runtime control scripts.
tcruntime-instance          - This is a native script provided by VMware for tomcat provisioning.
tcruntime-ctl               - This is a native script provided by VMware for controlling runtime i.e. start | run | stop | restart | status.
cg-tcruntime-instance-v3    - This is the custom script for tomcat installation which in turn calls native tcruntime-instance script by taking additional params like AppName, AppInstance, version to create the directory structure and creates instances.


The above installation scripts should be present in a directory - /users/mwtools/tc and should be run by mwadmin account.
These scripts create the instances in /users/domains/tomcat/$APP_NAME/$INSTANCE_NAME. 
The created servers should be managed by webapp account.
