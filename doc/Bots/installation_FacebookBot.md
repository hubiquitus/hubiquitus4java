##How to run FacebookBot

You need to:
  * [Install HubotSDK](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/HubotSDK/installation_HubotSDK.md)
  * Fill the file _config.txt_
    - Your _config.txt_ would look like: 

```js
{
  "type" : "com.mycompany.WordCount",
	"actor" : "urn:domain:u1", // your login to connect to server
	"pwd" : "urn:domain:u1", // your password to connect to server
	"hserver" : "localhost:8080", // the server url you want to connect to
	
	"adapters" : [ 
		{
			"type" :  "org.hubiquitus.hubotsdk.adapters.HFacebookAdapterInbox",// fix, the path of class HFacebookAdapterInbox
			
			"properties" : {
				"proxyHost":"yourProxyHost", // optional, your proxy host
				"proxyPort":yourProxyPort, // optional, your proxy port
				"pageName":"yourPage", // the facebook page you want to count the number of its likes
				"roundTime":320 //the time in milliseconds to check the facebook page
			}				
		}	
	]
}
```


  * Install all the jar included in pom.xml
    - Windows with intellij : Maven Project -> FacebookBot -> Lifecycle -> install
    - Linux : 
        1. Go to hubiquitus4java/Bots/Facebook in terminal
        2. tap "mvn clean install"
  * run project
