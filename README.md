# Cloud-Shell-GSP101-Google-Cloud-Essential-Skills-Challenge-Lab
Template project for a cloud shell tutorial  
DeleteMe- Find all sections that say DeleteMe, these should be deleted.  
ReplaceMe- Sections, keywords, id numbers that need to be replaced or personalized.  
VerifyMe/- Text thatmight apply for all instances but you might want to look to see if there is new information.  

ToDo List before going to production:
- [ ] Check for and note locations of VerifyMe 
- [ ] Check for and note locations of ReplaceMe 
- [ ] Check for and note locations of DeleteMe 
- [ ] Change GCP Lab number references
- [ ] Change Lab Title references
- [ ] Change Lab Quests references
- [ ] Change Overview references
- [ ] Change Objective references
- [ ] Change video references
- [ ] Change Get started references if there are specific details associated with this lab.
- [ ] First Run through
- [ ] Second Runthrough for ease of use
- [ ] Third Runthrough for special details and learn more references.
- [ ] Change or add lab verification links in Qwiklab documentation 
- [ ] Check for and delete VerifyMe 
- [ ] Check for ReplaceMe 
- [ ] Check for DeleteMe 
- [ ] Check for The Markup references at the end of the template and delete them.


Lab ID: GSP101

# Cloud-Shell-GSP101-Google-Cloud-Essential-Skills-Challenge-Lab
[Overview from Lab Guide]

[https://google.qwiklabs.com/focuses/7716?parent=catalog](https://google.qwiklabs.com/focuses/7716?parent=catalog)

This lab is also part of the [ReplChallenge: GCP Architecture](https://google.qwiklabs.com/quests/47) Quest


## Overview
For this Challenge Lab you must complete a series of tasks within a limited time period. Instead of following step-by-step instructions, you'll be given a scenario and task - you figure out how to to complete it on your own! An automated scoring system (shown on this page) will provide feedback on whether you have completed your tasks correctly.

To score 100% you must complete all tasks within the time period!

When you take a Challenge Lab, you will not be taught GCP concepts. You'll need to use your advanced Google Compute Engine (GCE) skills to assess how to build the solution to the challenge presented. This lab is only recommended for students who have GCE skills. Are you up for the challenge?


### Objectives
In this lab, you learn how to perform these tasks:
* Create a Linux Virtual Machine Instance
* Enable public access to VM instance
* Running basic Apache Web Server
* Test your server

ReplaceMeOjectives

### What you'll need
#### Setup
Before you click the Start Lab button
Read these instructions. Labs are timed and you cannot pause them. The timer, which starts when you click Start Lab, shows how long Cloud resources will be made available to you.

This Qwiklabs hands-on lab lets you do the lab activities yourself in a real cloud environment, not in a simulation or demo environment. It does so by giving you new, temporary credentials that you use to sign in and access the Google Cloud Platform for the duration of the lab.

The Google Chrome browser. Other browsers are currently not supported by some parts of GCP suckh as Cloud Dataprep.

To complete this lab, you need:
* Access to a standard internet browser (Chrome browser recommended).
* Time to complete the lab.  
Note: If you already have your own personal GCP account or project, do not use it for this lab.


### What you'll learn
Your challenge is to deploy the site in the public cloud by completing the tasks below. You will use a simple Apache web server as a placeholder for the new site in this exercise. Good luck!

Running a Basic Apache Web Server
A virtual machine instance on Google Compute Engine can be controlled like any standard Linux server. Deploy a simple Apache web server (a placeholder for the new product site) to learn the basics of running a server on a virtual machine instance.

### Here are some links: 
[Running a basic Apache web server](https://cloud.google.com/compute/docs/tutorials/basic-webserver-apache) A virtual machine instance on Google Compute Engine can be controlled like any standard Linux server. Deploy a simple Apache web server to learn the basics of running a server on a virtual machine instance.


### Here are videos for your use:  
[Google Compute Engine - Seven Minute Test Drive: Set Up your own Web Server](https://www.youtube.com/watch?v=BnEhYaUY4sA) This demonstration covers getting started with the Google Cloud Platform and Google Compute Engine. See the process of creating a project, starting up a cloud based virtual machine and installing a web server on it.  
[Hands on with Load Balancing on Google Compute Engine](https://www.youtube.com/results?search_query=%22Google+Cloud+Platform%22+%22cloud+dataprep%22)  
[Puppet and Google Compute Engine: a 10 minute video demo)](https://www.youtube.com/watch?v=YT_SuYX4vUI)  
[Learn how to scale your applications with Google Compute Engine (100 Days of Google Dev)](https://www.youtube.com/watch?v=TfbEwfYjKl4)  
[Google Compute Engine - Ten Minute Test Drive: Set Up your own Web Server](https://www.youtube.com/watch?v=LrjpcR-IJwY)  


### Get Started:
To begin the tutorial in a Qwiklab open your Google Cloud Consoles as you normally would.
1.  If you have issues with the console try using incognito mode and go to https://console.cloud.google.com/
2.  If you are in the student session of the GCP Console, click the Cloud Shell icn on the top right that looks like this: ![alt text](https://walkthroughs.googleusercontent.com/tutorial/resources/cloud-shell-icon-v1.svg "Cloud Shell Icon on the top right of the GCP Console")
3.  Enter the following commands to clone this repository and launch the turotial.
```bash
git clone https://github.com/ratokeshi/Cloud-Shell-GSPReplaceMeNumber-ReplaceMeName.git
&& cd Cloud-Shell-GSPReplaceMeNumber-ReplaceMeFolder && cloudshell launch-tutorial tutorial.md
```

```bash
gcloud config configurations create qwiklab-$(date +%s)
gcloud config unset project
gcloud auth login <google5150507_student@qwiklabs.net>
gcloud config set project <from Lab>
cloudshell launch-tutorial tutorial.md
```


To begin the tutorial in your currently authenticated Google account, click on the button given below:
[![Open in Cloud Shell](http://gstatic.com/cloudssh/images/open-btn.png)](https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/ratokeshi/Cloud-Shell-GSPReplaceMeNumber-ReplaceMeFolder.md)
