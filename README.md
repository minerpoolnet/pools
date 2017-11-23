Data used in e.g. https://minerpool.net

This repo is used as a central data source. Please keep in mind that this data will be used at least on minerpool.net to list your pool public.

If you want to be listed please send your pull request to the <coin>.json you want to be listed in with your pool. If the coin want to be listed in is not available at the moment open up an issue and we'll see if we can support the coin.

Data format at the moment:
```json
	{
		"name":"<how the pool will be shown in the lists>",
		"stats":"https://<api fqdn with our without :port>/api/stats",
		"blocks":"https://<api fqdn with our without :port>/api/blocks",
		"payments":"https://<api fqdn with our without :port>/api/payments",
		"accounts":"https://<api fqdn with our without :port>/api/accounts",
		"miners":"https://<api fqdn with our without :port>/api/miners",
		"url":"<fqdn only without protocol or ports!>",
		"notify":"<your email adress for later notifying>"
	},
```
For e.g. open-ethereum-pool operators the different api paths will be mostly identical, but are still separated for other configurations.

To be done: 
- ~~Complete rework of the souce code, changes in the data structure~~ (finished / 100% done)
- Miner tracking, to identify pool hoppers
- Notifications to the pool operators in case of errors 
- Notifications to the miners in the case one of the rigs goes down 
