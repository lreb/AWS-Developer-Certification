### [Back to main readme](Readme.md)

- The visibility timeout of each queue is 30 seconds by default.
- Amazon SNS allows applications to send time-critical messages to multiple subscribers through a “push” mechanism, eliminating the need to periodically check or “poll” for updates. Amazon SQS is a message queue service used by distributed applications to exchange messages through a polling model, and can be used to decouple sending and receiving components. 
- FIFO (first-in-first-out) queues preserve the exact order in which messages are sent and received
- You pay only for what you use, and there is no minimum fee.
- The Amazon SQS Free Tier provides you with 1 million requests per month at no charge.
- Developers can get started with Amazon SQS by using only three APIs: SendMessage, ReceiveMessage, and DeleteMessage. SaveMessage is not required.