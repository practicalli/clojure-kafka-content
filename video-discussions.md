# Video Discussions

## Session 02
{% youtube %}
https://www.youtube.com/watch?v=mQOO4wfcj7E?autoplay=1loop=1
{% endyoutube %}


Amr Gawish [10:59 PM]
Special thanks for the attendees: @jr0cket, @Gurps Bassi and @kanke.
*Summary of the meeting*
-------------------------------------------------------------------------------------------
• *1.* We talked about the architecture and discussed different components that make Kafka like brokers, topics, logs and partitions. We also spoke about Zookeeper and its role of managing Kafka cluster.

• *2.* We also had a small hands-on on how to test a sample HelloWorld producer, and consumer using Docker, the sample of the application used is available from this GitHub repo: https://github.com/SciSpike/kafka-lab

• *3.* John also shared an intriguing finding around Kafka not supporting Java 10 at the moment, and it seems to be related to Kafka using specific scripting that targets specific Java versions.

• *4.* We briefly spoke about the communication and how messages in Kafka is binary and would require serialization from producer side and deserialization from the consumer side, and you can JSON serializer and deserializer, binary serializers like Avro is better to be suited and provide more performance and compression (https://www.confluent.io/blog/avro-kafka-data/).

• *5.* We also spoke about How Apache Kafka core lacks multiple modules like _Kafka Connect_, _Kafka Streams_ and _Kafka REST proxy_ (https://www.confluent.io/blog/a-comprehensive-open-source-rest-proxy-for-kafka/) which are part of Confluent but have been open sourced while still maintained under confluent themselves (https://www.confluent.io/product/confluent-open-source/)

• *Finally* We agreed on the next tasks for the group, which will be:

>*Task:* Study the following articles: _*Kafka vs JMS*_ (http://cloudurable.com/blog/kafka-vs-jms/index.html) and _*Kafka Topic Architecture*_ (http://cloudurable.com/blog/kafka-architecture-topics/index.html)

>*Next Meeting:* Wednesday 27th of June 2018, from 9 PM BST.

>*Optional:* Hands-on with installing and setting up Kafka

:point_right: Session 2 video here: https://youtu.be/mQOO4wfcj7E :point_left: (edited)


Amr Gawish [11:03 PM]
set the channel topic: *Task:* Study the following articles: http://cloudurable.com/blog/kafka-vs-jms/index.html & http://cloudurable.com/blog/kafka-architecture-topics/index.html
*Next Meeting:* Wednesday 27th of June 2018, from 9 PM BST.


Amr Gawish [9:15 PM]
Yea, there is an `--offset` parameter, check here https://gist.github.com/mackwic/e68ccf10d9a27d1e1d7196bac5790831 (edited)


Gurps Bassi [9:18 PM]
ah I see what I’m doing wrong. I haven’t specified a partition.
the --offset only works with a partition
now I gotta figure out the name of the partition
when I started the broker I just specified
```--partitions 1```
and no name
ah got it
just needed to specify --partition 0 --offset <someNumber>
since I created a single partition by default
Not sure why I was thinking partitions have a name, they’re just indexed from 0 (edited)

Gurps Bassi [10:08 PM]
@Amr Gawish can you share the answers for lab 3?

Amr Gawish [10:08 PM]
Good information, thanks @Gurps Bassi for sharing
@Gurps Bassi he discussed how we can think about the problem from administrative point of view and the last two.labs kind of doing that



@channel
Thanks for the session and special thanks for the attendees: @jr0cket, @Gurps Bassi, @Jeremie, @Ted (what's your display name?), @Vivek and @kanke
*Summary of the meeting*
-------------------------------------------------------------------------------------------
• *1.* @Gurps Bassi demonstrated his - as always - excellent mind map about Kafka Topic architecture and discussed how a topic is divided into Partitions, with each partition can be led in different brokers, with each partition can be consumed by one consumer at most in one consumer group.

• *2.* We also talked about ensuring ordered in topics, as Kafa can only guarantee order if everything is saved into one partition.

• *3.* @Gurps Bassi also walked through HandsOn Lab 2 (https://github.com/SciSpike/kafka-lab/tree/master/labs/02-Publish-And-Subscribe) of an example producer and consumer using Kafka Java APIs and how simple the APIs looked.

• *4.* We briefly spoke about the difference between Kafka and JMS and how disappointed we were with the materials on that subject!

• *5.* @jr0cket also hinted at the benefit of Kafka's duality as it can act as a Queue or a Pub/Sub depending based on the need.

• *Finally* We agreed on the next tasks for the group, which will be:

>*Task:* Study the following articles:
>> _*Kafka Consumer*_ (http://cloudurable.com/blog/kafka-architecture-consumers/index.html)
>> _*Kafka Producer*_ (http://cloudurable.com/blog/kafka-architecture-producers/index.html)
>> _*Using Kafka from command Line*_ You can follow this -> http://cloudurable.com/blog/kafka-tutorial-kafka-from-command-line/index.html *or* -> https://github.com/SciSpike/kafka-lab/blob/master/labs/01-Verify-Installation/hello-world-kafka.md _if you want to use Docker_

>*Next Meeting:* Wednesday 4th of July 2018, from 9 PM BST.

>*Optional:* Hands-on with Kafka and Avro

:point_right: _*Session 3 video:*_ https://youtu.be/TxFt28Cp8vA  :point_left: (edited)


SciSpike/kafka-lab
https://github.com/SciSpike/kafka-lab/tree/master/labs/02-Publish-And-Subscribe
Contribute to kafka-lab development by creating an account on GitHub.
cloudurable.com

Kafka Architecture: Consumers
http://cloudurable.com/blog/kafka-architecture-consumers/index.html
Covers Kafka Consumer Architecture with a discussion consumer groups and how record processing is shared among a consumer group as well as failover for Kafka consumers.

Kafka Architecture: Producers
http://cloudurable.com/blog/kafka-architecture-producers/index.html
Covers Kafka Producer Architecture with a discussion of how a partition is chosen, producer cadence, and partitioning strategies.


Kafka Tutorial: Using Kafka from the command line
http://cloudurable.com/blog/kafka-tutorial-kafka-from-command-line/index.html
Kafka Training: Using Kafka from the command line starts up ZooKeeper, and Kafka and then uses Kafka command line tools to create a topic, produce some messages and consume them.

SciSpike/kafka-lab
https://github.com/SciSpike/kafka-lab/blob/master/labs/01-Verify-Installation/hello-world-kafka.md
Contribute to kafka-lab development by creating an account on GitHub.

Amr Gawish [10:33 PM]
set the channel topic: *Task:* Study the following articles: http://cloudurable.com/blog/kafka-architecture-consumers/index.html & http://cloudurable.com/blog/kafka-architecture-producers/index.html
*Next Meeting:* Wednesday 4th of July 2018, from 9 PM BST.

Amr Gawish [1:48 PM]
@channel
:point_right: _*Session 3 video:*_ https://youtu.be/TxFt28Cp8vA  :point_left:
YouTubeAmr Gawish
Kafka Topic Architecture | Kafka Study Group - Session 3 (Meet a Mentor | RecWorks)
