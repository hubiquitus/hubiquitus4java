# Hubiquitus4java - An implementation of Hubiquitus for the Java platform

Hubiquitus4java is a set of Java components :

* [Hubiquitus API](https://github.com/hubiquitus/hubiquitus4java/tree/master/hapi) : A Java API that allows to access to our system Hubiquitus. We call it hAPI.

* [HubotSDK](https://github.com/hubiquitus/hubiquitus4java/tree/master/HubotsSDK) : A SDK that allows to develop hubiquitus agents called hubots

* [Hubiquitus Components](https://github.com/hubiquitus/hubiquitus4java/tree/master/HubiquitusComponents) : HTwitterAPI-1.1, HFacebook and HGooglePlus. The API used for the corresponding adapter in HubotSDK.

* [Bots](https://github.com/hubiquitus/hubiquitus4java/tree/master/Bots) : it contains the sample bots you can lance for test.


## Prerequisite

[maven](http://maven.apache.org/) : all our jars are managed by maven.

## How to install

First of all, clone the project.
Tap the following command in terminal(Linux) or in Powershell(Windows) : 

```js
git clone git://github.com/hubiquitus/hubiquitus4java.git
```

Then install hAPI and HubotSDK : 

 * See [Installation of hAPI](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/hAPI/installation_hapi.md) to install hAPI.

 * See [Installation of HubotSDK](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/HubotSDK/installation_HubotSDK.md) to install HubotSDK.


## How to use

### How to use hAPI

Copy the hAPI-0.6.0.jar in _C:\Users\[your account]\.m2\repository\org\hubiquitus\hubiquitus4java\hAPI\0.6.0_ to your project 
or include the dependency in your Maven configuration:

```xml
<dependency>
 		<groupId>org.hubiquitus.hubiquitus4java</groupId>
			<artifactId>hAPI</artifactId>
			<version>0.6.0</version>
</dependency>
```

#### API Reference :

 * [hClient Functions](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/hAPI/HClient_functions.md) : Connect, disconnect, builder ... All the function of the client.

 * [Codes](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/hAPI/Codes.md) : ConnectionStatus, ConnectionError, ResultStatus ... All the enumeration of Hubiquitus.

 * [Datamodel](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/hAPI/hAPI_Datamodel.md) : Information about hAPI Datamodel.

 * [Options](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/hAPI/Options.md) : Information about options class.



### How to use HubotSDK

 * [HubotSDK Introduction](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/HubotSDK/HubotSDKIntroduction.md) : Introduction of a hubot.

 * [HubotSDK API](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/HubotSDK/HubotSDK_API.md) : Information about the API.
 
 * [HubotSDK Adapters](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/HubotSDK/HubotsdkAdapters.md) : Information about the adapters of hubot.

 


## The test projects

### Bots

The "Bots" folder contains five samples bots :

* [HelloBot](https://github.com/hubiquitus/hubiquitus4java/tree/master/Bots/HelloBot) allows to retrive a string and publish it on a node.  [Run the bot](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Bots/installation_HelloBot.md) 

* [HelloHttpBot](https://github.com/hubiquitus/hubiquitus4java/tree/master/Bots/HelloHttpBot) allows to retrive data from a url.  [Run the bot](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Bots/installation_HelloHttpBot.md) 

* [TwitterBot](https://github.com/hubiquitus/hubiquitus4java/tree/master/Bots/TwitterBot) allows to retrive data from twitter and post a tweets. [Run the bot](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Bots/installation_TwitterBot.md)

* [FacebookBot](https://github.com/hubiquitus/hubiquitus4java/tree/master/Bots/FacebookBot) allows to retrive data from facebook.  [Run the bot](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Bots/installation_FacebookBot.md)

* [InstagramBot](https://github.com/hubiquitus/hubiquitus4java/tree/master/Bots/InstagramBot) allows to retrive data from instagram.  [Run the bot](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Bots/installation_InstagramBot.md) 

* [GooglePlusBot](https://github.com/hubiquitus/hubiquitus4java/tree/master/Bots/GooglePlusBot) allows to retrive data from googleplus.  [Run the bot](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Bots/installation_GooglePlusBot.md) 



### Examples

The "Examples" folder contains the following examples

* [TestClient](https://github.com/hubiquitus/hubiquitus4java/tree/master/Examples/TestClient) provides an interface to test the hAPI.  [Run the example](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Examples/TestClient.md)

* [HFacebook simple client](https://github.com/hubiquitus/hubiquitus4java/tree/master/Examples/HFacebookSimpleClient) allows to retrive data from facebook using HFacebook componement.  [Run the example](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Examples/HFacebookSimpleClient.md) 

* [HTwitter simple client](https://github.com/hubiquitus/hubiquitus4java/tree/master/Examples/HTwitterSimplesClients) allows to retrive data from twitter and post a tweets using HTwitterAPI-1.1.  [Run the example](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Examples/HTwitterSimpleClient.md)

* [HGooglePlus simple client](https://github.com/hubiquitus/hubiquitus4java/tree/master/Examples/HGooglePlusSimpleClient) allows to retrive data from Instagram using HGooglePlus.  [Run the example](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/Examples/HGooglePlusSimpleClient.md)

