---
layout: default
title: 8) Approve development
nav_order: 800
nav_exclude: false
permalink: /docs/intake-approval/
---

# 8) Approve Developer Intake Requests

---

In this section, our **App Engine Admin** Jayne will review and approve Sydney's App Intake request. 

{: .note-title}
> Jayne Nigel
> <table>
> <tbody>
> <tr>
> <td>
> <img src="https://creatorworkflowsnow.github.io/lab-aemc-utah/assets/images/Jayne_Nigel.png" />
> </td>
> <td>
> Jayne is the App Engine Admin.<br/>
> <br/>
> She is not a Platform Administrator and does not have the 'admin' role in any environment.<br/>
> <br/>
> She is responsible for managing requests from App Engine Users. Her approvals will trigger automation to provision user access, deploy apps to environments, and other activities. 
> </td>
> </tr>
> </tbody>
> </table>

When Sydney submitted her Intake Request it triggered an email to Jayne to let her know to take action. 

{: .important}
> **SUBJECT:** Please select user permission type for a new app request
> <table>
> <tbody>
> <tr>
> <td>
> <img src="https://creatorworkflowsnow.github.io/lab-aemc-utah/assets/images/2023-07-11-21-08-36.png">
> </td>
> </tr>
> </tbody>
> </table>

| 1) Click the avatar in the top-right, then click **Impersonate another user**.
| ![](../assets/images/2023-03-14-12-44-50.png)

| 2) Type **Jayne Nigel** and click **Jayne Nigel**.
| ![](../assets/images/2023-03-14-12-45-21.png)

| 3) Click **Impersonate user**.
| 4) Click **All** >> type **app engine management** >> click **App Engine Management Center**.
| ![](../assets/images/2023-07-05-16-16-55.png)

{: .highlight}
> This will open AEMC in a new browser tab.

| 5) In the **Pending requests to complete** widget, click the number **1** above **Intake** to open Sydney's request. 
| ![](../assets/images/2023-07-11-16-34-50.png)

| 6) Click the **RITM** number to open Sydney's request.
| ![](../assets/images/2023-07-11-16-36-33.png)

| 7) Scroll down the left-hand side of the page in the **Details** section.
|![](../assets/images/2023-07-11-16-39-06.png)

| 8) In the **Administration** section of the form, click on the **Permission type** drop-down field.
| ![](../assets/images/2023-07-11-16-42-31.png)

| 9) Click on **Create/edit applications (AES User Group)**
| ![](../assets/images/2023-07-11-16-44-56.png)

| 10) Scroll to the top of the page and click **Save** in the top right. 
| ![](../assets/images/2023-07-11-16-46-15.png)

| 11) Click on the **Catalog Tasks (1)** related list. 
| ![](../assets/images/2023-07-11-16-47-20.png)

| 12) Click the **SCTASK** number to open the Catalog Task.
| ![](../assets/images/2023-07-11-16-47-55.png)

| 13) Click **Close Task** in the top-right.
| ![](../assets/images/2023-07-11-16-49-14.png)

| 14) Click the i circle next to the **RITM** number to go back to the **RITM** record. 
| ![](../assets/images/2023-07-11-16-54-30.png)

| 15) Click **Approve** in the top-right of the page. 
| ![](../assets/images/2023-07-11-16-56-47.png)
| ![](../assets/images/2023-07-11-17-01-13.png)

{: .note}
> The Prod instance will attempt to configure Sydney's App Engine User access on the Dev environment.
>
> In the real world, there might be more than one person to do the approval and more time may be taken to review the answers.
>
> You may also want to require the person to undergo additional training before approving their access to build applications. 


![](../assets/images/2023-07-11-21-13-17.png)

{: .important}
> **SUBJECT:** Request REQ0010005 was approved
> <table>
> <tbody>
> <tr>
> <td>
> <img src="https://creatorworkflowsnow.github.io/lab-aemc-utah/assets/images/2023-07-11-21-14-08.png)">
> </td>
> </tr>
> </tbody>
> </table>

**Congratulations!** 

Sydney is ready begin building her first app.

Jayne was able to configure Sydney's access **without** the need for the admin role.

[Next](/lab-aemc-utah/docs/build-app){: .btn .btn-green .fs-2}