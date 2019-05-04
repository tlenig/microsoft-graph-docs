
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const checkin = {
  comment: "Updating the latest guidelines"
};

let res = await client.api('/drives/{drive-id}/items/{item-id}/checkin')
	.version('beta')
	.post(checkin);

```