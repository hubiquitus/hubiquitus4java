## How to run TwitterBot

You need to :
 * [Install HubotSDK](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/HubotSDK/installation_HubotSDK.md)
 * Fill the file _config.txt_
    - Your _config.txt_ would look like: 
    
```js
{
  "type" : "com.mycompany.WordCount",
	"actor" : "urn:localhost:u1", // your login to connect to server
	"pwd" : "urn:localhost:u1", // your password to connect to server
	"hserver" : "http://hub.novediagroup.com:8080", // the server url you want to connect to
	"properties" : {
		"screenName" : "***" // the screen name you want to publish
	},
	"adapters" : [ 
		{
			"type" :  "org.hubiquitus.hubotsdk.adapters.HTwitterAdapterInbox_1_1", // fix, the path of class HTwitterAdapterInbox_1_1
			"properties" : {

				"proxyHost":"0.0.0.0", // optional, your proxy host.
				"proxyPort":0000, // optional, your proxy port.
				"consumerKey" : "***", // the consumer key of your application twitter. (see the note below.)
				"consumerSecret" : "***", // the consumer secret of your application twitter. (see the note below.)
				"twitterAccessToken" : "***", // the twitter access token of your application twitter. (see the note below.)
				"twitterAccessTokenSecret" : "***", // the twitter access token secret of your application twitter. (see the note below.)

				"tags" : "novedia", // the tags of which you want to receive the tweets.
				"stallWarnings" :"true",
				"delimited":"all",
				"replies":"all",
				"langFilter" : "fr"

			}			
		},
		{

			"actor" : "twitter_outbox",
			"type" : "org.hubiquitus.hubotsdk.adapters.HTwitterAdapterOutbox_1_1",
			"properties" : {
				"proxyHost":"0.0.0.0",
				"proxyPort":0000,
				"consumerKey" : "***",
				"consumerSecret" : "***",
				"twitterAccessToken" : "***",
				"twitterAccessTokenSecret" : "***"
			}
		}
	]
}

```
  
  Note: [please see here to get your authentication of twitter application](https://dev.twitter.com/). 
  
 * Install all the jar incluede in pom.xml
    - Windows with intellij : 
    	Tool Button(on right side) :  Maven project -> TwitterBot -> Lifecycle -> install
    - Linux : 
    	 1. Go to hubiquitus4java/Bots/TwitterBot in terminal
    	 2. tap "mvn clean install"
 * run project 
