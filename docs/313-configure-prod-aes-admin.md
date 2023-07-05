---
layout: default
grand_parent: 3) Pipelines & Deployments
parent: 3.1) Configure Prod
title: 3.1.3) AES Admin in Prod
nav_order: 340
permalink: /docs/configure-prod-aes-admin
nav_exclude: true
---

2023.07.05 - Dale: I removed this page as it is now set up via automation. 

# 3.1.2) Configure Prod AES Admin Group

Configure App Engine Studio administrator group membership in the **production** instance to manage application intake and deployment requests.

{: .warning}
> Complete this section in **PROD**.

{: .highlight}
> *If you only have a **DEV** and **TEST** instance, then treat your **TEST** instance as if it were **PROD**.*


## Add users to the App Engine Studio Administrators group

| 1) In the 'Add users to the App Engine Admins group' section, click **Configure**.
| ![](../assets/images/2023-03-12-20-57-36.png)

| 2) In the 'Group Members' related list, click **Edit...**.
| ![](../assets/images/2023-03-12-21-00-01.png)

| 3) Search for **Jayne Nigel**, move her to the right side of the list collector, and click **Save**. 
| ![](../assets/images/2023-03-12-21-05-49.png)

| 4) Click **X** to exit the modal. 
| ![](../assets/images/2023-03-12-21-07-00.png)

| 5) In the 'Add users to the App Engine Admins group' section, click **Complete**. 
| ![](../assets/images/2023-03-12-21-07-42.png)

| 6) Click 'Pipelines and Deployments Guided Setup' at the top of the page.
|![](../assets/images/2023-03-12-21-08-59.png)

**Congratulations!** 

Your Production instance is configure for App Engine!

Next, you will configure your non-production instances. These are also sometimes referred to as subproduction.

[Next](/lab-aemc-utah/docs/configure-non-prod){: .btn .btn-green .fs-2}
