## Introduction

This eBook teaches you on how to create a Custom Connectors targeted to run on Power Automate Platform. I have been working in Power Automate for almost 2 years in building connectors in a large scale by leveraging most of the features available in the Platform.

## Who is this Book for

The target audience for this Book are anyone who has interested in Building Custom Connectors with basic knowledge of OpenAPI, REST API's and HTTP Request Response should able to understand this and can build connectors. Also, you should have some basic knowledge on Workflow, Flows which are the building Blocks in the Power Automate Platform.


## How this book organised

This book contains 14 Chapters which covers from Beginners to advanced features which can be leveraged in building Custom Connectors. This book also contains some Sample Snippets of Code mostly in JSON Syntax. 


Why we need Custom Connectors



Open API - Quick Introduction

- Power Platform uses OpenAPI as the base protocol for building the conectors. Currently it supports the older version 2.0 aka swagger file.
- A Swagger file contains the definition of all the operations exposed by a API Service including the Input and Output Parameters along with Security like Basic Auth, OAuth or API Key based Authentications.

- A Typical Swagger file looks like this with some important property nodes like paths, definitions, parameters, responses etc.

```
{

"paths":{

},

"definitions":{
}

"parameters":{
}


}



```

- Request Schema

- Response Schema



Different types of Connectors

- In Built Connectors
- Certified Connectors
- Open Sourced Connectors
- Independent Publisher Connector

How Microsoft Manages these Connectors

- Currently there are almost 200+ premium connectors available in the Microsoft gallery. To increase this the Power Platform Community encourages users to publish connectors via the Independent Publisher Program. 

To get your connector certified, either we need to upload the connector definition (swagger file) to the PowerPlatformConnector Repository. If you have any reason not to open source the connector code, then based on the approval, you can submit it to the ISV Studio.


Currently Microsoft uses Open Source Collaborative Method to manage some of the public connectors via GitHub Repository

https://github.com/Microsoft/PowerPlatformConnector


If you want to create one, you can fork the repository and send a pull request for that connector


Checklist for Submitting a Connector

Important

Schema Level
- Every connector operations should have a proper response Schema. Default Empty Schema will be reject unless there is a valid reason. `paconn` cli may not report this issue, but it will

 be enforced during submission.

```
"responses":{

"default":{

"description" : "default",
"schema": { }

}

}



```


```


responses":{

"200":{

"description" : "default",
"schema": { 

 "type":"object"
 "properties":{
 
 }

}

}

}




```


Cosmetic Level 

- By default the `paconn` cli may not add the `stackOwner` property in the apiProperties.json file when you download them. You need to add the stackOwner. 

```
StackOwner refers to the Original Owner of that API and the Publisher is the one who actually Publishes the connector. For certified connectors, if you are using someone's API under stackOwner then you may need get an approval letter before you submit them
```

- The swagger file should not have any additional spaces. If you are working in your custom IDE, those editors may add some spaces which may not be accepted by the certification team. The best way is to use the `paconn` cli to download the final assets and submit them for certification.













