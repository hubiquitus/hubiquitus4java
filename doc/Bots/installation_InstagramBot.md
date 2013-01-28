## How to run InstagramBot

You need to :
  * [Install HubotSDK](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/HubotSDK/installation_HubotSDK.md)
  * Fill the file _config.txt_
    - Your _config.txt_ would look like:
```js
  {
    "type": "com.mycompany.WordCount",
    "actor": "urn:localhost:u1", // your login to connect to server
    "pwd": "urn:localhost:u1", // your password to connect to server
    "hserver": "http://localhost:8080", // the server url you conncet to 
    "adapters": [
        {
            "type": "org.hubiquitus.hubotsdk.adapters.HInstagramRealTimeInbox", // fix, the path of class HInstagramRealTimeInbox
            "properties": {
                "port": yourPort, // port of your choice to listen http
        "clientId":"InstagramClientId", // Instagram clien id, you get it at the instagram subscription
                "clientSecret":"InstagramClientSecret", // Instagram clien secret, you get it at the instagram subscription.
            "object":"tag", // The object you'd like to subscribe to (in this case, "tag").
                "aspect":"media", // The aspect of the object you'd like to subscribe to (for this adapter, "media"). Note that Instagram API only support "media" at this time, but it might supports other types of subscriptions in the future.
                "object_id":"yourInstagramTag", // used to subscribe to new photos tagged with certain words. ie (Paris, USA, TIKJDA, ...), you can use 'object_id = nofilter' to listen all notification of new photos. You will receive a POST request at the callback URL every time anyone posts a new photo with the tag.
            "verifyToken":"YourVerfyToken", // "you can chose it randomly" ie(19a78b66c)
            "callbackUrl": "yourUrlCallBack" // is your url call back, ie( yourEndPoint:YourPort)   
            }
        }
    ]
}
```
Note: [Please see here for more information of instagram](http://instagram.com/developer/)

  * Install all the jar included in pom.xml
    - Windows with intellij : Maven Project -> InstagramBot -> Lifecycle -> install
    - Linux :
      1. Go to hubiquitus4java/Bots/InstagramBot in terminal
      2. tap "mvn clean install"

  * Run project
