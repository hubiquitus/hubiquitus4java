# Hubiquitus4java - An implementation of Hubiquitus for the Java platform

Hubiquitus4java is a set of Java components :

* Hubiquitus API : the Java bindings for the hubiquitus semantics
* Hubot SDK : a kit for Java developers allowing rapid development of hubiquitus agents called hubots
* Hubiquitus components : HTwitterAPI-1.1, HFacebook and HGooglePlus. The API used for the corresponding bots.
* Bots : it contains the sample bots you can lance for test.


## Prerequisite

[maven](http://maven.apache.org/) : all our jars are managed by maven.

## How to install

Before you lance the bots for test, you have to install the hAPI and HubotSDK.

 * See [Installation of hAPI](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/hAPI/installation_hapi.md) to install hAPI.
 * See [Installation of HubotSDK](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/HubotSDK/installation_HubotSDK.md) to install HubotSDK.


## How to use

### How to use hAPI


 * [Codes](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/hAPI/Codes.md) : ConnectionStatus, ConnectionError, ResultStatus ... All the enumeration of Hubiquitus.



 * [Datamodel](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/hAPI/hAPI_Datamodel.md) : Information about hAPI Datamodel.



 * [hClient Functions](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/hAPI/HClient_functions.md) : Connect, disconnect, builder ... All the function of the client.



 * [Options](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/hAPI/Options.md) : Information about options class.



### How to use HubotSDK



 * [HubotSDK Adapters](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/HubotSDK/HubotsdkAdapters.md) : Information about the adapters of hubot.



 * [HubotSDK Introduction](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/HubotSDK/HubotSDKIntroduction.md) : Introduction of a hubot.



 * [HubotSDK API](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/HubotSDK/HubotSDK_API.md) : Information about the API.



## The test projects

The "Bots" folder contains five samples bots :

* TwitterBot allows to retrive data from twitter and post a tweets. Click [here](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Bots/installation_TwitterBot.md) to see how to run the bot.
* FacebookBot allows to retrive data from facebook. Click [here](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Bots/installation_FacebookBot.md) to see how to run the bot.
* InstagramBot allows to retrive data from instagram. Click [here](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Bots/installation_InstagramBot.md) to see how to run the bot.
* GooglePlusBot allows to retrive data from googleplus. Click [here](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Bots/installation_GooglePlusBot.md) to see how to run the bot.
* HelloBot allows to retrive a string and publish it on a node. Click [here](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Bots/installation_HelloBot.md) to see how to run the bot.
* HelloHttpBot allows to retrive data from a url. Click [here](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Bots/installation_HelloHttpBot.md) to see how to run the bot.


The "Examples" folder content a sample exemples as :

* TestClient allows to test a hubiquitus plateform. Click [here](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Examples/TestClient.md) to see how to run the project.
* HFacebook simple client allows to retrive data from facebook using HFacebook componement. Click [here](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Examples/HFacebookSimpleClient.md) to see how to run the project.
* HTwitter Simples Clients allows to retrive data from twitter and post a tweets using HTwitterAPI-1.1. Click [here](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Examples/HTwitterSimpleClient.md) to see how to run the project.
* HGooglePlus Simple client allows to retrive data from Instagram using HGooglePlus. Click [here](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Examples/HGooglePlusSimpleClient.md) to see how to run the project.

