Poll Trigger

```
{
    "templateId": "pollingtrigger",
    "title": "PollingTriggerPolicy_889ac351-281a-4eb5-469b-71c5c96fff5f",
    "type": "PollingTrigger",
    "parameters": {
        "x-ms-apimTemplateParameter.triggerConfig": {
            "updated_after": "@{triggerBody().data[0].created_at_formatted}"
        },
        "x-ms-apimTemplateParameter.triggerDataPath": "@triggerBody().data",
        "x-ms-apimTemplate-operationName": ["ProjectSnapshotTrigger"]
    }
}
```

A polling trigger is basically an event that periodically makes a call to your service to look for new data. Polling triggers differ from webhooks in that a polling trigger initiates an event to determine if new data is available, whereas webhooks respond to a push of new data from the service. Once the flow determines that new data is available, you can then perform an action with that data. This tutorial demonstrates how to use a polling trigger to proactively retrieve new data.

https://docs.microsoft.com/en-us/connectors/custom-connectors/media/create-polling-trigger/how-polling-works.png


https://docs.microsoft.com/en-us/connectors/custom-connectors/media/create-polling-trigger/how-polling-works.png

![](https://docs.microsoft.com/en-us/connectors/custom-connectors/media/create-polling-trigger/how-polling-works.png)


Revisit this Later