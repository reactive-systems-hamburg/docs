#Akka-based MQTT broker


##About MQTT

https://en.wikipedia.org/wiki/MQTT

http://mqtt.org


##Why?
* Akka might be a good fit for a very scalable MQTT broker, that can handle millions of clients & millions of messages/second.
* We can learn a lot about implement a messaging protocol on top of Akka, and about MQTT
* Once we have a working broker, we can build some fun IoT application on top of it
* It should not be too difficult to get a start, there are clients, tests etc. from other projects we can use
* There is also at least one open source Java MQTT broker (Moquette), we can look at the implementation there when we are stuck.
* TCP server implementations on top of akka-io are also available as a starting point (e.g. Jürgens proxy?)
* Interesting to compare different architectures, both programming model and performance. Moquette is “designed to be evented, uses Netty for the protocol encoding and decoding part, the protocol logic is essentially a single threaded and it's isolated from front connectors part by LMAX disruptor's ring buffer.” That’s also pretty cool and it would be great to learn something about Netty and disruptor on the way, too. The node.js are surely also “essentially single threaded”.



##Links
###MQTT projects
https://github.com/mcollina/mosca (node.js)

https://github.com/fusesource/mqtt-client (just a client, maybe useful for testing?)

http://nodered.org (node.js)

http://mosquitto.org (C?)

https://code.google.com/p/moquette-mqtt/ (Java)

### Conformance/Interoperability Test suite

http://www.eclipse.org/paho/clients/testing/

###Other
https://hseeberger.github.io/blog/2013/06/17/introduction-to-akka-i-slash-o/


##To dos:
* kick-off meeting (Google Hangout)
* define “minimal viable product”
* define tasks & sprints
* Tool? Trello board?
* find a name
  * akka-mqtt (sounds too official..)
  * hamqtt (Hamburg Akka Meetup MQTT)
  * cutie
    * because mqtt sounds like m cutie t
    * cutie.io is available ;)
    * it's a cute name, not too serious, no danger of violating trade mark
   
