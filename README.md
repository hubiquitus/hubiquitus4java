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

## The test projects

The "Bots" folder contains five samples bots :

* TwitterBot allows to retrive data from twitter and post a tweets [[README]](https://github.com/maniadel/hubiquitus4java/blob/master/Bots/TwitterBot/README.md)
* FacebookBot allows to retrive data from facebook [[README]](https://github.com/maniadel/hubiquitus4java/blob/master/Bots/FacebookBot/README.md)
* InstagramBot allows to retrive data from instagram [[README]](https://github.com/maniadel/hubiquitus4java/blob/master/Bots/InstagramBot/README.md)
* GooglePlusBot allows to retrive data from googleplus 
* HelloBot allows to retrive a string and publish it on a node [[README]](https://github.com/maniadel/hubiquitus4java/blob/master/Bots/HelloBot/README.md)
* HelloHttpBot allows to retrive data from RSS feed [[README]](https://github.com/maniadel/hubiquitus4java/blob/master/Bots/HelloHttpBot/README.md)


The "HubiquitusComponents" folder content three components :

* HTwitterAPI-1.1 allows to retrive data from twitter and post a tweets 
* HFacebook allows to retrive data from facebook 
* HGooglePlus allows to retrive data from GooglePlus


The "Examples" folder content a sample exemples as :

* TestClient allows to test a hubiquitus plateform
* HFacebook simple client allows to retrive data from facebook using HFacebook componement
* HTwitter Simples Clients allows to retrive data from twitter and post a tweets using HTwitterAPI-1.1
* HGooglePlus Simple client allows to retrive data from Instagram using HGooglePlus


To **run** your first bot, please read the following file : [INSTALLATION.md](https://github.com/maniadel/hubiquitus4java/blob/master/doc/INSTALLATION.md)

For more informations, please read the following wiki :  [HOME.md](https://github.com/maniadel/hubiquitus4java/blob/master/doc/HOME.md)
