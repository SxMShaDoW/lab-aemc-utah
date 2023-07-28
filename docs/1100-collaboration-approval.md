---
layout: default
parent: Simulation
title: 11) Approve Collaboration
nav_order: 1100
nav_exclude: false
permalink: /docs/collaboration-approval
---

# 11) Approve Collaboration

---

When Sydney submitted the Collaboration Request in App Engine Studio, it triggered an email to Jayne prompting her to take action. 

{: .important}
> **SUBJECT:** Developer Collaboration Task DEV0001002 Approval Request
> <table>
> <tbody>
> <tr>
> <td>
> <img src="https://creatorworkflowsnow.github.io/lab-aemc-utah/assets/images/2023-07-11-21-20-36.png">
> </td>
> </tr>
> </tbody>
> </table>

Jayne decides to log in to take a closer look before approving. 

{: .warning}
> Complete this section in **PROD**.

{: .highlight}
> You should still have a browser tab for **Prod** opened to App Engine Management Center in which you are impersonating Jayne. 
>
> If not, follow these quick instructions to be sure:
>
> 1) Click the avatar in the top-right, then click **Impersonate another user**.
>
> 2) Type **Jayne Nigel** and click **Jayne Nigel**.
>
> 3) Click **Impersonate user**.
>
> 4) Click **All** >> type **app engine management** >> click **App Engine Management Center**.
>
> This will open AEMC in a new browser tab.

| 1) Click **Overview** in App Engine Management Center
| ![](../assets/images/2023-07-11-20-33-36.png) 

| 2) Click the **1** above **Collaboration**
| ![](../assets/images/2023-07-11-20-33-05.png)

{: .warning}
> If there is no collaboration task, then the environment controller is probably misconfigured and the approval task got created in dev. Validate that the environment records (checkbox should be set to true for the production url) are setup correctly in both environments.

| 3) Click the **DEV** ticket to open Sydney's Collaboration request.
| ![](../assets/images/2023-07-11-20-35-33.png)

| 4) Click **Approve** in the top-right of the page. 
| ![](../assets/images/2023-07-11-16-56-47.png)
| ![](../assets/images/2023-07-11-17-01-13.png)

| 5) Click **Overview** to return to the main AEMC page.
| ![](../assets/images/2023-07-11-20-38-56.png)


After Jayne approved the Collaboration Request, Sydney received an email to inform her that the request was approved. 

{: .important}
> **SUBJECT:** Your collaborator request was approved
> <table>
> <tbody>
> <tr>
> <td>
> <img src="https://creatorworkflowsnow.github.io/lab-aemc-utah/assets/images/2023-07-11-21-05-07.png">
> </td>
> </tr>
> </tbody>
> </table>

**Great!!** Approving the request triggered AEMC to automatically provision Priya's access to work on the app with Sydney as an Integration Specialist.

{: .highlight}
> **Integration Specialist** is a custom **[Collaboration Descriptor](https://docs.servicenow.com/csh?topicname=create-collaboration-descriptors.html&version=latest)** created for this lab. 

[Next](/lab-aemc-utah/docs/configure-integration){: .btn .btn-green .fs-2}
