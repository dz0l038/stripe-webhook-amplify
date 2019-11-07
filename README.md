# stripe-webhook-amplify
Receive webhook from Stripe using a lambda setting up with Amplify

### Create the function
If you already have an api
```
? Please select from one of the below mentioned services REST
? Please select the REST API you would want to update stripeapi
? What would you like to do Add another path
? Provide a path (e.g., /items) /webhook
? Choose a Lambda source Create a new Lambda function
? Provide a friendly name for your resource to be used as a label for this category in the project: stripeWebhook
? Provide the AWS Lambda function name: stripeWebhook
? Choose the function template that you want to use: Serverless express function (Integration with Amazon API Gateway)
? Do you want to access other resources created in this project from your Lambda function? No
? Do you want to edit the local lambda function now? No
Succesfully added the Lambda function locally
? Restrict API access No
? Do you want to add another path? No
```

Push it
```
amplify push
```

### Create a webhook in Stripe
Stripe Dashboard -> Developers -> webhooks
Add a webhook with the endpoint and the event trigger

### Update the app.js
Copy the app.js in this repo. Replace the secret key and the webhook secret.
push
```
amplify push
```

Done! You can now use add your specific code in the app.js
