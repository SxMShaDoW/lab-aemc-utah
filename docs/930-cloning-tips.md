---
layout: default
title: Cloning tips and tricks
parent: References
nav_order: 930
permalink: /docs/cloning-tips
---

# Cloning Tips

If App Engine Studio is the only application using the Credentials table, consider creating data preservers for Credential Alias, Basic Auth, and Discovery credentials -- otherwise, ensure that these tables are not overwritten when the production instance is cloned down to sub-production instances.

App Engine Studio has data preservers on the following tables:
-   Pipeline Instance
-   Request Authorization Key
-   Deployment Request
-   Deployment Environment Request

To ensure application and developer data is not lost in development environments during a clone, add **data preservers** to the following:

-   Collaboration Descriptor tables:
-   App Collaboration Descriptors **[sys_appcollab_descriptor]**
-   App Collaboration Descriptor Permissions **[sys_appcollab_permission_m2m]**
-   Collaboration Users and Groups tables:
-   App Collaboration Users **[sys_appcollab_user]**
-   App Collaboration Groups **[sys_appcollab_group]**

Additionally, add **clone excludes** for the following Collaboration Descriptor tables. so that data in these tables are preserved after cloning and that no data from the source instance gets copied over. It is ok to have data merge from source and target for collaboration users and groups tables.

-   App Collaboration Descriptors **[sys_appcollab_descriptor]**
-   App Collaboration Descriptor Permissions **[sys_appcollab_permission_m2m]**

After cloning, a post-clone clean-up script is needed to reassign users and groups the appropriate delegated development permissions. We assume that in-development applications are backed up before cloning and users/groups are same between target and source instance.

***Note:** New App Engine Studio customers (Tokyo +) will only have data preservers on the tables listed above. Existing customers (pre-Tokyo) will also have data preservers on the following tables : Pipeline, Environment. Pipeline Environment Order, Pipeline Types*

[Next](/lab-aemc/docs/credential-tips){: .btn .btn-green .fs-2}