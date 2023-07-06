---
layout: default
parent: 5) Simulation
title: 5.2) Onboard a developer
nav_order: 520
nav_exclude: false
permalink: /docs/approval/
---

# 5.2) Approval

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
| ![](../assets/images/2023-07-05-16-17-25.png)
| ![](../assets/images/2023-03-14-12-44-50.png)

{: .highlight}
> This will open AEMC in a new browser tab.

| 7) In the **Intake application requests** widget, click Sydney's request to open it. 
| ![](../assets/images/2023-03-14-12-49-13.png)

| 8) In the top right, click **Approve**.
| ![](../assets/images/2023-03-14-12-50-13.png)

{: .note}
> The Prod instance will attempt to configure Sydney's App Engine User access on the Dev environment.
>
> In the real world, there might be more than one person to do the approval and more time may be taken to review the answers.

| 9) Click **X** to close the RITM tab in AEMC.
| ![](../assets/images/2023-03-14-12-52-16.png)

**Congratulations!** 

Sydney is ready begin building her first app.

Jayne was able to configure Sydney's access **without** the admin role by clicking Approve on the request.

[Next](/lab-aemc-utah/docs/build-app){: .btn .btn-green .fs-2}