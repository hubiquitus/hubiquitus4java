## How to run HelloBot

You need to:
 * [install hAPI](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/hAPI/installation_hapi.md)
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