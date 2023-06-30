---
layout: default
grand_parent: 3) Pipelines & Deployments
parent: 3.1) Configure Prod
title: 3.1.2) Pipeline
nav_order: 330
permalink: /docs/configure-prod-pipeline
---

# 3.1.2) Configure Prod Pipeline

Pipelines enable you to automate the propagation and installation of your applications from one instance to another. Pipelines are powered by the **[ServiceNow CI / CD spoke](https://docs.servicenow.com/csh?topicname=cicd-spoke-1.html&version=latest)**, which enables you to automate processes such as publishing applications to the **[application repository](https://docs.servicenow.com/csh?topicname=app-repo.html&version=latest)**, installing them on target instances, and running **[ATF tests](https://docs.servicenow.com/csh?topicname=automated-test-framework.html&version=latest)** and/or **[instance scans](https://docs.servicenow.com/csh?topicname=hs-landing-page.html&version=latest)**.

Pipeline and deployment setup activities do not sync across instances and pipeline configuration activities are required on all instances (production and sub-production).

In the **production** instance, complete the following steps to configure environments and deployment pipelines to streamline your application deployment process.

# Configure pipelines in production

A pipeline defines the path an application takes from the development to production environments and allows administrators to quickly move applications across instances.

Set up and configure your pipeline by specifying the environments to include along with their position in the pipeline.

| 1) In the '*Configure pipelines*' section click **Configure**. 
| ![](../assets/images/2023-03-12-17-25-15.png)

| 2) Click **New**.
| ![](../assets/images/2023-03-12-17-27-31.png)

| 3) Complete the form as below. Click Submit when complete.

| Field | Value 
|:---|:---
| Name | ```My first pipeline``` 
| Pipeline Type | ```Application Deployment```
| Source Environment | ```Dev```
| Active | Checked

{: .note}
> Once a pipeline has been created, use the **Pipeline Environments Order** Related List on the Pipeline record to configure the instance order for the pipeline. 
> 
> Create a record in the related list for all instances ***except*** the development instance and specify the environment's order within the pipeline.
>
> Application movement across pipelines is dictated by the order of the environments in the Pipeline Environment Order related list, and applications are promoted based on ascending 'Order' values.
>
> Be sure the environment order is consistent with the defined instance strategy. The production instance should have the highest 'Order' value *(i.e., Testing: 100, Staging: 200, Production: 300).
>

| 4) Click **My first pipeline** to open the record.
| ![](../assets/images/2023-03-12-17-31-52.png)

| 5) In the **Pipeline Environments Order** related list, click **New**.
| ![](../assets/images/2023-03-12-17-32-31.png)

| 6) Complete the form as below. Click **Submit** when complete.

| Field | Value 
|:---|:---
| Pipeline | ```My first pipeline``` 
| Environment | ```Production```
| Order | ```100```

{: .note}
> Since the development environment is already identified as the 'Source Environment' on the pipeline record, a pipeline environment order related record is not required.

| 7) Click **X** to close the modal.
| ![](../assets/images/2023-03-12-17-34-44.png)

| 8) In the '*Configure Pipelines*' section click **Mark as Complete**.
| ![](../assets/images/2023-03-12-17-35-33.png) 

**Congratulations!** You have created a new **Pipeline** in your Prod environment. 

Next, we will configure the **AES Admins** group in Prod. 

{: .note}
> For more information, see **[Product Documentation: Create a pipeline](https://docs.servicenow.com/csh?topicname=create-pipeline.html)**.

[Next](/lab-aemc-utah/docs/configure-prod-aes-admin){: .btn .btn-green .fs-2}