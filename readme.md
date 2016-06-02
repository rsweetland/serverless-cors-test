## Let's Get CORS working with JSON + Forms

This is a sample project that uses the [serverless
framework](http://serverless.com/) to accept an inbound post.

The endpoint works from http://test-cors.org/ with application/json.

I would like for it to accept raw form input from a CORS resource

# Installing

* Install Serverless
```npm install -g serverless```

* Clone this repo.

* ```npm install```

* Run the serverless init command

* Run ```serverless function deploy``` to deploy lambda function

* Run ```serverless endpoint deploy --all`` to deploy all endpoints
(required to include OPTIONS endpoint for CORS)

* Run ```serverless client deploy``` to deploy UI
