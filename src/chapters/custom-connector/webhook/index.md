With the advent of webhook, applications can notify each other as and when a event occured. In the past polling method is used to check the status of particular interested event which is not efficient on both the side client and server. For example, if you want to get notified when a payment has been declined in a stripe account, you can subscribe for that particular event in Stripe API by providing a Notification/Webhook Url while subscribing. Stripe will post back the data to your webhook during a payment decline.

Not all modern API's provides this type of feature to subscribe for events. 
Lets take an another example that a Cloud Storage Provider gives a API to get the list of files in a folder. Assume this is a shared folder and you want to get notified as soon as someone modifies any items to this folder.

They don;t provide a webhook subscription to listen for a change to that folder. In this case we may need to use a poller based event trigger

Push Trigger

Poll Trigger