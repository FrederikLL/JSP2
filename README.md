# JS Period 2 handIn


## Explain Pros & Cons in using Node.js + Express to implement your Backend compared to a strategy using, for example, Java/JAX-RS/Tomcat
Pros:
JS only instead of multiple languages.
Node uses v8 engine by google, and its fast
Asynchronous processing non blocking
Cons:
Not really any alternative for javascript backend other than Node.
Not as old and used as java
cpu intenive apps dont work well with node(video,audio editing programs)

## (y) Explain the difference between Debug outputs and ApplicationLogging. What’s wrong with console.log(..) statements in our backend code.

## (y) Demonstrate a system using application logging and environment controlled debug statements.

## Explain, using relevant examples, concepts related to testing a REST-API using Node/JavaScript/Typescript + relevant packages 

## Explain a setup for Express/Node/Test/Mongo-DB development with Typescript, and how it handles "secret values", debug and testing.

(        
## Explain, preferably using an example, how you have deployed your node/Express applications, and which of the Express Production best ## practices you have followed.

## Explain possible steps to deploy many node/Express servers on the same droplet, how to deploy the code and how to ensure servers will ## continue to operate, even after a droplet restart.

## Explain, your chosen strategy to deploy a Node/Express application including how to solve the following deployment problems:
## - Ensure that you Node-process restarts after a (potential) exception that closed the application
## - Ensure that you Node-process restarts after a server (Ubuntu) restart
## - Ensure that you can run “many” node-applications on a single droplet on the same port (80)
)

## Explain, using relevant examples, the Express concept; middleware.

Middleware functions are functions that have access to the request object (req), the response object (res), and the next function in the application’s request-response cycle. The next function is a function in the Express router which, when invoked, executes the middleware succeeding the current middleware.

Middleware functions can perform the following tasks:

Execute any code.
Make changes to the request and the response objects.
End the request-response cycle.
Call the next middleware in the stack.

We use middlewares for loggers.

## Explain, using relevant examples, your strategy for implementing a REST-API with Node/Express  + TypeScript and demonstrate how you ## have tested the API.

## Explain, using relevant examples, how to test JavaScript/Typescript Backend Code, relevant packages (Mocha, Chai etc.) and how to test asynchronous code.

## NoSQL and MongoDB 

## Explain, generally, what is meant by a NoSQL database.

NoSQL is a non-relational database. Storage and retrieval of data is different from that classic rleational databses we know. They are increasingly popular in big data and real-time applications(like ours). Another good this is the easier horisontal scaling that can be a problem for relaitional databases. The data structeres are different in noSQL DBs and are viewed as being more flexible than the relational DB tables we know.

## (y) Explain Pros & Cons in using a NoSQL database like MongoDB as your data store, compared to a traditional Relational SQL Database ## like MySQL.

## Explain about indexes in MongoDB, how to create them, and demonstrate how you have used them.
Indexes in MongoDB are used to work with values other than primary key. Without indexes MongoDB queries must perform a scan on all documents in a collection. Indexes are a special data structure that store a small portion data set.
example of how to create the lastupdated index that we use to delete "old" locations:
await positionCollection.createIndex({ "lastUpdated": 1 }, {expireAfterSeconds: EXPIRES_AFTER});


## Explain, using your own code examples, how you have used some of MongoDB's "special" indexes like TTL and 2dsphere and perhaps also ## the Unique Index.

## Demonstrate, using a REST-API you have designed, how to perform all CRUD operations on a MongoDB

## Explain, using a relevant example, a full JavaScript backend including relevant test cases to test the REST-API (not on the ## production ##database)

## (r) Demonstrate, using your own code-samples, decisions you have made regarding → normalization vs denormalization

## Geo-location and Geojson


## Explain and demonstrate basic Geo-JSON, involving as a minimum, Points and Polygons

## (y) Explain and demonstrate ways to create Geo-JSON test data

## (y) Explain the typical order of longitude and latitude used by Server-Side API’s and Client-Side API’s

## Explain and demonstrate a REST API that implements geo-features, using a relevant geo-library and plain JavaScript

## Explain and demonstrate a REST API that implements geo-features, using Mongodb’s geospatial queries and indexes.

## This will come in period-3

## Explain and demonstrate a React Native Client that uses geo-components (Location, MapView, etc.)

## Demonstrate both server and client-side, of the geo-related parts of your implementation of the ongoing semester case.

