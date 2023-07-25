---
layout: default
parent: Implementation
title: 2a) Create Credentials in Prod
nav_order: 200
permalink: /docs/credentials-prod
---

# 2a) Create Credentials in Prod

<button class="btn btn-green fs-3" disabled>Estimated Time to Complete: 10 minutes</button>

## Overview 

In this exercise, you will configure **Service Account Credentials**. These credentials allow App Engine Management Center to communicate with the environments in the pipeline.

{: .highlight}
> For this exercise, the specific Application Scope for the credentials is not critical - Global is acceptable. Always check with your Platform Administrator for any company policies around **<a href="https://docs.servicenow.com/csh?topicname=connection-alias.html&version=latest" target="_blank">Connection and Credential Aliases ↗</a>**.

## Instructions

| 1) Log in to **PROD**.

| 2) Click **All**, then type **Connection & Credential Aliases** in the search box, and click the SECOND **Connection & Credential Aliases** that appears in the drop-down list.
| ![Navigate to Aliases](../assets/images/2023-07-11-15-10-23.png)

| 3) Click the purple **New** button in the top-right to create a new Credential Alias record. 
| ![Create Alias](../assets/images/2023-03-07-15-38-10.png)

| 4) Set the **Type** to **Credential**. 
| ![Set Type](../assets/images/2023-03-07-15-37-39.png) 

| 5) Set the **Name** to `Pipeline Credentials` and click **Submit**.
| ![Set Name](../assets/images/2023-03-08-14-14-44.png)
| ![Submit Name](../assets/images/2023-07-13-17-00-48.png)

| 6) Click **Pipeline Credentials** to open the record. 
| ![Open Record](../assets/images/2023-03-09-13-48-09.png) 

| 7) Navigate to the **Credentials** Related List and click **New** to add a credential. 
| ![Add Credential](../assets/images/2023-03-09-13-49-03.png)

| 8) Select **Basic Auth Credentials**.
| ![Select Basic Auth](../assets/images/2023-03-09-13-50-33.png)

{: .important}
> You will now input credentials for the App Engine Management Center to use when logging into a remote environment. The password for this remote account is pre-configured. Errors will occur if you do not use the specified password provided below. 

| 9) On the **Basic Auth Credentials** form, fill in the following values and click **Submit**.

**Use the clipboard icon on the right of the gray box below to conveniently copy the values for pasting.**

```markdown
Pipeline Service Account
```
```markdown
svc_pipeline
```
```markdown
ILoveHyperAutomationTimes500!
```

| ![Enter Credentials](../assets/images/2023-06-27-22-50-59.png)

## Lessons Learned

By completing this exercise, you've accomplished the following:
- Created a Service Account Credential in the Prod environment.
- Added a Basic Auth Credential to this account.

[Next](/lab-aemc-utah/docs/credentials-dev){: .btn .btn-green .fs-2}