So where to start with this what is vibe coding? How do you Vibe Code? How do you do it in Salesforce? Should you be doing it? Why would you do it? This is what this post looks to tackle its going to he semi instructional semi-opinion piece and hopefully mildly interesting. 

### What is Vibe Coding?
So lets start off with the big one What is vibe coding? Vibe coding is this process of using an AI and english languge to create code based on the vibes, the excitement, the energy, the feelings, the colour of your socks... Or as it is normally known plain text prompts into a LLM with the express purpose of writing code. It is an accessible way for non technical people to produce software (or technical people to 10x their productivity if you believe the hype). This puts coding in the hands of almost anyone who can get access to the code base and write a prompt.I think it is important that I get my opinion across here so you understand my angle, I really like this technology, I think it is fun to use and can actually generate some usable code and as someone that isnt a developer I love having that power in my hands. There are of course detractors of vibe coding and they would say that non-techincal staff using this can lead to poor quality code, lots of bugs and potential security vunerabilities. Those things aside I still think this is worth exploring for the non-technical Salesforce proffesional.

### Apex Vibes
I have used what I am going to talk about, with medium success in the past few months. I have tried the various models that are out there, Gemini, ChatGPT, Microsoft CoPilot (the corporate one) and GitHub Copilot but one LLM stood out head and shoulders above the others when it came to Salesforce Development and that was Salesforce's Agentforce Plugin for VSCode. Now you might be thinking "Tom doesnt agentforce just send data out to one of the big LLM providers" and you would right that is what it does on Platform but we arent on Platform here are we? 

Where are we then? We are actually interfacing with Salesforces own, cutomised LLMs, that right plural! CodeGen25 and and xGen-Code the former is for basic code completion whilst the later offers a more indepthbuilt from the ground up for writing the Launges in Salesforce. There are And creating Apex Classes, Apex Test Classes ,Lightning Web Components and Aura Components Super duper cool and Salesforce having their own LLM who knew?

### Instructions/Ramblings
This is the bit where I tell you sort of how to do it and also ruin the idea that you can be a complete coding rookie and access Agentforce for Developers from anywhere. It is accessible from VS Code - Microsoft's Free code platform. It can also be found in Salesforces own "Code Builer" app - basically an online version of VS code accssible from a properly configued salesforce org. 

I am not going to explain code builder as I don' have much experience with it and for all intents and purposes it is a just online VS Code. Let's talk through desktop VS Code, this is what I used day to day and by explain I mean you can watch Matt Gerry from Coding with the Force explain connecting and setting up a VS Code [here](https://www.youtube.com/watch?v=zKidSyBn-3Q&list=PL0wESsiWMBTqd9TMVrwC-wFoSVVDGYlzP&ab_channel=CodingWithTheForce).

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
This is so so aggresive, sometimes it wants to complete what you are currently writing/editing but more often than not it wants to insert multiple lines sometimes entire methods out of thin air! Can be great but can also be frustrating as it's suggestions are interesting...

**Test Case Generation**
A great idea, for those that don't know apex classes must have at leat 75% of their executable lines (non comments) covered by unit tests or you can't move your code between Salesforce environments. So this feature is essential! I have found it hit and miss sometimes genrating test classes that either test nothing useful or check for test results that don't makesense and don't scale. I am not that fond of this feature, it is more of a good starting point than an up and running out of the gate.

So there are the features! 

### Tip of the Iceberg
Hopefully this article has conveyed my level of excitement for what YOU could achieve with vibe coding. I think like right now, like today! This is a super fun way of writing code and gettng your toes wet in the Salesforce code. Set your VS Code up and enjoy several ways to get writing code you can either start speaking to the LLM and tell it what you want or start writing a little bit of code and Agentforce will fill in the blanks! 

### Useful Links
-[Code Gen on GitHub](https://github.com/salesforce/CodeGen)


So what does it look like in Salesforce? Something on ChatGPT, Gemini, Claude? For that we need to hop into VScode and install the agentforce extension.
