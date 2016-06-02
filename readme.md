## Let's Get CORS working with JSON + Forms

This is a sample project that uses the [serverless
framework](http://serverless.com/) to accept an inbound post.

The CORS endpoint works with application/json which you can test here:

http://test-cors.org/

Live Endpoint (at the time of this writing): https://lqua9t0r4g.execute-api.us-east-1.amazonaws.com/dev/testPost

I would like for it to accept raw form input and parse out an "email" input.

Returning the parsed input in the function response would be fine for now.

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
