# AWS SNS and SQS
* SNS supports several end points such as email, sms, http end point and SQS. If you want unknown number and type of subscribers to receive messages, you need SNS.

## SNS (Simple Notification Service)

* **SNS** (Simple Notification Service)
* **SNS is a distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS.**
*  fast
* flexible
* fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients.
*  makes it simple and cost effective to send push notifications to mobile device users
* A distributed publish-subscribe system ,Messages are pushed to subscribers as and when they are sent by publishers to SNS ,SNS supports several end points such as email, sms, http end point and SQS.**you want unknown number and type of subscribers to receive messages, you need SNS.**
 
* You can use SNS to send SMS messages to mobile device users in the US or to email recipients worldwide.



## SQS
**SQS** is distributed queuing service.
* Messages are not pushed to receivers. Receivers have to poll SQS to receive messages
* Messages can’t be received by multiple receivers at the same time
*  Any one receiver can receive a message, process and delete it
* Other receivers do not receive the same message later.
* is mainly used to decouple applications or integrate applications.
* Messages can be stored in SQS for short duration of time (max 14 days).
* Messages can be stored in SQS for short duration of time (max 14 days).

## Use Cases
* **Choose SNS if:**
* You would like to be able to publish and consume batches of messages.
* You would like to allow same message to be processed in multiple ways.
* Multiple subscribers are needed.
* **Choose SQS if:**
* You need a simple queue with no particular additional requirements.
* Decoupling two applications and allowing parallel asynchronous processing.
* Only one subscriber is needed.

## Term
* **FIFO Queue :**Firt in queue First Out
* **Pub/Sub :** is an asynchronous messaging service that decouples services that produce events from services

# Q
1. What’s the difference between a FIFO and a standard queue?

- FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing. FIFO queues provide additional features that help prevent unintentional duplicates from being sent by message producers or from being received by message consumers

2. How can the server be assured a message was properly received?
- socket.io’s acknowledgements.

3. What classic design pattern is best represented by event driven programming?
-  Event-driven from end to end

4. How do you test an event driven system?
- 