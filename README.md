# Modular DBpedia Chatbot GSoC 2021

Hello everyone, I am Jayesh Desai.<br /> 
I am very happy to announce about my selection in [Modular DBpedia Chatbot](https://summerofcode.withgoogle.com/projects/#5922382260207616) for GSoC 2021.
This will be my first GSoC project and I am very excited to work on this project Thank you [Andreas both](https://www.linkedin.com/in/andreas-both-94267222/), [Alexander perevalov](https://www.linkedin.com/in/alexander-perevalov-837780111/?lipi=urn%3Ali%3Apage%3Ad_flagship3_people_connections%3BU%2FpdNmPFSUqmoz82LyrZKA%3D%3D), [Ricardo usbeck](https://www.linkedin.com/in/ricardo-usbeck/?lipi=urn%3Ali%3Apage%3Ad_flagship3_people_connections%3BQQw%2Bvv%2FvRwmEwkG30ZxSsQ%3D%3D), [Ram athreya](https://www.linkedin.com/in/ramgathreya/?lipi=urn%3Ali%3Apage%3Ad_flagship3_people_connections%3BQQw%2Bvv%2FvRwmEwkG30ZxSsQ%3D%3D) for giving me this opportunity excited to work with you all!
<br />
<br />
Google Summer of Code 2021 Modular DBpedia Chatbot Project link: [link](https://github.com/dbpedia/chatbot-ng)
<br />
<br />

## Table of Contents
<a href="#community_period">GSOC Community Bonding period</a>   
<a href="#coding_period">GSOC Coding period</a><br /> 
<span>&#8226;</span> <a href="#coding_period_weekone">Week one</a><br /> 
<span>&#8226;</span> <a href="#coding_period_weektwo">Week two</a><br /> 
<span>&#8226;</span> <a href="#coding_period_weekthree">Week three</a> 

<h3 id="community_period">GSOC Community Bonding period</h3>

[06/03/2021] I had a first meeting with almost all mentors/students and got to know about all the diffrent projects of this year <br> 
[06/04/2021] I had my first meeting with my mentors, During this first meeting, we have done self-introduction and looked to a overview of the project and decided to meet every week to show the progress of the project and to discuss about next steps and I am so glad to know my mentors and I will have a great journey of GSOC in this summer!

<h3 id="coding_period">GSOC Coding period</h3>

<h4 id="coding_period_weekone">Week one</h4>
Today is first day of first week I have gone through several documentations on [Qanary framework](https://github.com/WDAqua/Qanary) to understand more about it 
and to start with the project we decided to work on this three category first <br /> 1) Basic conversation <br /> 2) Configure settings <br /> 3) Question answer system <br />
<br /> So in Basic conversation there will be intents like Welcome intent, Fallback intent, Smalltalks and DBpedia questions like What is DBpedia? How to contribute to DBpedia? <br /> <br />  Configure settings contains intents like (de-)activate components (this status needs to be stored) and Get information about the current Qanary pipeline configuration intent <br /> <br /> 
Finally in Question answer system I need to create a intent which saves the user questions and send it to Qanary via API and after the whole qanary process it gives us the answer of the given question then we have to show it via dialogflow. <br /> <br /> 
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



<h4 id="coding_period_weektwo">Week two</h4>
<h4 id="coding_period_weekthree">Week three</h4>



<br />  Adding everthing in detail soon! <br /> 




