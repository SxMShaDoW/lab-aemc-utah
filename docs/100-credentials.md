---
layout: default
title: 1) Credentials
nav_order: 100
permalink: /docs/credentials
---

# 2) Credentials

In this lab, we will configure **Service Account Credentials** that allow App Engine Studio and App Engine Management Center to communicate across environments. Check with your company policy on Service Accounts for requirements. 

{: .highlight}
> For the purposes of this lab, it is not important what Application Scope you create the credentials in. Global is fine.
>
> Check with your Platform Administrator to see if your company has any policies around **[Connection and Credential Aliases](https://docs.servicenow.com/csh?topicname=connection-alias.html&version=latest)**.

{: .warning}
> **Complete the steps below in all of your Lab environments.**
>
> Start with **Prod** then **Test** then **Dev**.
>
> Some Labs may only have a **Prod** and **Dev**.  

| 1) Navigate to **All**.

| 2) Type "**Connection & Credential Aliases**"

| 3) Click on **Connection & Credential Aliases**.
| ![](../assets/images/2023-03-07-15-28-59.png)

| 4) Click the purple **New** button in the top-right to create a new Credential Alias record. 
| ![](../assets/images/2023-03-07-15-38-10.png)

| 5) Set the **Type** to **Credential**. 
| ![](../assets/images/2023-03-07-15-37-39.png) 

| 6) Set the **Name** to `Pipeline Credentials` and click **Submit**.
| ![](../assets/images/2023-03-08-14-14-44.png)

| 7) Click **Pipeline Credentials** to open the record. 
|![](../assets/images/2023-03-09-13-48-09.png) 

| 8) Navigate to the **Credentials** Related List and click **New** to add a credential. 
|![](../assets/images/2023-03-09-13-49-03.png)

| 9) Select **Basic Auth Credentials**.
|![](../assets/images/2023-03-09-13-50-33.png)

| 10) On the **Basic Auth Credentials** form, fill in these values and click **Submit**. 
|![](../assets/images/2023-06-27-22-50-59.png)

**Click the clipboard icon on the right of the gray box below to copy.**

```markdown
Pipeline Service Account
```
```markdown
svc_pipeline
```
```markdown
ILoveHyperAutomationTimes500!
```

{: .warning}
> **STOP!!**
>
> Did you repeat the instructions above for both **Prod** and **Dev**?
>
> Remember to start with **Prod** then **Test** then **Dev**.

{: .note}
> For more information, see **[Product Documentation: Create a Connection & Credential Alias](https://docs.servicenow.com/csh?topicname=connection-alias.html)**

[Next](/lab-aemc-utah/docs/pipelines-deployments){: .btn .btn-green .fs-2}