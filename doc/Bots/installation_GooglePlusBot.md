##How to run GooglePlusBot

You need to :
  * [Install HubotSDK](https://github.com/hubiquitus/hubiquitus4java/blob/master/doc/HubotSDK/installation_HubotSDK.md)
  * Fill the file _config.txt_
    - Your _config.txt_ would look like:

```js
{
    "type" : "com.mycompany.PlusCount",
    "actor" : "urn:domain:u1", // your login to connect to server
    "pwd" : "urn:domain:u1", // your password to connect to server
    "hserver" : "http://localhost:8080", // the server url you want to connect to
    "adapters": [
        {
            "type": "org.hubiquitus.hubotsdk.adapters.HGooglePlusOneCercedInBox", // fix, the path of class HGooglePlusOneCercedInBox
            "properties": {
                "proxyHost": "yourProxyHost", // optional, your proxy host
                "proxyPort": yourProxyPort, // optional, your proxy port
                "googlePusNameOrId": "+Coca-cola", //Specified Name or Id GooglePlus Page used for finding information. ie : "+Coca-cola, 111883881632877146615"
                "roundTime": 5000, // refresh time in milliseconds
                "APIKey": "yourAPIKey" //Key to acces to the GooglePlus API, it means Simple API Access.
            }
        }
    ]
}
```

Note : [please see here for more information of G+](https://developers.google.com/+/).
  * Install all the jar included in pom.xml
    - Windows with intellij : 
        Tool Button(on right side) : Maven Project -> GooglePlusBot -> Lifecycle ->install
    - Linux : 
        1. Go to hubiquitus4java/Bots/GooglePlusBot in terminal
        2. tap "mvn clean install"
  * Run project
