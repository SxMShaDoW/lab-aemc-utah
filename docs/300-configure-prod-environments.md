---
layout: default
parent: Implementation
title: 3) Configure Prod Environments
nav_order: 300
permalink: /docs/configure-prod-environments
---

# 3) Configure Environments in Prod Instance

<button class="btn btn-green fs-3" disabled>Estimated Time to Complete: 10 minutes</button>

## Overview 

[Environment records](https://docs.servicenow.com/csh?topicname=config-pipeline-environments.html&version=latest){:target="_blank"} <i class="fas fa-external-link-alt"></i> (`sn_pipeline_environment`) contain information about a ServiceNow instance and how to access it.

Environment records do not sync across instances so creation is required on all instances (production and sub-production).

Environment records are put together in a Pipeline to let App Engine Management Center know what path to promote applications to Production.

```mermaid
graph LR
    style Pipeline fill:#C5D6D8,stroke:#333,stroke-width:1px
    subgraph Pipeline
        style Dev fill:#FFCCCC,stroke:#333,stroke-width:2px
        style Prod fill:#CCFFCC,stroke:#333,stroke-width:2px
        Dev[Dev Environment] --> Prod[Prod Environment]
    end

```

{: .highlight}
> For this exercise, the specific Application Scope for the environments is not critical - Global is acceptable. Always check with your Platform Administrator for any company policies around **<a href="https://docs.servicenow.com/csh?topicname=connection-alias.html&version=latest" target="_blank">Connection and Credential Aliases ↗</a>**.
>
> Only users with the **System Administrator** (admin) role can define instance credentials for environments. 
> 
> Users with the **App Engine Administrator** (`sn_app_eng_notify.app_engine_admin`) role can view environment records; however, the Instance credential field is not visible.

## Instructions

{: .warning}
> **Complete this section in PROD.**

| 1) Log in to **Prod**.

| 2) Click **All** >> type **environment** >> click **Environments**
| ![](../assets/images/2023-06-30-15-17-33.png)

| 3) Click **New** in the top-right.
| ![](../assets/images/2023-06-30-15-19-10.png)

| 4) Complete the form as below.

| Field | Value 
|:---|:---
| Name | ```Dev``` 
| Instance Type | ```Development``` 
| Instance URL | ```The full URL of your Dev Lab instance (Ex. https://your-lab-123.service-now.com)``` 
| Instance credential | ```Pipeline_Credentials``` 
| Is Controller? | ```Leave unchecked``` 
| Instance Id | ```This will auto populate after clicking Validate.``` 

| 5) Click the "Validate" button. 
| ![](../assets/images/2023-07-11-15-38-49.png)

| ![](../assets/images/2023-07-11-15-14-18.png)

| You should see a blue message that says "The environment was validated successfully". 
| ![](../assets/images/2023-07-11-15-37-24.png)

| 6) Click **Submit** to finish creating the environment record.
| ![](../assets/images/2023-07-11-15-37-58.png)

**Congratulations!**
You have now created your **Dev Environment** record in your Prod instance.
 
---
Next, we will create the **Prod Environment** record on your Prod instance.  

## Create a Prod Environment Record (*in your Prod instance*)

| 7) Click **New** in the top right.
| ![](../assets/images/2023-06-30-15-19-10.png)

| 8) Complete the form as below.

| Field | Value 
|:---|:---
| Name | ```Prod``` 
| Instance Type | ```Production``` 
| Instance URL | ```The full URL of your Prod Lab instance (Ex. https://your-lab-123.service-now.com)``` 
| Instance credential | ```Pipeline_Credentials``` 
| Is Controller? | ```Checked``` 
| Instance Id | ```This will auto populate after clicking Validate.``` 

| 9) Click the "Validate" button. 
| ![](../assets/images/2023-07-11-15-38-49.png)

| You should see a blue or yellow message that says "*The controller environment was validated successfully*". 
| ![](../assets/images/2023-07-11-15-15-10.png)
| ![](../assets/images/2023-07-13-17-13-29.png)

| 10) Click **Submit** to finish creating the environment record.
| ![](../assets/images/2023-07-11-15-37-58.png)

## Lessons Learned

In this exercise, you have:

- Understood the function and importance of Environment records in the ServiceNow platform.
- Successfully configured Environment records for both Development and Production instances in your Prod environment.
- Acquired the knowledge of validating these Environment records.

[Next](/lab-aemc-utah/docs/configure-prod-pipeline){: .btn .btn-green .fs-2}