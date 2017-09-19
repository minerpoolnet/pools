Data used in e.g. https://minerpool.net 

This repo is used as a central data source. Please keep in mind that this data will be used at least on minerpool.net to list your pool public. 

If you want to be listed please send your pull request to the <coin>.json you want to be listed in with your pool. If the coin want to be listed in is not available at the moment open up an issue and we'll see if we can support the coin.

Data format at the moment e.g.: 

    {  
	"name":"<how the pool will be shown in the lists>", 
	"stats":"https://<api fqdn with our without :port>/api/stats", 
	"blocks":"https://<api fqdn with our without :port>/api/blocks", 
	"payments":"https://<api fqdn with our without :port>/api/payments",
  	"miners":"https://<api fqdn with our without :port>/api/miners",
	"url":"<fqdn only without protocol or ports!>", 
	"notify":"<your email adress for later notifying>"
    },
    
To be done: 
- complete rework of the souce code, changes in the data structure (in work at the moment)
- miner tracking, to identify pool hoppers
- Notifications to the pool operators in case of errors 
- Notifications to the miners in the case one of the rigs goes down 
