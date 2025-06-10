---
layout: post
title: Buh-bye Classic Approvals
date: 2025-06-09T00:00:00.000Z
author: tom
author_profile: /about/
categories:
  - technology
  - Salesforce
  - Release
  - Summer '25
image: /assets/images/FlowApprovals.jpg
tags:
  - technology
  - Salesforce
  - Release
  - Summer'25
  - Flow
---

Flow Approvals, for me one of the most exciting updates in recent years a HUGE Quality of Life jump over Classic Approvals (Salesforce's Name not mine) with acres of possibilities. Let me introduce you to what they have crammed into this release, in true internet click-baity fashion I have left the best till last!

Before I fly in let me start at the start. What exactly is a Flow Approval? Well many moons ago Salesforce launched a product called flow orchastrator, flow orchastrator had with in an Approval Orchastration a simple flow with two key elements Decision and Approval Steps. Whilist interesting this was a paid extra and you paid PER flow run. So not many people were looking this as a solution for their approvals, that was until spring '25 when Saleforce made this tool free! It is now known as Flow Approvals and looks to be the future of Approvals on the Salesforce platform, now we know the history lets talk 

### Recall Path for Approvals

![Recall!]({{site.baseurl}}/assets/images/ApprovalsDeepDive/Recall Path.png)

An essential part of any approval is the ability for the user that sent it to cancel it or "Recall" it and for us as the System Admin to be able to execute some automation when a user performs this action. Well with Flow Approvals this is now possible! A recall path can be added and one Stage can be configured with background step(s). This is great for say rolling back to an earlier stage if your approval has been updating the records stage, changing some record values or any other data clean up activity really!

### Delegation

![Work Guide.png]({{site.baseurl}}/assets/images/ApprovalsDeepDive/Work Guide.png)

The theme here really is Feature Parity, flow approvals are the future aren't they? This does as classic approvals did using the "Delegated approver" field on the user record. The delegated approver will then see approvals either in the work guide on the record page, in the approval work items componenet or in teir Approvals App. Super helpful and super clean.

### Submit from a Flow

![]({{site.baseurl}})![Submit an Approval Flow.png]({{site.baseurl}}/assets/images/ApprovalsDeepDive/Submit an Approval Flow.png)


FEATURE PARITY! Just like with classic approvals you can now launch an approval from a flow, you can pass in variables and you can even set how long the flow waits for an approval to happen before it Times out. It's not even feature parity it's a feature bonanza! 

### MAGIC!

![The Magical Wizard.png]({{site.baseurl}}/assets/images/ApprovalsDeepDive/The Magical Wizard.png)

One thing that was missing that made classic approvals so easy to get up and running was a setup Wizard. Well you won't believe what is here in this release... that's right a Setup wizard! Say it with me now FEATURE PARITY!!! Now it isn't without its quirks but where this feature shines is in the ability to teach you how Salesforce expects this functionality to be used, you can add all of the current features and upto 3 levels of approval. It does only create an auto launched Flow and not a record triggered Flow, hopefully that is a change they will make in the future to let you create both types. 

![Approval App Creating A Wizard.png]({{site.baseurl}}/assets/images/ApprovalsDeepDive/Approval App Creating A Wizard.png)

So where do you find this magical wizard, in the approvals app of course! What is the approvals app you say, a one stop shop for pending approvals, your approval submissions, your approval work items, reviewing my approval work itesm and now creating approvals. I think the wizard should exist inside of the automation app/Setup > Flow but what do I know.

If you made it here Thank You!

