## Modular DBpedia Chatbot
### This tutorial will show you, step by step, How to use DBpediaxQanary chatbot!
### What’s inside: <br />
<span>&#8226;</span> What is Qanary? <br />
<span>&#8226;</span> Greetings and Information <br />
<span>&#8226;</span> How to configure chatbot <br />
<span>&#8226;</span> How to ask a question to chatbot<br />
### First let's learn quickly about what is Qanary?
Qanary is a methodology that allows to create, share and use components for Question Answering systems in an open ecosystem. It is part of the WDAqua research project which addresses the whole pipeline of question answering: <br />
(1) understand a spoken question <br />
(2) analyze the question’s text <br />
(3) find data to answer the question <br />
(4) present the answer(s).
<br />
<br />
Some more Information about the Qanary System:<br />
[Follow this](https://github.com/WDAqua/Qanary) Tutorial to create QANARY System Locally 
To learn more about QANARY [Click Here](https://github.com/WDAqua/Qanary/wiki/What-is-Qanary%3F) <br />
Github Link for [Qanary repository](https://github.com/WDAqua/Qanary) <br />
So in a Nutshell, Question>Qanary>DBpedia knowledge base>Dialogflow
<br />
### Greetings and Information: <br />
**Here are some Information questions you can ask!**
<br />
User - how to contribute to dbpedia <br />
Bot - There are multiple ways to contribute to DBpedia You can: 1 - Look at open issues if you want to contribute to the codebase 2 - Improve Documentation 3 - Join the discussion on upcoming features, releases, and issues

User - what is DBpedia? <br />
Bot - DBpedia is a crowd-sourced community effort to extract structured information from Wikipedia and make this information available on the Web. <br />


### How to configure chatbot:<br />
Let us take the question “What is the real name of Superman?” as running example. <br /> To ask this question to chatbot first you need to turn on following components  <br /> NED-DBpediaSpotlight,QueryBuilderSimpleRealNameOfSuperHero,SparqlExecuter <br />
So basically, components plays important role here before asking any question you need to turn on component according to the question (To make it run remember component list must be in order) <br />
If you want to learn more about Qanary Question Answering components There are around 30+ [Components](https://github.com/WDAqua/Qanary-question-answering-components) Integrated in Qanary.   <br />
Below Image represents steps after configuring the components  
<br />
<img src="https://imgur.com/U3PcKwR.png" height="500" width="500"> <br /> <br />

Now lets focus on how to Add or Remove and see the current active component from your list <br />  
**Configuration and internal information:** <br /> <br />
**To Activate/Add component you need to say "Add [Component name]" for example - Add sparql executer** <br />
here is the conversation flow -  <br />
```
User - Hi  
Bot - Hello! I am the DBpedia bot, How can I help you?  
User - Add sparql executer 
Bot - Succesfully Added SparqlExecuter you can add more components by saying Add and then name of the component.  
```
<br />
**To Remove/Deactivate component you need to say "Remove [Component name]" for example - Remove sparql executer** <br />
```
User - Hi  
Bot - Hello! I am the DBpedia bot, How can I help you?  
User - Remove sparql executer  
Bot - succesfully removed SparqlExecuter from components list. 
```
<br />
**To see current active component from your list you need to say "tell me an order of components list"** <br />
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
User - reset component list 
Bot - Components list are now empty  
```
<br />
Default component which are always on are NEDDBpediaSpotlight,QueryBuilderSimpleRealNameOfSuperHero,SparqlExecuter,OpenTapiocaNED,BirthDataQueryBuilder,WikidataQueryExecuter <br />

**To see the Active/Live QANARY Components from Server not from the local List you can use the below command:** <br />
```
User - list of active qanary components  
Bot - Total Active components are 55 and components are "coronabot-named-entity-recognition-location-de","SparqlExecuter","TagmeNED","MeaningCloud","NED-DBpediaSpotlight","coronabot-question-classification","QAnswerQueryBuilderAndExecutor","NERD-LuceneLinker","coronabot-missing-information","Dandelion","NER-FOX","WikidataQueryExecute.................
```

### How to ask a question to chatbot:  <br />

**After setting up the components now we can ask questions to the bot** <br />
For the example number one make sure you have activated follwing components - NED-DBpediaSpotlight,QueryBuilderSimpleRealNameOfSuperHero,SparqlExecuter 
<br />
```
User - What is the real name of hulk? 
Bot - resource:http://dbpedia.org/resource/Hulk answer:Robert Bruce Banner label:Hulk  
```
<br />
Now lets see Another example for this activate - OpenTapiocaNED,BirthDataQueryBuilder,WikidataQueryExecuter 
<br />

If the components mentioned above are already activated then you dont have to activate again on the local list of components 
<br />
Tip - To see the order of the component list you can ask "tell me an order of components list"
<br />
If you are facing any bug please create a issue [here](https://github.com/dbpedia/chatbot-ng)
