---
layout: default
parent: 2) Pipelines & Deployments
title: 2.2) Configure non-Prod
nav_order: 220
has_children: false
permalink: /docs/configure-non-prod
---

# 2.2) Configure Controller Environment in Dev Instance

We need to make sure the Dev environment knows where to send Deployment Requests. 

They will get sent to App Engine Management Center in Production for review by the App Engine Admin Group.

{: .warning}
> Complete this section in **DEV**.

{: .highlight}
> For the purposes of this lab, it is not important what Application Scope you create the environment records in. Global is fine. 

## Environment setup

| 1) Log in to the **DEV** environment. 

| 2) Click **All** >> type **environment** >> click **Environments** 
| ![](../assets/images/2023-07-05-09-45-11.png)

| 3) Click **New** in the top-right
| ![](../assets/images/2023-06-30-15-19-10.png)

| 4) Complete the form using the information below. 

| Field | Value 
|:---|:---
| Name | ```Prod``` 
| Instance Type| ```Production``` 
| Instance URL | ```The full URL of your Prod Lab instance (Ex. https://your-lab-123.service-now.com)``` 
| Instance credential | ```Pipeline_Credentials``` 
| Is Controller? | ```Checked``` 
| Instance Id | ```This will auto populate after clicking Validate```

| ![](../assets/images/2023-03-13-10-31-06.png)
| ![](../assets/images/2023-07-05-13-56-23.png)

| You should see a blue message that says "The controller environment was validated successfully". 
| ![](../assets/images/2023-03-12-17-05-44.png)

| 14) Click **Submit** to finish creating the **Prod** environment record.
| ![](../assets/images/2023-07-05-14-01-45.png)

**Congratulations!**

You're one step closer to deploying apps with App Engine Management Center. 

{: .note}
> For more information see **[Product Documentation: Define environments](https://docs.servicenow.com/csh?topicname=config-pipeline-environments.html&version=latest)**

[Next](/lab-aemc-utah/docs/app-intake){: .btn .btn-green .fs-2}