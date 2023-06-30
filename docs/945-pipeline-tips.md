---
layout: default
title: Pipeline tips and tricks
parent: References
nav_order: 945
permalink: /docs/pipeline-tips
---

# Pipeline tips

Set up and configure the environments that will be included within your pipelines. These will be referenced when building your pipelines.

Your production instance is where your pipeline configurations reside and will be your controller instance.

The 'Is Controller?' box will be **checked** on your production instance only. This box will be **unchecked** for all sub-production Environment records.

If you have **more than one** Production environment, then AEMC will only be the controller on a single instance for all of your other Prods. 

{: .warning}
> If group membership is empty in the production instance, or if the Deployment Pipeline plugin is not installed, the system will refer to App Engine Studio Administrator group membership in the development instance.

{: .note}
> For more information, see **[Product Documentation: Create a pipeline](https://docs.servicenow.com/csh?topicname=create-pipeline.html)**

[Next](/lab-aemc-utah/docs/docs){: .btn .btn-green .fs-2}