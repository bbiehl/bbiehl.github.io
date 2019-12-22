---
layout: post
title:  "What I learned in 2019"
date:   2019-12-22 06:00:00 -0500
categories: post
---

### 22 Dec
- Patched a serialize-javascript moderate security vulnerability. `npm i serialize-javascript`
- Found more vulnerabilities...

```
$ npm audit

                       === npm audit security report ===

found 7 vulnerabilities (3 moderate, 4 high) in 903739 scanned packages
  run `npm audit fix` to fix 7 of them.
```
- Fix action...

```
$ npm audit fix

                       === npm audit security report ===

found 0 vulnerabilities
 in 906331 scanned packages
```
- A definition for middleware that isn't confusing. *"A middleware component sits between the client and the server, processing inbound requests and outbound responses, but it's more than interface that can be used to talk to web server. It's used to group and order modules, which are usually Ruby classes, and specify dependency between them."*

### 20 Dec
* I have not spent much time reviewing [The Ruby Style Guide](https://rubystyle.guide/), but most of the time I appear to be getting it right by accident.

### 18 Dec
* How to think about addiction differently.

### 17 Dec
* The best way to set up a DNS for a serverless app that is deployed to AWS Amplify, but registered with GoDaddy. *Hint: Use AWS R53*
* How to check hg logs for recent changesets `hg log | head -10`
* How to ignore changes to a tracked file in git. `git update-index --assume-unchanged FILEPATH`

### 6 Dec
* Bridging the chasm, how to know if you have product market fit.
* Your first users it should be early adapters. They will tell their friends. 
* Your next, and biggest group of users will be the pragmatist, also known as the early majority.
* Your last group of users will be the conservatives, the late majority.
* Laggards are the last group, and they will never adapt.

### 5 Dec
* Linux PATH is an environmental variable that tells the shell which directories to search for executable files in response to commands issued by the user. 
* A Linux shell is a program that takes commands from the keyboard and gives them to the operating system. 
a terminal is a program that opens a window and lets you interact with the shell

### 4 Dec
* How to use an AWS EC2 shell script and cron job to automate the generation of a Ruby Cucumber test of a RESTful API

### 27 Nov
* How to use kornshell booleans to create function to verify end-to-end system performance. 

### 26 Nov
* I should look a using [neovim](https://neovim.io/)
* I should leverage the training on [Upcase](https://thoughtbot.com/upcase)

## 25 Nov
* Python native assertions 

### 22 Nov
* Installed Docker Community Edition on my local machine.
* Started a Docker Container. A container is just a process on an OS.

### 21 Nov
* How I can apply stimulus-reflex in my art gallery side project.
* vim command `:%s/\t//g` to reduce a frustrating exercise to a few seconds of joy.

### 20 Nov
* Used vim to build a Puppeteer [Jest](https://jestjs.io/docs/en/puppeteer) scenario. 

### 19 Nov
* How to alias jvisualvn to check the status of RHEL systems. 
* Used vim to create a shell script that quickly scans for log records across 4 RHEL instances. 

### 18 Nov
* How to use node.js headless chrome testing on AWS Lambda

### 17 Nov
* Learned about [Jest](https://jestjs.io/)

### 16 Nov
* The best way to study for Security+ (4x exposure to material)
    * Take notes when first studying the material.
    * Audio Record important information from text boxes
    * Rewrite the notes later.
    * Replay audio

### 15 Nov
* A little bit about FlyWheel’s pricing model.
* How Linux sysadmins enable CAC login via private/public keys pairs.
* how to use Exceed to view system status as super user
* How to execute SQL developer from RHEL. 
* Uncovered windows regedit deficiency. researched solution and created instructions for windows admin professionals to fix the deficiency. 

### 14 Nov
* Why I should do this. 
* How to instruct the Air Force network operation security center to reload secure CRT and Exceed to my VDI profile.
* A little more about AWS Lambda.
* How do use mercurial to clone a repo on VMware.
* A primer on how to properly use service objects in Ruby on Rails. 
