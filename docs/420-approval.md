---
layout: default
parent: 4) Simulation
title: 4.2) Approval
nav_order: 420
nav_exclude: false
permalink: /docs/approval/
---

# 4.2) Review and Approve Developer Requests

| 1) Click the avatar in the top-right, then click **Impersonate another user**.
| ![](../assets/images/2023-03-14-12-44-50.png)

| 2) Type **Jayne Nigel** and click **Jayne Nigel**.
| ![](../assets/images/2023-03-14-12-45-21.png)

| 3) Click **Impersonate user**.

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
> She is responsible for managing requests from App Engine Users, which will trigger automated testing and deployments. 
> </td>
> </tr>
> </tbody>
> </table>

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

{: .note}
> The Prod instance will attempt to configure Sydney's App Engine User access on the Dev environment.
>
> In the real world, there might be more than one person to do the approval and more time may be taken to review the answers.

| 9) Click **X** to close the RITM tab in AEMC.

**Congratulations!** 

Sydney is ready begin building her first app.

Jayne was able to configure Sydney's access **without** the admin role by clicking Approve on the request.

[Next](/lab-aemc-utah/docs/build-app){: .btn .btn-green .fs-2}