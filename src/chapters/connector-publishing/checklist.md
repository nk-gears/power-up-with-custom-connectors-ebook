# Common Errors Schema





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


