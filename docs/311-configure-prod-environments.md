---
layout: default
grand_parent: 3) Pipelines & Deployments
parent: 3.1) Configure Prod
title: 3.1.1) Environments
nav_order: 320
permalink: /docs/configure-prod-environments
---

# 3.1.1) Configure Prod Environments 

*Environment ```[sn_pipeline_environment]``` records contain information about a ServiceNow instance and how to access it. Together, they make up a pipeline.*

*You must first configure the environment records before the pipeline can be setup. Environment records do not sync across instances so creation is required on all instances (production and sub-production).*

{: .highlight}
> In this section, you will configure environments for your pipeline on your **Prod** instance.
> 
> *If you only have a **DEV** and **TEST** instance, then treat your **TEST** instance as if it were **PROD**.*

## Create a Dev Environment Record (in your Prod instance)

{: .warning}
> Complete this section in **PROD**.
>
> The Environment records will function fine in any scope, but we recommend changing to the **Deployment Pipeline** scope before continuing. 

| 1) Click **All** >> type **environment** >> click **Environments** 
| ![](../assets/images/2023-06-30-15-17-33.png)

| 2) Click **New** in the top-right
| ![](../assets/images/2023-06-30-15-19-10.png)

| 3) Complete the form as below and click the "Validate" button. 

| Field | Value 
|:---|:---
| Name | ```Dev``` 
| Instance Type | ```Development``` 
| Instance URL | ```The full URL of your Dev Lab instance (Ex. https://your-lab-123.service-now.com)``` 
| Instance credential | ```sn_deploy_pipeline.Pipeline_Credentials``` 
| Is Controller? | ```Leave unchecked``` 
| Instance Id | ```This will auto populate after clicking Validate.``` 

| ![](../assets/images/2023-03-09-15-32-08.png) 

| You should see a blue message that says "The environment was validated successfully". 
|![](../assets/images/2023-03-09-15-51-38.png)

| 4) Click **Submit** to finish creating the '*Dev*' environment record.

***You have now created your Dev Environment record in your Prod instance.***

## Create a Prod Environment Record (in your Prod instance)

| 5) Click **New** in the top right.
| ![](../assets/images/2023-06-30-15-19-10.png)

| 6) Complete the form as below and click the 'Validate' button.

| Field | Value 
|:---|:---
| Name | ```Prod``` 
| Instance Type | ```Production``` 
| Instance URL | ```The full URL of your Prod Lab instance (Ex. https://your-lab-123.service-now.com)``` 
| Instance credential | ```sn_deploy_pipeline.Pipeline_Credentials``` 
| Is Controller? | ```Checked``` 
| Instance Id | ```This will auto populate after clicking Validate.``` 

| ![](../assets/images/2023-06-30-15-26-16.png)

| You should see a blue message that says "*The controller environment was validated successfully*". 
| ![](../assets/images/2023-03-12-17-05-44.png)

| 23) Click **Submit** to finish creating the '*Prod*' environment record.
| ![](../assets/images/2023-03-12-16-59-46.png)

That completes setup of your Environment records in the Prod environment.

Next up, you will configure the Pipeline in the Prod environment.

{: .note}
> For more information see **[Product Documentation: Define environments](https://docs.servicenow.com/csh?topicname=create-environment.html)**

[Next](/lab-aemc-utah/docs/configure-prod-pipeline){: .btn .btn-green .fs-2}