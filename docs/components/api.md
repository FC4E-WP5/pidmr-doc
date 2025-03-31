


### Metaresolver API -  PIDMR-API

The Metaresolver API is built using the Quarkus framework. It is designed to resolve Persistent Identifiers (PIDs) from various PID Providers. 
It redirects to  the Metaresolver that is responsible for the final resolution of the PIDs. 
The API is using specific regular expressions to understand the type of Provider and validate the Persistent identifier. The API understands 
the type of PID and then resolves it by requesting resolvable URLs from an external handler, the Metaresolver. 

The API supports three different resolution methods: resource, metadata, and landing page. 

The main characteristics are the following: 

 - PID Providers: The API supports the management of PID Providers. An administrator is able to manage (add, update, delete) the data of a PID Provider. The API also displays the list of PID Providers, each responsible for validating specific PIDs based on predefined regular expressions. An authorised user may also get the details of the PID Provider.
 - Resolve PIDs: For each resolution method, the API requests the corresponding resolvable URL from the Metaresolver. By default, this operation returns a JSON response containing the URL resolving the PID. A user may immediately resolve the PID by using the 'redirect' parameter since the API redirects you to the resolving page. The different types of resolution are as follows.
 - Resource Resolution: Resolving a PID using the resource resolution method provides the URL to the associated resource.
 - Metadata Resolution: Metadata resolution returns the URL to the metadata associated with a PID.
 - Landing Page Resolution: This resolution method provides the URL to the landing page associated with a PID.
 - Validate PIDs: This operation checks the validity of each identifier. Every Provider has a regex based on which the validation is performed.
 - Identify PIDs: This operation identifies PIDs based on a set of rules that are in the core of the API. The identification may be exact or it may be a proposal that matches more than one PID.
 - Batch PIDs: Another feature is that the api can fetch a number of PIDs , validate , identify and return the type of PID . 

This endpoint identifies PIDs from the provided text.

The Metaresolver API resides at [https://api.pidmr.argo.grnet.gr/](https://api.pidmr.argo.grnet.gr/)] and the documentation of the API can be 
reached at [https://api.pidmr.argo.grnet.gr/swagger-ui/](https://api.pidmr.argo.grnet.gr/swagger-ui/).
