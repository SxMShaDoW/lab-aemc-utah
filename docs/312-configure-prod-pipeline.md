---
layout: default
grand_parent: 3) Pipelines & Deployments
parent: 3.1) Configure Prod
title: 3.1.2) Pipeline
nav_order: 330
permalink: /docs/configure-prod-pipeline
---

# 3.1.2) Configure Pipeline in Prod only

A pipeline defines the path an application takes from the development to production environments and allows administrators to quickly move applications across instances.

Set up and configure your pipeline by specifying the environments to include along with their position in the pipeline.

The Pipeline is only configured on the Controller Environment, which is the Production instance. 

{: .warning}
> Complete this section in **PROD**.

{: .highlight}
> *If you only have a **DEV** and **TEST** instance, then treat your **TEST** instance as if it were **PROD**.*

| 1) Click **All** >> type **pipelines** >> click **Pipelines** 
| ![](../assets/images/2023-06-30-15-31-49.png)

| 2) Click **New** in the top-right
| ![](../assets/images/2023-06-30-15-19-10.png)

| 3) Complete the form as below. Click Submit when complete.

| Field | Value 
|:---|:---
| Name | ```Main Pipeline``` 
| Pipeline Type | ```Application Deployment```
| Source Environment | ```Dev```
| Active | Checked

| ![](../assets/images/2023-06-30-15-34-56.png)

| 4) Click **Main Pipeline** to open the record.
| ![](../assets/images/2023-06-30-15-38-29.png)

| 5) In the **Pipeline Environments Order** related list, click **New**.
| ![](../assets/images/2023-06-30-15-40-02.png)

| 6) Complete the form as below. Click **Submit** when complete.

| Field | Value 
|:---|:---
| Pipeline | ```Main Pipeline``` 
| Environment | ```Prod```
| Order | ```100```

| ![](../assets/images/2023-06-30-15-42-05.png)

**Congratulations!** You have created a **Pipeline** in your Prod environment to deploy applications with!

{: .note}
> For more information see **[Product Documentation: Create a pipeline](https://docs.servicenow.com/csh?topicname=config-p-and-d.html&version=latest)**

[Next](/lab-aemc-utah/docs/configure-non-prod){: .btn .btn-green .fs-2}