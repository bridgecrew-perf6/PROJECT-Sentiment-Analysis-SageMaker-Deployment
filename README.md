# PROJECT-Sentiment-Analysis-SageMaker-Deployment
AWS SageMaker deployment project

This is my final project in Udacity's Deep Learning Nanodegree Program.
In this project I constructed a recurrent neural network (RNN) for the purpose of determining the sentiment of a movie review using the IMDB data set. I created this model using Amazon's SageMaker service. In addition, I also deployed the model and constructed a simple web app which could interact with the deployed model.

I also made use of some additinal AWS services, to make this setup working from an external webapp.
The diagram in Web App Diagram.svg gives an overview of how the various services will work together. I consturcted a Lambda function and gave it permission to send and recieve data from a SageMaker endpoint.

Lastly, the method I used to execute the Lambda function was a new endpoint that I created using API Gateway. This endpoint was a url that listens for data to be sent to it. Once it gets some data it will pass that data on to the Lambda function and then return whatever the Lambda function returns.

