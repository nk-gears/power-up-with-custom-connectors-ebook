# Power Up - Custom Connectors - Work In Progress

This book contains cookbook recipes to develop custom connectors

# Summary

- [Introduction](README.md)
- [Power Automate](README.md)
  - [Flows](README.md)
  - [Flow vs Logic Apps](README.md)
- [Templates (PreBuilt Recipes)](README.md)
- [Create Flow](README.md)
  - [Automated](README.md)
  - [Instant](README.md)
  - [Scheduled](README.md)
  - [Business Process Flow](README.md)
- [Data Connections](README.md)
  - [API](README.md)
  - [OAuth](README.md)
- [Connectors](README.md)
  - [Built-in Connectors](README.md)
  - [Custom Connectors](README.md)
    - [Import](README.md)
    - [Connector App Manifest](README.md)
    - [Security ( Basic, OAuth 2.0, API Key, None)](README.md)
    - [Connector Definition](README.md)
    - [Actions - (API Operations)](README.md)
    - [Triggers - Webhook and Data Polling](README.md)
    - [Model Definitions](README.md)
    - [Policy Hooks - Change Behaviours of the Request/Response](README.md)
    - [Convert an array to an object (Preview)](README.md)
    - [Convert an object to an array (Preview)](README.md)
    - [Set host URL](README.md)
    - [Route requestSet HTTP header](README.md)
    - [Set property (Preview)](README.md)
    - [Set query string parameterSet header/query parameter value from URL (Preview)](README.md)
    - [Convert delimited string into array of objects (Preview)](README.md)
- [Test the Connector](README.md)
- [Publish the Connector](README.md)
- [Advanced Examples](README.md)
  - [Redirecting to External Data Service/Url](README.md)
    - [Upload/Download using a Azure Function](README.md)
    - [Encapsulate Business Feeatures using Azure Function](README.md)
    - [Secure the Authorization Headers](README.md)


-----------

[Contributors](misc/contributors.md)



# todo

Contents

- overview of the book
- power automate intro
- creating new custom connectors
- connector definitions
  - swagger 2.0
  - paths
  - encoding scheme
  - vendor metadata
  - x-ms-summary
  - dynamic schema
  - dynamic properties lookup
  - set policies
  - using dynamic variables inside policies
  - building independent connectors
  - Paconn cli
  - validate, update
  - client secrets
  - certified connectors procedure
  - dealing with large connectors
  - schema empty
  X-ms-summary
  - special characters
  - stack owner, publisher
  - warning paths
  - file picker
  - capability
  - Parameters
  - Definitions
  - responses
  
  - data connections
    - single connection
    - multiple auth connection
    - dynamic properties
    
  - webhook triggers
    - poll triggers
    - push triggers with callback
    