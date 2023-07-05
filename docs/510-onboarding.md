---
layout: default
parent: 5) Simulation
title: 5.1) Onboard a developer
nav_order: 510
nav_exclude: false
permalink: /docs/onboarding
---

# 5.1) Onboard a developer

{: .note-title}
> Sydney Carter
> <table>
> <tbody>
> <tr>
> <td>
> <img src="../assets/images/2023-03-28-15-52-55.png">
> </td>
> <td>
> Sydney Carter has been in IT for years in various roles.<br/>
> <br/>
> She wants to join her company's Citizen Developer Program.<br/>
> <br/>
> This section will show what that experience is like.
> </td>
> </tr>
> </tbody>
> </table>

| 1) In the top right, click the **System Administrator** avatar >> **Impersonate user**.
| ![](../assets/images/2023-03-14-12-31-53.png)

| 2) Type **Sydney Carter** and click **Sydney Carter** in the search results.
| ![](../assets/images/2023-03-14-12-34-01.png)

| 3) Click **Impersonate User**. 
| ![](../assets/images/2023-03-14-12-34-24.png)

| 4) Click **All** >> type **employee center** >> click **Employee Center** 
| ![](../assets/images/2023-07-05-10-07-57.png)

| 5) Click **IT for IT** 
| ![](../assets/images/2023-03-14-12-36-45.png)

| 6) Click **Apply for Citizen Development**
| ![](../assets/images/2023-03-14-12-37-08.png)

{: .highlight}
> This error message only appears for users logged in with the admin role even if impersonating.
>
> ![](../assets/images/2023-03-14-12-37-43.png)
>
> In the real world, users with the **admin** role would **not be** applying for citizen development. 

| 11) Fill out the form with the values below. 

| Field | Value 
|:---|:---
| Application Name | ```Request Time Off``` 
| Describe your idea | ```Allow users to request time off with approvals.```
| Is your process repeatable? | ```Yes```
| Do you have an email... ? | ```No```
| How many users... ? | ```>20```
| Does this involve... ? | ```No```
| Do you need data... ? | ```No```
| Who are the users... ? | ```Anyone in the IT Department```

| 12) Click **Submit**.

| 13) After the request is submitted, close the browser tab and return to the original browser tab. 

| 14) Click the avatar in the top-right, then click **Impersonate another user**.
| ![](../assets/images/2023-03-14-12-44-50.png)

| 15) Type **Jayne Nigel** and click **Jayne Nigel**.
| ![](../assets/images/2023-03-14-12-45-21.png)

| 16) Click **Impersonate user**.

{: .note-title}
> Jayne Nigel
> <table>
> <tbody>
> <tr>
> <td>
> <img src="https://creatorworkflowsnow.github.io/lab-aemc-utah/assets/images/2023-03-28-16-42-23.png">
> </td>
> <td>
> Jayne is our App Engine Admin that we configured earlier in Lab 1, Step 22.<br/>
> <br/>
> She is not a Platform Administrator.<br/>
> <br/>
> She is responsible for managing requests from App Engine Users.
> </td>
> </tr>
> </tbody>
> </table>

| 17) Click **All**.

| 18) Type **app engine management**.

| 19) Click **App Engine Management Center**.
| ![](../assets/images/2023-04-25-10-57-02.png)

{: .highlight}
> This will open AEMC in a new browser tab.

| 20) In the **Intake application requests** widget, click Sydney's request to open it. 
| ![](../assets/images/2023-03-14-12-49-13.png)

| 21) In the top right, click **Approve**.
| ![](../assets/images/2023-03-14-12-50-13.png)

{: .note}
> The Prod instance will attempt to configure Sydney's App Engine User access on the Dev environment.
>
> In the real world, there might be more than one person to do the approval and more time may be taken to review the answers.

| 22) Click **X** to close the RITM tab in AEMC.
| ![](../assets/images/2023-03-14-12-52-16.png)

**Congratulations!** 

Sydney is ready begin building her first app.

Jayne was able to configure Sydney's access **without** the admin role by clicking Approve on the request.

[Next](/lab-aemc-utah/docs/build-app){: .btn .btn-green .fs-2}