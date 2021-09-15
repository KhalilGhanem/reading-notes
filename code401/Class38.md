# Notifications

## Amazon SNS

Amazon Simple Notification Service (Amazon SNS) is a managed service that provides message delivery from publishers to subscribers (also known as producers and consumers).

## Creating an Amazon SNS topic

An Amazon SNS topic is a logical access point that acts as a communication channel. A topic lets you group multiple endpoints (such as AWS Lambda, Amazon SQS, HTTP/S, or an email address).

To create a topic using the AWS Management Console:

* Sign in to the Amazon SNS console
* Do one of the following:

   * If no topics have ever been created under your AWS account before, read the description of Amazon SNS on the home page.
   * If topics have been created under your AWS account before, on the navigation panel, choose Topics.
* On the Topics page, choose Create topic.
* On the Create topic page, in the Details section, do the following:
   
   * For Type, choose a topic type (Standard or FIFO).
   * Enter a Name for the topic. For a FIFO topic, add .fifo to the end of the name.
* Choose Create topic.
* Copy the topic ARN to the clipboard, for example: `arn:aws:sns:us-east-2:123456789012:MyTopic`.
