## Modular DBpedia Chatbot
### This tutorial will show you, step by step, How to use DBpediaxQanary chatbot!
### What’s inside: <br />
<span>&#8226;</span> <a href="#WhatisQanary">What is Qanary?</a> <br />
<span>&#8226;</span> <a href="#Whatisthepurposeofthischatbot?">What is the purpose of this chatbot?</a> <br />
<span>&#8226;</span> <a href="#GreetingsandInformation">Greetings and Information</a> <br />
<span>&#8226;</span> <a href="#Howtoconfigurechatbot">How to configure chatbot</a> <br />
<span>&#8226;</span> <a href="#Howtoaskaquestiontochatbot">How to ask a question to chatbot</a><br />
<span>&#8226;</span> <a href="#Howtoloadgraphvisualizationofthequestion">How to load graph visualization of the question</a><br />
<span>&#8226;</span> <a href="#Howtomakeaprofile">How to make a profile</a><br />

<h3 id="WhatisQanary">First let's learn quickly about what is Qanary?</h3>
Qanary is a methodology that allows to create, share and use components for Question Answering systems in an open ecosystem. It is part of the WDAqua research project which addresses the whole pipeline of question answering: <br />
(1) understand a spoken question <br />
(2) analyze the question’s text <br />
(3) find data to answer the question <br />
(4) present the answer(s).
<br />
<br />
Some more Information about the QANARY System:<br />
[Follow this](https://github.com/WDAqua/Qanary) Tutorial to create QANARY System Locally 
<br />
To learn more about QANARY [Click Here](https://github.com/WDAqua/Qanary/wiki/What-is-Qanary%3F) <br />
Github Link for [Qanary repository](https://github.com/WDAqua/Qanary) <br />
So in a Nutshell, Question>Qanary>DBpedia knowledge base>Dialogflow
<br />
<h3 id="Whatisthepurposeofthischatbot">What is the purpose of this chatbot?</h3> <br />
Currently the Qanary system is not easier to use for user so by making the chatbot it is now lot better to understand and use it and evern it supports feature like audio input, smalltalks and more state of the art features. 
<h3 id="GreetingsandInformation">Greetings and Information:</h3> <br />
**Here are some Information questions you can ask!**
<br />
```
User - how to contribute to DBpedia  
Bot - There are multiple ways to contribute to DBpedia You can: 1 - Look at open issues if you want to contribute to the codebase 2 - Improve Documentation 3 - Join the discussion on upcoming features, releases, and issues
```
```
User - what is DBpedia?  
Bot - DBpedia is a crowd-sourced community effort to extract structured information from Wikipedia and make this information available on the Web.  
```

<h3 id="Howtoconfigurechatbot">How to configure chatbot:</h3><br />
Let us take the question “What is the real name of Superman?” as running example. <br /> To ask this question to chatbot first you need to turn on following components  <br /> NED-DBpediaSpotlight,QueryBuilderSimpleRealNameOfSuperHero,SparqlExecuter
<br />
So basically, components play an important role here before asking any question you need to turn on component according to the question (To make it run remember the component list must be in order) 
<br />
If you want to learn more about Qanary Question Answering components There are around 30+ [Components](https://github.com/WDAqua/Qanary-question-answering-components) Integrated into Qanary. or you can simply ask "list of active Qanary components" to get the list of the available component to use.<br />

Now lets focus on how to Add or Remove and see the current active component from your list <br />  
**Configuration and internal information:** <br /> <br />
**To Activate/Add component you need to say "Add [Component name]" for example - Add sparql executer** <br /> 

```
User - Hi  
Bot - Hello! I am the DBpedia bot, How can I help you?  
User - Add sparql executer 
Bot - Successfully Added SparqlExecuter you can add more components by saying Add and then name of the component.  
```
<br />
**To Remove/Deactivate component you need to say "Remove [Component name]" for example - Remove sparql executer** <br />
```
User - Hi  
Bot - Hello! I am the DBpedia bot, How can I help you?  
User - Remove sparql executer  
Bot - successfully removed SparqlExecuter from the components list. 
```
<br />
**To see the currently active component from your list you need to say "tell me an order of components list"** <br />
```
User - Hi 
Bot - Hello! I am the DBpedia bot, How can I help you?  
User - tell me an order of components list  
Bot - currently, active components are NED-DBpediaSpotlight,QueryBuilderSimpleRealNameOfSuperHero,OpenTapiocaNED,BirthDataQueryBuilder,WikidataQueryExecuter  
```
<br />
**To see Reset the list of component from your list you need to say "reset component list"** <br />
```
User - Hi  
Bot - Hello! I am the DBpedia bot, How can I help you?  
User - reset the component list 
Bot - Components list are now empty  
```
<br />
Default components which are always on - NEDDBpediaSpotlight,QueryBuilderSimpleRealNameOfSuperHero,SparqlExecuter,OpenTapiocaNED,BirthDataQueryBuilder,WikidataQueryExecuter <br />

**To see the Active/Live QANARY Components from Server, not from the local List you can use the below command:** <br />
```
User - list of active Qanary components  
Bot - Total Active components are 55 and components are "coronabot-named-entity-recognition-location-de","SparqlExecuter","TagmeNED","MeaningCloud","NED-DBpediaSpotlight","coronabot-question-classification","QAnswerQueryBuilderAndExecutor","NERD-LuceneLinker","coronabot-missing-information","Dandelion","NER-FOX","WikidataQueryExecute.................
```
<br />
Below Image represents steps after configuring the components  
<br />
<img src="https://imgur.com/CQALTWn.png"> 
<br /> 

<h3 id="Howtoaskaquestiontochatbot">How to ask a question to chatbot:</h3>  <br />

**After setting up the components now we can ask questions to the Chatbot** 
<br />
For the example number one make sure you have activated follwing components - NED-DBpediaSpotlight,QueryBuilderSimpleRealNameOfSuperHero,SparqlExecuter 
<br />
```
User - What is the real name of hulk? 
Bot - resource:http://dbpedia.org/resource/Hulk answer:Robert Bruce Banner label:Hulk  
```
<br />
Now lets see Another example for this demo activate - OpenTapiocaNED,BirthDataQueryBuilder,WikidataQueryExecuter 
<br />
```
User - Where and when was Ada Lovelace born?
Bot - personLabel:Ada Lovelace birthplaceLabel:London birthdate:1815-12-10T00:00:00Z
```

If the components mentioned above are already activated then you don't have to activate them again on the local list of components 
<br />
Hint - To see the order of the component list you can ask "tell me an order of components list"
<br />
Currently, Answers are not looking good so we are planning to use NLP techniques to paraphrase the answer.
<br />

<h3 id="Howtoloadgraphvisualizationofthequestion">How to load graph visualization of the question:</h3>  <br />
**To understand more about how the Qanary system is working you can check out the graph using the below command**  <br />

```
User - Where and when was Ada Lovelace born?
Bot - personLabel:Ada Lovelace birthplaceLabel:London birthdate:1815-12-10T00:00:00Z
User - show rdf graph
Bot - Go to this link to see RDF Visualization - https://rdfgraphvisualizations.herokuapp.com/visualize/example
```
click on this [link](https://webengineering.ins.hs-anhalt.de:41022/visualize/example) to see demo graph.  <br />

<h3 id="Howtomakeaprofile">How to make a profile:</h3>  <br />
**To create a profile in which you can add a list of components you need to say “create [Profile name] profile” for example - create sport profile** - <br />

```
User - create sport profile
Bot - sport Profile added successfully. Now to use this profile you can say start sport to activate the profile. 
```
**To add component to profile you need to say “activate [component name] to [profile name]” for example - activate query builder to sport** - <br />
```
User - activate query builder to sport
Bot - Successfully Added QueryBuilder to the sport you can add more components by saying Add and then name of the component.
```
**To remove component to profile you need to say “deactivate [component name] from [profile name]” for example - deactivate query builder from sport** - <br />
```
User - deactivate query builder from sport
Bot - Successfully removed QueryBuilder from components list of sport. 
```

**To add profile components to local components list you need to say “start [profile name]” for example - start sport** - <br />
```
User - start sport
Bot - sport Activated Successfully to know about active components use command 'list of active components'.
```

**To see a list of components of a specific profile you need to say “show components of [profile name]” for example - show components of sport** - <br />
```
User - show components of sport
Bot - sport contains QueryBuilder
```

**To add default components use the command** - <br />
```
User - start default component
Bot - default component Activated Successfully to know about active components use command 'list of active components'.
```



If you are facing any bug please create an issue [here](https://github.com/dbpedia/chatbot-ng)
