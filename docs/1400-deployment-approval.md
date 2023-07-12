---
layout: default
title: 14) Approve Deployment
nav_order: 1400
nav_exclude: false
permalink: /docs/deployment-approval
---

# 14) Approve and Deploy Sydney's App

{: .note-title}
> Jayne Nigel
> <table>
> <tbody>
> <tr>
> <td>
> <img src="https://creatorworkflowsnow.github.io/lab-aemc-utah/assets/images/2023-03-28-16-42-23.png">
> </td>
> <td>
> Jayne is familiar many different software methodologies such as Agile and SAFe.<br/> 
> <br/>
> She is familiar with Update Sets from her ServiceNow training, but she does not regularly work with them.<br/>
> <br/>
> How will she deploy Sydney's app?
> </td>
> </tr>
> </tbody>
> </table>

When Sydney submitted the Deployment Request in App Engine Studio, it triggered an email to Jayne prompting her to take action.

{: .important}
> **SUBJECT:** Developer Collaboration Task DEV0001002 Approval Request
> <table>
> <tbody>
> <tr>
> <td>
> <img src="https://creatorworkflowsnow.github.io/lab-aemc-utah/assets/images/2023-07-11-22-07-39.png">
> </td>
> </tr>
> </tbody>
> </table>

{: .warning}
>This section is to be completed in your **Production** instance where AEMC is running. That is your controller instance. 

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


| ![](../assets/images/2023-07-11-22-12-55.png)

| 1) In the **Deployment requests** widget, click the new Deployment request number. 
| ![](../assets/images/2023-03-15-14-12-49.png)

| 9) Review the fields on the form to see the values that Sydney submitted. 

| 10) Click **Approve**.
| ![](../assets/images/2023-03-15-14-15-20.png)
| ![](../assets/images/2023-03-15-14-15-47.png)

***Go take a five minute break or stretch.  It can take several minutes or more for the app to deploy to the next environment.***

| 11) To check the status of the Deployment... 

| 12) Click the related list **Deployment Environment R..**
| ![](../assets/images/2023-03-15-14-17-35.png)

| 13) Click the refresh button to refresh this list. 

| 14) Eventually, you will see a record appear for your deployment. 
| ![](../assets/images/2023-03-15-14-18-20.png)

| 15) If **Has Error** is **false**, then the app deployed successfully to the next environment. 

| 16) If you have more than two instances in the pipeline, you will need to perform an approval for each environment after Dev. 

***How can you confirm if the app actually deployed?***

| 17) Click **All**.

| 18) Type **My Company Applications**.

| 19) Click **My Company Applications**.
| ![](../assets/images/2023-03-15-14-20-14.png)

{: .note}
> My Company Applications shows you the applications that have been published to your company's App Repo. 
>
> For more information see **[Product docs: ServiceNow application repository](https://docs.servicenow.com/csh?topicname=app-repo.html&version=latest)**

| 20) You should see the application installed. 
| ![](../assets/images/2023-03-15-14-23-44.png)

**Congratulations!**  

You have made it!! You deployed an app with the click of a button!

[Next](/lab-aemc-utah/docs/optional-setup-tasks){: .btn .btn-green .fs-2}