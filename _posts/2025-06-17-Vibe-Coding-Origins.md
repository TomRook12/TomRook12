---
layout: post
title: "Vibe Coding Orgins"
date: 2025-06-17
author: tom
categories: [technology, Salesforce, Agentforce, AI]
image: /assets/images/VibeCoding.png
tags: [technology, Salesforce, AI, Agentforce, Coding]
---
You may have heard this term Vibe Coding banded about (it was actually coined only a few months ago) and thought what is that? Can I use that? Are there Salesforce Vibes? Well I too had these thoughts so I jumped in to a salesforce org see what was possible.

### What is Vibe Coding?
Vibe coding is this process of using an AI and the vibes, the excitement, the energy, the feelings, the colour of your socks... Or as it is normally known plain text prompts into a LLM with the express purpose of writing code. It is championed as an accessible way for non technical people to produce software (or technical people to 10x their productivity if you believe the hype). This in thoery puts coding in the hands of almost anyone who can get access to the code base and write a prompt!

I think it is important that I get my opinion across here, I really like this technology, I think it is fun to use and can actually generate some usable code and as someone that isnt a developer I love having that power in my hands. There are of course detractors of vibe coding and they would say that non-techincal people using this can lead to poor quality code, lots of bugs and potential security vunerabilities. Those are to be quite honest valid critiques of this approach... but those things aside I still think this is worth exploring for the non-technical Salesforce proffesional to get their toes wet with coding.

### Apex Vibes
Now I have tried the various LLMs that are out there, Gemini, ChatGPT and GitHub Copilot but one LLM stood out head and shoulders above the others when it came to Salesforce Development and that was Salesforce's Agentforce for Developers. Now you might be thinking *"Tom doesn't agentforce just send data out to one of the big LLM providers"* and you would right that is what it does on the Salesforce Platform but we arent on the Salesforce Platform here are we? 

Where are we then? We are actually interfacing with Salesforces own, cutomised LLMs, that right plural! CodeGen25 and and xGen-Code, you don't pick which one to use they both come under the banner of Agentforce for Developers. They are used for creating and reviewing Apex Classes, Apex Test Classes, Lightning Web Components and Aura Components Super duper cool and Salesforce having their own LLM who knew?

### Instructions/Ramblings
This is the bit where I tell you sort of how to do it and also ruin the idea that you can be a complete coding rookie and access Agentforce for Developers from anywhere. It is accessible from VS Code - Microsoft's Free code platform. It can also be found in Salesforces own "Code Builer" app - basically an online version of VS code accssible from a properly configued Salesforce org. 

I am not going to explain code builder as I don't have much experience with it and for all intents and purposes it is a just online VS Code, so we'll park that option if it's ok with you. That being said let's talk through desktop VS Code, this is what I used day to day and by explain I mean you can watch Matt Gerry from Coding with the Force explain connecting and setting up a VS Code [here](https://www.youtube.com/watch?v=zKidSyBn-3Q&list=PL0wESsiWMBTqd9TMVrwC-wFoSVVDGYlzP&ab_channel=CodingWithTheForce).

If you have succesfully installed VS Code, the extensions and finally connected to a Salesforce Org you should have a new Salesforce AI logo that you can click on! What features does the Salesforce AI bring with it? 
-Dev Assitant - You can ask for help here, even passing in the current file you have open, asking questions about the code in front of you, like what it does or improving/enhacning it.
-Straight Code Creation - Just like other LLMs prompt it to create something using a plain text use case.
-Inline Code Completion - Will finish line(s) for you, with helpful reccomendations.
-Test Case Generation - A specific page for creating tests for APEX and LWC.

Some of these features are better than others for our vibe coding advneture. Let's review:

**Straight Code Creation**
This is the heart of the vibe coding area, truly great in my opinion and where Agentforce for Developers shines, generating Apex, Java Script, HTML, XML and CSS. Once code is generated you can also ask it about errors when deploying, errors when running and have it generate comments. Absoloutely fantastic! 

**Dev Assistant**
Great for understanding code you don't understand at the moment.

**Inline Code Completion**
This is so so aggresive, sometimes it wants to complete the line that you are currently writing/editing but more often than not it wants to insert multiple lines sometimes entire methods out of thin air! Can be great but can also be frustrating as it's suggestions are interesting...

**Test Case Generation**
Test cases are important, but this was frustrating to use, for those that don't know apex classes must have at leat 75% of their executable lines (non comments) covered by unit tests or you can't deploy your code between Salesforce environments. So tests are essential! I have found it hit and miss sometimes genrating test classes that either test nothing useful or check for test results that don't make sense and don't scale. I am not that fond of this feature, it is more of a good starting point than an up and running out of the gate.

So there are the features, that you could get invoved in!

### Tip of the Iceberg
Hopefully this article has conveyed my level of excitement for what **YOU** could achieve with vibe coding, and also how much I have enjoyed Agentforce for Developers. I would reccomend that you get out there in a dev org and give this a whirl. Set your VS Code up and enjoy several ways to get writing code you can either start speaking to the LLM and tell it what you want or start writing a little bit of code and Agentforce will fill in the blanks (if you want to try this option head over to Salesforce Developers help for code snippets and examples of what to do). 

### Useful Links
-[Code Gen on GitHub](https://github.com/salesforce/CodeGen)
-Salesforce's Agentforce for Developer home
-Salesforce Developer Help
-Coding with the Force YouTube



So what does it look like in Salesforce? Something on ChatGPT, Gemini, Claude? For that we need to hop into VScode and install the agentforce extension.
