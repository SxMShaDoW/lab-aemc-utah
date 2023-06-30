---
layout: default
title: 2) Credentials
nav_order: 200
permalink: /docs/credentials
---

# 2) Credentials

In this lab, we will configure Service Account Credentials that allow App Engine Studio and App Engine Management Center to communicate.

Set up and configure the environments that will be included within your pipelines. These will be referenced when building your pipelines.

Your production instance is where your pipeline configurations reside and will be your controller instance.

The 'Is Controller?' box will be **checked** on your production instance only. This box will be **unchecked** for all sub-production Environment records.

If you have **more than one** Production environment, then AEMC will be the controller on a single instance for all of your other Prods.

{: .warning}
> Complete the steps below in all of your Lab environments.  
>
> Start with Prod then Dev.

{: .highlight}
> For this lab, the credentials will be created in your current scope which should still be "App Engine Studio".
>
> Check with your Platform Administrator to see if there are any preferred policies around connection and credential storage. 

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
> Remember to complete the steps above in all of your Lab environments before continuing to the next exercise. 

{: .note}
> For more information, see **[Product Documentation: Create a Connection & Credential Alias](https://docs.servicenow.com/csh?topicname=connection-alias.html)**

[Next](/lab-aemc/docs/pipelines-deployments){: .btn .btn-green .fs-2}