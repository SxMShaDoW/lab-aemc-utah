---
layout: default
title: 12) Configure Integration
nav_order: 1200
nav_exclude: false
permalink: /docs/configure-integration
---

# 12) Configure Integration

In this section, Priya will go to **Dev** and work on Sydney's app.

{: .note-title}
> Priya Bapat
> <table>
> <tbody>
> <tr>
> <td>
> <img src="https://creatorworkflowsnow.github.io/lab-aemc-utah/assets/images/Priya_Bapat.png" />
> </td>
> <td>
> Priya has many years in IT building integrations on various Platforms.<br/>
> <br/>
> She recently completed some Integration training on ServiceNow and is ready to assist Sydney.<br/>
> </td>
> </tr>
> </tbody>
> </table>

After Jayne approved the Collaboration Request, Priya received an email that she is now a collaborator on the app.

{: .important}
> **SUBJECT:** You are now a collaborator
> <table>
> <tbody>
> <tr>
> <td>
> <img src="https://creatorworkflowsnow.github.io/lab-aemc-utah/assets/images/2023-07-11-20-59-36.png">
> </td>
> </tr>
> </tbody>
> </table>


{: .note-title}
> Priya Bapat
> <table>
> <tbody>
> <tr>
> <td>
> <img src="https://creatorworkflowsnow.github.io/lab-aemc-utah/assets/images/Priya_Bapat.png" />
> </td>
> <td>
> She clicks the button in the email to go to App Engine Studio...<br/>
> </td>
> </tr>
> </tbody>
> </table>

{: .warning}
> Complete this section in **DEV**.

| 1) Go to your **Dev** instance.

| 2) In the top right, click the user avatar icon » **Impersonate another user**.
| ![](../assets/images/2023-07-11-20-50-38.png)

| 3) Type **Priya** and click **Priya Bapat** in the search results.
|![](../assets/images/2023-07-11-20-56-14.png)

| 4) Click **Impersonate User**. 
| ![](../assets/images/2023-03-14-12-34-24.png)

| 5) Click **All** » type ```app engine``` » click **App Engine Studio**
| ![](../assets/images/2023-07-11-17-18-49.png)

{: .highlight}
> This will open AES in a new browser tab.

| 6) Click **My Apps** 
| ![](../assets/images/2023-07-11-21-26-37.png)

| 7) Click on the **IT Time Off Request** app
| ![](../assets/images/2023-07-11-21-27-20.png)

| 8) Note some of the differences in Priya's experience versus Sydney's. She does not have access to the **Submit** button to request to deploy the app.  She also can not see or modify any of the **Experiences** in the app. 
| ![](../assets/images/2023-07-11-21-29-13.png)

| 9) Scroll down and click **+Add** next to **Logic and Automation**.
| ![](../assets/images/2023-07-11-21-31-14.png)

| 10) Click **Flow**
| ![](../assets/images/2023-07-11-21-31-35.png)

| 11) Click **Build from scratch**
![](../assets/images/2023-07-11-21-31-59.png)

| 12) Enter ```Send data to Workday``` in the **Name** field and click **Continue**
| ![](../assets/images/2023-07-11-21-34-10.png)
| ![](../assets/images/2023-07-11-21-34-43.png)

| 13) Click **Edit this flow**
| ![](../assets/images/2023-07-11-21-35-23.png)

| 14) Click **Add a trigger**
| ![](../assets/images/2023-07-11-21-36-31.png)

| 15) Click **Updated**
| ![](../assets/images/2023-07-11-21-37-01.png)

| 16) In the **Condition** field, type ```time off``` and click the **Time Off Request** table.
| ![](../assets/images/2023-07-11-21-37-53.png)

| 17) Click **Add filters** next to **Condition**
| ![](../assets/images/2023-07-11-21-45-26.png)

| 18) Configure a condition of **Active changes to false**
| ![](../assets/images/2023-07-11-21-47-04.png)

| 19) Click **Done**
| ![](../assets/images/2023-07-11-21-38-16.png)

| 20) Click **Add an Action, Flow Logic, or Subflow**
| ![](../assets/images/2023-07-11-21-38-51.png)

| 21) Click **Action** >> type ```log``` >> click **Log**
| ![](../assets/images/2023-07-11-21-43-05.png)

| 22) Type something in the **Message** field and click **Done**
| ![](../assets/images/2023-07-11-21-44-16.png)

| 23) Click **Save** in the top-right
| ![](../assets/images/2023-07-11-21-44-55.png)
| ![](../assets/images/2023-07-11-21-47-29.png)

| 24) Click **Activate** >> **Activate**
| ![](../assets/images/2023-07-11-21-48-02.png)
| ![](../assets/images/2023-07-11-21-48-50.png)

| 25) Click the **App Engine Studio** browser tab and return to the **Dev** platform view.
| ![](../assets/images/2023-07-11-21-52-42.png)

**Congrats!!** 

Priya has built an integration in the app. It is simplistic for the lab, but in a real world scenario she would build a more complex integration for Sydney. 

She sends a MS Teams message to Sydney letting her know that the integration portion of the app development is completed. 

The app is now ready for Sydney to request it to be deployed. 

[Next](/lab-aemc-utah/docs/deployment-request){: .btn .btn-green .fs-2}