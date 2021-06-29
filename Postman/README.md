# CollectiveAccess API Tests for Postman 

This collection of queries and mutations can be used to explore and test the [CollectiveAccess GraphQL API] (https://manual.collectiveaccess.org/developer/web_api/graphql.html) using [Postman](https://www.postman.com).

To get started, install Postman and import the `collectiveaccess.postman_collection.json` file. Next, create a new environment in Postman and add the following environment variables:

|  Variable  | Purpose                | Example initial value  
|---         |---                     |---	    
| domain     | Hostname of server     | ca.example.com     
| apiUrl     | URL to CA GraphQL endpoint    | https://ca.example.com/service   
| apiUsername     | Username to authenticate with     | serviceUser  
| apiPassword     | Password to authenticate with     | myServicePassword     
| jwtExpiresAt     | Expiration date/time of current token     | &lt;Leave initial value blank&gt;    
| refreshExpiresAt     | Expiration date/time of current refresh token     | &lt;Leave initial value blank&gt;    
| jwtToken     | Current token     | &lt;Leave initial value blank&gt;   
| refreshToken     | Current refresh token    | &lt;Leave initial value blank&gt;    

The `domain`, `apiUrl`, `apiUsername` and `apiPassword` variables must be set to valid values for your CollectiveAccess instance. The login used for authentication must have privileges to use the GraphQL API associated with it.

The Postman collection includes the following features:

* Automatic refresh of tokens
* Basic testing of API responses
* A (soon to be) full set of API query and mutation examples
