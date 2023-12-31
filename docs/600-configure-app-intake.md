---
layout: default
parent: Implementation
title: 6) Configure App Intake
nav_order: 600
nav_exclude: false
permalink: /docs/configure-app-intake
---

# 6) Configure Application Intake

---

{: .highlight}
> **[Application Intake](https://docs.servicenow.com/csh?topicname=config-app-intake.html&version=latest)** has already been configured as part of the setup for this lab. 
>
> This section can be safely skipped and will not affect the rest of the lab. 
>
> We are providing the information below to help add context.

Application Intake is configured in the Prod Environment and consists of a few important tasks:

- Set the ```sn_app_intake.instance_can_provision_users``` system property to **true**.

- Set the Catalog Item **Apply for Citizen Development - V2** to **active=true**. *This catalog item can be configured to suit the needs of your organization.*

- Add users to the App Engine Admin group.

{: .note}
> For more information see **[Product Docs: Customize the App Intake form in Catalog Builder](https://docs.servicenow.com/csh?topicname=customize-app-intake-form-catalog-builder.html&version=latest)**

[Next](/lab-aemc-utah/docs/intake-request){: .btn .btn-green .fs-2}