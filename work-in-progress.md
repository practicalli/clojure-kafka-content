# Work in progress

> ####TODO::Very messy - just a brain dump



 I’ve read the first two chapters and yes it is high level at the moment. However I’m enjoying it since the sections are small and focused. I think it will start getting more practical down the line.
Being new to Kafka, I’ve learnt some valuable stuff about its offering, architecture and its nomenclature.
@Amr Gawish when are we doing the next meet? Think we should bump up the pace to reading 2 sections a week. Will help us get to the practical quicker

Amr Gawish [12:22 PM]
Good point @Gurps Bassi, but people might be busy
Is everyone in @here able to read 2 sections a week of articles, I would not argue against diversifying our sources as we can talk about differences when we have an online gathering

Gurps Bassi [12:45 PM]
yeh it is important we stick to the same pace to make sure everyone gets the best out of it. Maybe set a target of 2 sections and then check to see before the e-meet where everyone has got to and if a lot of people haven’t managed to do 2, we drop the discussion to only 1.



## Schedule from paid online kafka course

https://www.safaribooksonline.com/live-training/courses/kafka-fundamentals/0636920183686/#instructors

Apache Kafka is an increasingly popular foundation for large-scale software systems. In this course, you’ll learn how to use Kafka to publish and subscribe to data streams, and how Kafka can be used to solve various use cases. You’ll also learn how to install and configure a Kafka cluster, and how to use the Kafka API’s to produce and consume data. We’ll also discuss how to connect Kafka to technologies for stream processing, log aggregation, and other related big-data technologies.

What you'll learn-and how you can apply it
Why Kafka is scalable
How to interact with Kafka
Kafka’s role in enterprise architectures
How to design Kafka topics and partitions
Participants will be able to:

Install and configure Kafka
Publish data to Kafka
Subscribe to data from Kafka
Design Kafka topics and partitions
This training course is for you because...
You are a software architect with experience building enterprise systems, and you need to ensure that your systems are scalable and fault tolerant
You are a software developer with Java experience, and you need to build software on top of Kafka
Prerequisites

Basic knowledge of Java
A GitHub link to a description for installations will be provided.

Recommended Preparation:

Learning Modern Java: A Crash Course Using Java 8

Docker: Up & Running, Chapter 3. Installing Docker

Introduction to Apache Kafka

About your instructor
Petter Graff is the co-founder of SciSpike, helping Fortune-500 companies reach their potential through training, consulting and custom development. Petter has extensive experience building large scale software systems for many of the Fortune-500 companies. Petter was the main architect behind the open source project Yaktor (yaktor.io) which relies on Kafka to deliver messages across large clusters of computation nodes. Yaktor and Kafka has been used by various companies to build systems processing millions of messages per second. Petter is also a frequent speaker at various conferences and an O’Reilly author (check out his Video Series on Design Patterns in Java).



Schedule
The timeframes are only estimates and may vary according to how the class is progressing

DAY 1
Introduction (Lecture ~ 20 min)

Who are we
What is Kafka
Explain first lab
Verify that everything is installed and working (Lab ~ 20 min)

Install Kafka through Docker
Run a simple example of Kafka
Introduction to Kafka (Lecture ~ 30 min)

Kafka under the hood
What is a topic
What is a partition
What is a producer
What is a consumer
Creating a topic and pass a message (Lab ~30 min)

Create a topic
Run a simple consumer
Run a simple producer
Dissecting the first example (Lecture/Discussion ~ 30 min)

Walkthrough of the first lab
Question and answers
Design of Kafka topics and partitions (Lecture ~ 30 min)

Case study
How to select topics
How to select partitions
Exercise: Designing topics and partitions (Group Project ~ 20 min)
- Design topics and partitions

DAY 2
Evaluation of the designs and suggested solutions (Discussion ~20 min)

Discussion of the suggested solution(s)
Recommended design of case study
Implement Topics and Partitions for case study (Lab ~30 min)

Define a topic and partition in Kafka
Create a consumer and producer
Run a test script
Scaling Kafka (Lecture ~30 min)

Kafka Brokers
Kafka Clusters
Cluster mirroring
Consumer groups
Streaming APIs for Kafka (Lecture ~20 min)

What is streaming
Why use streams
Programming to streams
Example streams using Spark
Streaming and IoT Case Study (Lab ~30 min)

Consume a stream from Kafka
Build a Spark application over the Kafka stream
Kafka Administration and Integration (Lecture ~30 Min)

Integration with Big Data tools (Storm, Spark, Hadoop)
Kafka Connect
Certified Kafka connectors
Kafka administration
Kafka monitoring
Security







Amr Gawish [9:41 PM]
Thanks for those who attended the session today, it was really interesting and very useful.
Special thanks to @Gurps Bassi for his amazing mind map about his Kafka and opening up the conversation with his findings around Zero Copying (https://www.ibm.com/developerworks/library/j-zerocopy/index.html) and backpushing
Thanks to @Jeremie for his encouragement and his thoughts around the application using IoT devices
Big thanks to @jr0cket for scaring all of us about the amount of transaction he works with everyday and his insights on those big machinery and how Kafka could be of benefit to them.
ibm.com
Efficient data transfer through zero copy
This article explains how you can improve the performance of I/O-intensive Java applications running on Linux and UNIX platforms through a technique called zero copy. Zero copy lets you avoid redundant data copies between intermediate buffers and reduces the number of context switches between user space and kernel space.


Amr Gawish [10:21 PM]
@channel Actions for the next meeting:
*Meeting Date:* 20th of June 2018, from 9 to 10pm
*Task:* http://cloudurable.com/blog/kafka-architecture/index.html
*Optional Hands on:* Thinking about how you can create a small slack chatbot to put messaged into Kafka topics to be utilised later
cloudurable.com

Kafka Architecture
Kafka Architecture: This article discusses the structure of Kafka. Kafka consists of Records, Topics, Consumers, Producers, Brokers, Logs, Partitions, and Clusters. Records can have key, value and timestamp. Kafka Records are immutable. This article covers the structure of and purpose of topics, log, partition, segments, brokers, producers, and consumers.



kankemwa Ishaku [9:42 AM]
@Amr Gawish Just joined unfortunately and went through the previous chats. Thanks for running the Kafka group. Is the whole of ->  http://cloudurable.com/blog/kafka-tutorial-v1/index.html and http://cloudurable.com/blog/kafka-architecture/index.html all you have covered in the group so that I can catch up.
cloudurable.com
Kafka Tutorial with Examples
http://cloudurable.com/blog/kafka-tutorial-v1/index.html
Cloudurable provides AWS Cassandra and Kafka support, Cassandra consulting, Cassandra training, and Kafka consulting. Our focus is on successful deployments of Cassandra and Kafka in AWS EC2. We work with the full AWS stack including Lambdas, EC2, EBS, CloudFormation, CloudWatch and more.
cloudurable.com
Kafka Architecture
http://cloudurable.com/blog/kafka-architecture/index.html
Kafka Architecture: This article discusses the structure of Kafka. Kafka consists of Records, Topics, Consumers, Producers, Brokers, Logs, Partitions, and Clusters. Records can have key, value and timestamp. Kafka Records are immutable. This article covers the structure of and purpose of topics, log, partition, segments, brokers, producers, and consumers.


(Amr Gawish) [9:45 AM]
Hi @kanke, welcome to the Kafka group.
This was our first meeting as we covered only part one of the tutorial (http://cloudurable.com/blog/what-is-kafka/index.html), the meeting points are above the pinned message to give you an idea what did we talk about during that online meeting
http://cloudurable.com/blog/what-is-kafka/index.html
