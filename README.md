# Modular DBpedia Chatbot GSoC 2021 
Hello everyone, I am Jayesh Desai.<br /> 
I am very happy to announce about my selection in [Modular DBpedia Chatbot](https://summerofcode.withgoogle.com/projects/#5922382260207616) for GSoC 2021.
This will be my first GSoC project and I am very excited to work on this project Thank you [Andreas Both](https://www.linkedin.com/in/andreas-both-94267222/), [Aleksandr Perevalov](https://www.linkedin.com/in/alexander-perevalov-837780111/?lipi=urn%3Ali%3Apage%3Ad_flagship3_people_connections%3BU%2FpdNmPFSUqmoz82LyrZKA%3D%3D), [Ricardo Usbeck](https://www.linkedin.com/in/ricardo-usbeck/?lipi=urn%3Ali%3Apage%3Ad_flagship3_people_connections%3BQQw%2Bvv%2FvRwmEwkG30ZxSsQ%3D%3D), and [Ram Athreya](https://www.linkedin.com/in/ramgathreya/?lipi=urn%3Ali%3Apage%3Ad_flagship3_people_connections%3BQQw%2Bvv%2FvRwmEwkG30ZxSsQ%3D%3D) for giving me this opportunity excited to work with you all!
<br />
<br />
Google Summer of Code 2021 Modular DBpedia Chatbot Project link: [link](https://github.com/dbpedia/chatbot-ng) <br />
Tutorial link: [link](https://jayeshdesai4520.github.io/DBpedia-GSoC-2021/about)
<br />
<br />

## Table of Contents
<a href="#community_period">GSOC Community Bonding period</a>   
<a href="#coding_period">GSOC Coding period</a><br /> 
<span>&#8226;</span> <a href="#coding_period_weekone">Week One</a><br /> 
<span>&#8226;</span> <a href="#coding_period_weektwo">Week Two</a><br /> 
<span>&#8226;</span> <a href="#coding_period_weekthree">Week Three</a> <br /> 
<span>&#8226;</span> <a href="#coding_period_weekfour">Week Four</a><br /> 
<span>&#8226;</span> <a href="#coding_period_weekfive">Week Five</a><br />
<span>&#8226;</span> <a href="#coding_period_weeksix">Week Six</a><br /> 
<span>&#8226;</span> <a href="#coding_period_weekseven">Week Seven</a><br /> 
<span>&#8226;</span> <a href="#coding_period_weekeight">Week Eight</a><br /> 
<span>&#8226;</span> <a href="#coding_period_weeknine">Week Nine</a><br /> 
<span>&#8226;</span> <a href="#coding_period_weekten">Week Ten</a><br /> 
<span>&#8226;</span> <a href="#coding_period_weekeleven">Week Eleven</a><br /> 


<h3 id="community_period">GSOC Community Bonding period</h3>

[06/03/2021] I had a first meeting with almost all mentors/students and got to know about all the diffrent projects of this year <br> 
[06/04/2021] I had my first meeting with my mentors, During this first meeting, we have done self-introduction and looked to a overview of the project and decided to meet every week to show the progress of the project and to discuss about next steps and I am so glad to know my mentors and I will have a great journey of GSOC in this summer!

<h3 id="coding_period">GSOC Coding period</h3>

<h4 id="coding_period_weekone">Week one</h4>
Today is first day of first week I have gone through several documentations on [Qanary framework](https://github.com/WDAqua/Qanary) to understand more about it 
and to start with the project we decided to work on this three category first <br /> 1) Basic conversation <br /> 2) Configure settings <br /> 3) Question answer system <br />
<br /> So in Basic conversation there will be intents like Welcome intent, Fallback intent, Smalltalks and DBpedia questions like What is DBpedia? How to contribute to DBpedia? <br /> <br />  Configure settings contains intents like (de-)activate components (this status needs to be stored) and Get information about the current Qanary pipeline configuration intent <br /> <br /> 
Finally in Question answer system I need to create a intent which saves the user questions and send it to Qanary via API and after the whole qanary process it gives us the answer of the given question then we have to show it via dialogflow. <br /> <br /> 
[6/7/2021] Created GitHub repository<br />
[6/7/2021] I have created below intents<br />
1) Basic conversation<br />
	 Welcome Intent<br />
	 Fallback Intent<br />
	 SmallTalks<br />
2) DBpedia questions<br />
	 What is DBpedia?<br />
	 How to contribute to DBpedia?<br />
Later today I have added suggestion chip response to both of the DBpedia questions

[6/8/2021] Learning how to connect Webhooks to Dialogflow!

[6/9/2021] I have successfully implemented webhook tutorial
Link of tutorial [Link](https://chatbotsjournal.com/step-by-step-guide-to-integrate-dialogflow-with-nodejs-aba949302caa)

[6/10/2021]Learning how to connect External API like weather API to DialogFlow just for practice....

[6/12/2021]Uploaded code to heroku so no need to turn on ngrok everytime when to test chatbot




<h4 id="coding_period_weektwo">Week two</h4>
I had a meeting with my mentors at the end of week one and decided to work on 5 issues this week which are on github check [Link](https://github.com/jayeshdesai4520/chatbot-ng-internal/issues)<br />
[6/14/2021] ...<br />
[6/14/2021] Checking all possible options to do RDFvisualizations and SPARQL visualization that can be integrated to chatbot<br />
[6/15/2021] Checked demo of Qanary chatbot UI [Link](https://github.com/WDAqua/Qanary-Chatbot-UI) and understood how it works like component list and all<br />
[6/17/2021] Ran automated test using botium



<h4 id="coding_period_weekthree">Week three</h4>
[6/22/2021] Trying to visualize graph using pyvis library<br />
[6/23/2021] RDF Graph visualization is working now and hosted to Heroku<br />
[6/24/2021] Connected Qanary webservice<br />
[6/25/2021] Used Fallback Intent to get the question from user to send to Qanary<br />
<br />

<h4 id="coding_period_weekfour">Week Four</h4>
[6/28/2021] Added user sessions so each conversation for component list will be unique<br />
[7/3/2021]  Made RDF Graph visualization dynamic<br />
<br />


<h4 id="coding_period_weekfive">Week Five</h4>
[7/6/2021] Fetched list of Qanary components from Qanary framework in every 15 seconds it updates the list of components<br />
[7/7/2021] Added intent for user cannot ask for reload component for for then 10 times otherwise it will give a 30 second timeout<br />
[7/9/2021] Used Fuzzyset library so now no need to use Dialogflow entity Advantage of using fuzzy set library is now no need to update Dialogfloe entity every time when there is some new component in the live list of Qanary components
<br />
<h4 id="coding_period_weeksix">Week six</h4>
[7/12/2021] Updating the Dialogflow modeling so that the Qanary components names are not part of the configuration	<br />
[7/14/2021] Optimize Intent map and code<br />
[7/16/2021] Use camelcase everywhere and move all Intent functions to a seperate file<br />
<br />
<h4 id="coding_period_weekseven">Week seven</h4>
[7/19/2021]	Add "start with" Intent so that user can search components by alphabet or by word<br />
[7/21/2021]	Change the reset component logic<br />
[7/23/2021]	Add activate profile Intent<br />
<br />
<h4 id="coding_period_weekeight">Week Eight</h4>
[7/26/2021]	Add suggetsion chip reponse to suitable Intents and add support for Google Assistant App<br />
[7/28/2021]	Create a new blogpost tutorial<br />
[7/30/2021]	Add docker files<br />
<br />
<h4 id="coding_period_weeknine">Week Nine</h4>
[8/2/2021]	Get QANARY components as part of application startup<br />
[8/4/2021]	Create a custom component profile<br />
[8/6/2021]	Fix python file and get rid of global variable<br />
<br />
<h4 id="coding_period_weekten">Week Ten</h4>
[8/9/2021]	Add activate,remove,add,show profile component Intents<br />
[8/11/2021]	Remove hard-coded configuration from RDF-Vizualization file<br />
[8/12/2021]	Create a JS method for querying Qanary triplestore<br />
[8/13/2021]     Added new commands to remove all components from list<br />

<br />
<h4 id="coding_period_weekeleven">Week Eleven</h4>
[8/13/2021]	Work on documentation<br />
[8/16/2021]	Add wiki page<br />
<br /> 




