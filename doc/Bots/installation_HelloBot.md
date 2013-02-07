## How to run HelloBot

You need to:
 * [install HubotSDK](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/HubotSDK/installation_HubotSDK.md)
 * fill the file _config.txt_
    - the _config.txt_ would look like :
    
```js
      
{
	"type" : "com.mycompany.WordCount",
	"actor" : "urn:localhost:u1", // the login to connect
	"pwd" : "urn:localhost:u1", // the password to connect
	"hserver" : "http://localhost:8080", // the server url you connect to
	"adapters" : [
			{
  				"actor" : "urn:localhost:testChannel" // the channel urn you want to subscribe to
			}
		]
}
```

 * install the jar included in pom.xml
   - Windows with intellij :
	Tool Button(on right side) : Maven Project -> HelloBot -> Lifecycle -> install
   - Linux : 
  	 1. Go to hubiquitus4java/Bots/HelloBot in terminal
  	 2. tap "mvn clean install"
 * run the project

## How to use HelloBot
 * Start TestClient (Examples/TestClient), a simple interface for Java hAPI
 * In the TestClient interface, specify a different username from HelloBot (for example, urn:localhost:u2).
 * Copy username into password
 * Fill "Actor" field with HelloBot's username (default is urn:localhost:u1)
 * Send a message such as "Azerty", HelloBot will answer with : "Hello Azerty"
 * You can also send a message through the channel HelloBot suscribed to. Warning : the channel must have been specified in the topology (hubiquitus/samples/sample1.json declares urn:localhost:channel). Change channel in "adapters" in HelloBots's config file to match.
Specify the same channel in "Actor" field in your TestClient interface and send, HelloBot should answer.
