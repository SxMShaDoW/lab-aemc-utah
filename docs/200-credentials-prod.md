---
layout: default
parent: Implementation
title: 2a) Create Credentials in Prod
nav_order: 200
permalink: /docs/credentials-prod
---

# 2a) Create Credentials in Prod

---

In this exercise, we will configure **Service Account Credentials** that allow App Engine Management Center to communicate to the Environments in the Pipeline.

{: .warning}
> Complete this section in **PROD**.

{: .highlight}
> For the purposes of this exercise, it is not important what Application Scope you create the credentials in. Global is fine.
>
> Check with your Platform Administrator to see if your company has any policies around **[Connection and Credential Aliases](https://docs.servicenow.com/csh?topicname=connection-alias.html&version=latest)**.

| 1) Log in to **PROD**

| 2) Click **All** » type **Connection & Credential Aliases** » click the SECOND **Connection & Credential Aliases**
| ![](../assets/images/2023-07-11-15-10-23.png)

| 3) Click the purple **New** button in the top-right to create a new Credential Alias record. 
| ![](../assets/images/2023-03-07-15-38-10.png)

| 4) Set the **Type** to **Credential**. 
| ![](../assets/images/2023-03-07-15-37-39.png) 

| 5) Set the **Name** to `Pipeline Credentials` and click **Submit**.

*Click the clipboard icon on the right of the gray box below to copy.*

```markdown
Pipeline Credentials
```

| ![](../assets/images/2023-03-08-14-14-44.png)
| ![](../assets/images/2023-07-13-17-00-48.png)

| 6) Click **Pipeline Credentials** to open the record. 
|![](../assets/images/2023-03-09-13-48-09.png) 

| 7) Navigate to the **Credentials** Related List and click **New** to add a credential. 
|![](../assets/images/2023-03-09-13-49-03.png)

| 8) Select **Basic Auth Credentials**.
|![](../assets/images/2023-03-09-13-50-33.png)

{: .important}
> Next, you will be inputting credentials that App Engine Management Center will use to log in to a remote environment. 
>
> The password for that remote account is already configured. 
>
> You will encounter errors if you do not use the specified password below. 

| 9) On the **Basic Auth Credentials** form, fill in these values and click **Submit**. 

*Click the clipboard icon on the right of the gray box below to copy.*

```markdown
Pipeline Service Account
```
```markdown
svc_pipeline
```
```markdown
ILoveHyperAutomationTimes500!
```

|![](../assets/images/2023-06-27-22-50-59.png)

[Next](/lab-aemc-utah/docs/credentials-dev){: .btn .btn-green .fs-2}
