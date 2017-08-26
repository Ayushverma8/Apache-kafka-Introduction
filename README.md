<!-- Problem Statement -->
<h1> Apache Kafka | Introduction </h1>
Apache Kafka is a publish-subscribe messaging system.A messaging system let you send messages between processes, applications, and servers.Broadly Speakng,  Apache Kafka is a software where topics (A topic might be a category) can be defined and further processed . Applications may connect to this system and transfer a message onto the topic. A message can include any kind of information ,from any event on your Personal blog or can be a very simple text message that would trigger any other event.



<h2>Kafka Broker</h2>
A Kafka cluster usually consists of one or more servers (called as kafka brokers), which are running Kafka over them. <strong>Producers</strong> are processes that publish data (push messages over trigger) into Kafka topics within the specified broker. A consumer of topics pulls messages off a Kafka topic. <!--more-->

<!--more-->


<img src="http://i.imgur.com/OO2Coeq.png" alt="Cluster" />
<h2>Kafka Topic</h2>
A Topic basically  is a category or a feed name to which messages are stored and published during operations. Messages are mostly  byte arrays that can store any object in any format.Yes , That's the best thing about kafka.Any object can be stored as byte array. Also,As we discussed before, all Kafka messages are organized into topics. If you wish to send a message you send it to a specific topic and if you wish to read a message you read it from a specific topic. 
<!--more-->

<h2>Consumers and consumer groups</h2>
Consumers can Always read messages starting from a specific offset and are allowed to read from any offset point they choose in between. This allows consumers to join the cluster at any point in time.This makes functioning and working really smooth.
<strong>Partitions allow you to parallelise a topic by splitting the data in a particular topic across multiple brokers.</strong>

<img src="http://i.imgur.com/MVkB5JK.jpg" alt="Consumer" />

<h2>Apache Kafka and Important Server concepts</h2>
	
	<li><strong>Topic partition</strong>: Kafka topics are divided into a number of partitions, which allows you to split data across multiple brokers.
</li>
	<li><strong>Consumer Group</strong>: A consumer group includes the set of consumer processes that are subscribing to a specific topic.</li>
	<li><strong>Node</strong>: A node is a single computer in the Apache Kafka cluster.</li>
	<li><strong>Replicas</strong> A replica of a partition is a "backup" of a partition. Replicas never read or write data. They are used to prevent data loss.
</li>
<li> <strong>Producer</strong>: Application that sends the messages.	
<li><strong>Consumer</strong>: Application that receives the messages.
</li>

<h2> Real time Applications </h2>
	<li><strong>Twitter</strong>: Registered users can read and post tweets, but unregistered users can only read tweets. Twitter uses Storm-Kafka as a part of their stream processing infrastructure.</li>
	<li><strong>LinkedIn</strong>:Apache Kafka is used at LinkedIn for activity stream data and operational metrics. Kafka mes-saging system helps LinkedIn with various products like LinkedIn Newsfeed, LinkedIn Today for online message consumption and in addition to offline analytics systems like Hadoop</li>
	<li><strong>Netflix</strong>: Netflix is an American multinational provider of on-demand Internet streaming media. Netflix uses Kafka for real-time monitoring and event processing.

</li>
	<li><strong>Box</strong>:At Box, Kafka is used for the production analytics pipeline &amp; real time monitoring infrastructure. We are planning to use Kafka for some of the new products &amp; features </li>



<strong>References</strong> :
<a href="https://kafka.apache.org/" target="_blank">Kafka official</a>
<a href="https://en.wikipedia.org/wiki/Apache_Kafka" target="_blank">Wiki</a>
