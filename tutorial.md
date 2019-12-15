# GSP101 -- Tutorial: Google Cloud Essential Skills: Challenge Lab

## Overview
For this Challenge Lab you must complete a series of tasks within a limited time period. Instead of following step-by-step instructions, you'll be given a scenario and task - you figure out how to to complete it on your own! An automated scoring system (shown on this page) will provide feedback on whether you have completed your tasks correctly.

To score 100% you must complete all tasks within the time period!

When you take a Challenge Lab, you will not be taught GCP concepts. You'll need to use your advanced Google Compute Engine (GCE) skills to assess how to build the solution to the challenge presented. This lab is only recommended for students who have GCE skills. Are you up for the challenge?

### Objectives ###
Topics tested
Create a Linux Virtual Machine Instance

* Enable public access to VM instance
* Running basic Apache Web Server
* Test your server 

## Prerequisites VerifyMe##

 -  You have a Google Cloud Platform account and a Google Project (note the Google Project Id) provided by Quiklab. You can find this on the left side of the QwikLab page.
 -  The [Google Chrome browser](https://www.google.com/chrome/browser/desktop/). Other browsers are currently not supported by Cloud Dataprep.
 
 
### Task 1. Setting up your development environment ##
#### Qwiklab
##### Before you click the Start Lab button
Read these instructions. Labs are timed and you cannot pause them. The timer, which starts when you click Start Lab, shows how long Cloud resources will be made available to you.

This Qwiklabs hands-on lab lets you do the lab activities yourself in a real cloud environment, not in a simulation or demo environment. It does so by giving you new, temporary credentials that you use to sign in and access the Google Cloud Platform for the duration of the lab.

#### What you need
To complete this lab, you need:

Access to a standard internet browser (Chrome browser recommended).
Time to complete the lab.
Note: If you already have your own personal GCP account or project, do not use it for this lab.

#### Setting up Google Cloud Platform Console
##### How to start your lab and sign in to the Console

1. Click the Start Lab button. If you need to pay for the lab, a pop-up opens for you to select your payment method. On the left is a panel populated with the temporary credentials that you must use for this lab.  


Note: You can view the menu with a list of GCP Products and Services by clicking the Navigation menu at the top-left, next to “Google Cloud Platform”.
<walkthrough-spotlight-pointer spotlightId="devshell-web-preview-button"
                               text="Open Web Preview">
</walkthrough-spotlight-pointer>
![](https://cdn.qwiklabs.com/a6YnJv8GlGae4rnJIbjA27J8c7YApa%2B6noPFkkKxZjk%3D)

- Verify current account from QwikLab
```bash
gcloud auth list
```

- Check your current project.
```bash
gcloud config list project
```
Your current project name is: {{<project-name>}}  
Your current project id is: {{<project-id>}}  
 Be sure to compare this to the display in your Qwiklab after you start the lab. The display looks like this:  
 ![Login Info](https://cdn.qwiklabs.com/%2FtHp4GI5VSDyTtdqi3qDFtevuY014F88%2BFow%2FadnRgE%3D)  
 
1. Copy the username, and then click Open Google Console. The lab spins up resources, and then opens another tab that shows the Choose an account page.

Tip: Open the tabs in separate windows, side-by-side.

1. On the Choose an account page, click Use Another Account.  
 ![Login Info](https://cdn.qwiklabs.com/eQ6xPnPn13GjiJP3RWlHWwiMjhooHxTNvzfg1AL2WPw%3D) 
 
1.   The Sign in page opens. Paste the username that you copied from the Connection Details panel. Then copy and paste the password.

Important: You must use the credentials from the Connection Details panel. Do not use your Qwiklabs credentials. If you have your own GCP account, do not use it for this lab (avoids incurring charges).

1. Click through the subsequent pages:

Accept the terms and conditions.
Do not add recovery options or two-factor authentication (because this is a temporary account).
Do not sign up for free trials.
After a few moments, the GCP console opens in this tab.
Note: You can view the menu with a list of GCP Products and Services by clicking the Navigation menu at the top-left, next to “Google Cloud Platform”.
![Hamburger](https://cdn.qwiklabs.com/9vT7xPlxoNP%2FPsK0J8j0ZPFB4HnnpaIJVCDByaBrSHg%3D)  
Open the Navigation Menu Icon
<walkthrough-nav-menu-icon>
</walkthrough-nav-menu-icon>
<walkthrough-spotlight-pointer
    spotlightId="nav-menu-icon">
    spotlight on the nav menu icon
</walkthrough-spotlight-pointer>

#### Activate Google Cloud Shell
Google Cloud Shell is a virtual machine that is loaded with development tools. It offers a persistent 5GB home directory and runs on the Google Cloud. Google Cloud Shell provides command-line access to your GCP resources.   

1.  In GCP console, on the top right toolbar, click the Open Cloud Shell button.
ReplaceMeBelow - Below is an example imagefrom the Qwiklab site.
![](https://cdn.qwiklabs.com/vdY5e%2Fan9ZGXw5a%2FZMb1agpXhRGozsOadHURcR8thAQ%3D)  

Task 2. Click Continue.
![](https://cdn.qwiklabs.com/lr3PBRjWIrJ%2BMQnE8kCkOnRQQVgJnWSg4UWk16f0s%2FA%3D)

It takes a few moments to provision and connect to the environment. When you are connected, you are already authenticated, and the project is set to your PROJECT_ID. For example:

![](https://cdn.qwiklabs.com/hmMK0W41Txk%2B20bQyuDP9g60vCdBajIS%2B52iI2f4bYk%3D)  
gcloud is the command-line tool for Google Cloud Platform. It comes pre-installed on Cloud Shell and supports tab-completion.

You can list the active account name with this command:

```bash
gcloud auth list
``` 
Output:  
```bash
Credentialed accounts:
 - <myaccount>@<mydomain>.com (active)
```

Example output:

```bash
Credentialed accounts:
 - google1623327_student@qwiklabs.net
```
You can list the project ID with this command:

gcloud config list project

Output:

[core]
project = <project_ID>

Task 3. Challenge scenario
Your company is ready to launch a brand new product! Because you are entering a totally new space, you have decided to deploy a new website as part of the product launch. The new site is complete, but the person who built the new site left the company before they could deploy it.


Your challenge
Your challenge is to deploy the site in the public cloud by completing the tasks below. You will use a simple Apache web server as a placeholder for the new site in this exercise. Good luck!

Running a Basic Apache Web Server
A virtual machine instance on Google Compute Engine can be controlled like any standard Linux server. Deploy a simple Apache web server (a placeholder for the new product site) to learn the basics of running a server on a virtual machine instance.

Create a Linux VM Instance
Create a Linux virtual machine, name it "apache" and specify the zone as "us-central1-a".

Enable Public Access to VM Instance
While creating the Linux instance, make sure to apply the appropriate firewall rules so that potential customers can find your new product.

Click Check my progress to verify the objective.

Create a Compute Engine instance, add necessary firewall rules.
Running a Basic Apache Web Server
A virtual machine instance on Google Compute Engine can be controlled like any standard Linux server. Deploy a simple Apache web server (a placeholder for the new product site) to learn the basics of running a server on a virtual machine instance.

Click Check my progress to verify the objective.

Add Apache2 HTTP Server to your instance
Test Your Server
Test that your instance is serving traffic on its external IP. You should see the "Hello World!" page (a placeholder for the new product site).

Click Check my progress to verify the objective.

Test your server
Troubleshooting
Receiving a Connection Refused Error:

Your VM instance is not publicly accessible because the VM instance does not have the proper tag that allows Compute Engine to apply the appropriate firewall rules, or your project does not have a firewall rule that allows traffic to your instance's external IP address.
You are trying to access the VM using an https address. Check that your URL is http:// EXTERNAL_IP and not https:// EXTERNAL_IP

Congratulations!
You've successfully explored your ecommerce dataset and created a recurring data transformation pipeline with Cloud Dataprep.

Go back to the Qwicklabs page to verify the lab shows as complete.

<walkthrough-conclusion-trophy></walkthrough-conclusion-trophy>