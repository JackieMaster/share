The main idea of that PR is to standard webhooks across the services, using the graph service model.
However, it relates to the issue with an initial login not working because the current front-end polls the backend to find out when the SIWF transactions have completed.
A better solution is for the backend to use a Server Sent Event (SSE) to the front end when it receives the webhook callback from gateway account service.
There is an example of using SSE in SAT already, it's used to update the feeds when the content-publishing service uses its webhook callback when it finds new content on the blockchain.
6:59
Let me know if you would like specific pointers to the code where all of this is implemented.
