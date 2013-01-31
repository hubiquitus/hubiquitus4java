## How to run HelloHttpBot

You need to : 
 * [install HubotSDK](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/HubotSDK/installation_HubotSDK.md)
 * fill the file _config.txt_
    - Your _config.txt_ would look like:

```js

{
  "type" : "com.mycompany.WordCount",
  "actor" : "urn:localhost:u1", // your login to connect
	"pwd" : "urn:localhost:u1", // your password to connect
	"hserver" : "http://localhost:8080", // your server url to connect
	"adapters" : [
		{
            "type" : "org.hubiquitus.hubotsdk.adapters.HHttpAdapterInbox", // fix, the path of the class HHttpAdapterInbox
            "properties" :
                {
                    "host" : "localhost", // host + port (+ path) :  the endpoint where you want to receive the request
                    "port" : "8082",
                    "path" : "?id=1" //optional
                }
        },
        {
            "actor" : "httpOutbox", // the actor of your outbox adapter
            "type" : "org.hubiquitus.hubotsdk.adapters.HHttpAdapterOutbox" // fix, the path of the class HHttpAdapterOutbox
        }
	]
}
```
 * install the jar included in pom.xml
   - Windows with intellij : 
   	Tool Button(on right side) : Maven Project -> HelloHttpBot -> Lifecycle -> install
   - Linux : 
  	 1. Go to hubiquitus4java/Bots/HelloHttpBot in terminal
  	 2. tap "mvn clean install"
 * run the project
