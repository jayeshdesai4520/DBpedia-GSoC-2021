## Modular DBpedia Chatbot
### This tutorial will show you, step by step, How to use DBpediaxQanary chatbot!
### What’s inside: <br />
<span>&#8226;</span> What is Qanary? <br />
<span>&#8226;</span> How to configure chatbot <br />
<span>&#8226;</span> How to ask a question to chatbot<br />
### First let's learn quickly about what is Qanary?
Qanary is a methodology that allows to create, share and use components for Question Answering systems in an open ecosystem. It is part of the WDAqua research project which addresses the whole pipeline of question answering: <br />
(1) understand a spoken question <br />
(2) analyze the question’s text <br />
(3) find data to answer the question <br />
(4) present the answer(s).
<br />
Follow this Tutorial to create QANARY System Locally [Link](https://github.com/WDAqua/Qanary) 
<br />
To learn more about QANARY [Click Here](https://github.com/WDAqua/Qanary/wiki/What-is-Qanary%3F)
<br />
Let us take the question “What is the real name of Superman?” as running example. <br /> To ask this question to chatbot first you need to turn on following component NED-DBpediaSpotlight,QueryBuilderSimpleRealNameOfSuperHero,SparqlExecuter <br />
So basically, component plays important role here before asking any question you need to turn on component according to the question(To make it run remember component list must have to be in order) <br />
If you want to learn more about Qanary Question Answering components There are around 30+ [Components](https://github.com/WDAqua/Qanary-question-answering-components) Integrated in Qanary.
Defualt component which are always on are NED-DBpediaSpotlight,QueryBuilderSimpleRealNameOfSuperHero,SparqlExecuter,OpenTapiocaNED,BirthDataQueryBuilder,WikidataQueryExecuter
If you are facing any bug please create a issue [here](https://github.com/dbpedia/chatbot-ng)
