
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const alert = {
  assignedTo: "String",
  closedDateTime: "String (timestamp)",
  comments: [
    "String"
  ],
  feedback: "@odata.type: microsoft.graph.alertFeedback",
  status: "@odata.type: microsoft.graph.alertStatus",
  tags: [
    "String"
  ],
  vendorInformation: {
    provider: "String",
    vendor: "String"
  }
};

let res = await client.api('/security/alerts/{alert_id}')
	.update({alert : alert});

```