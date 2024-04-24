a. what is amqp?

AMQP (Advanced Message Queuing Protocol) is an open standard application layer protocol for message-oriented middleware, allowing applications to communicate in a way that is reliable, secure, and efficient.

b. what it means? guest:guest@localhost:5672 , what is the first quest, and what is the second guest, and what is localhost:5672 is for?

`guest:guest@localhost:5672` is a typical format used to represent connection parameters to an AMQP server. The first `guest` is the username. The second `guest` is the password. `localhost:5672` specifies the hostname or IP address and port number of the AMQP server. When connecting to an AMQP server, those values must be replaced with the appropriate credentials and server information.

- Simulation slow subscriber
![](static/Screenshot%202024-04-24%20140217.png)
My total number of queue reach around 40. That is because the intentional delay that makes the thread sleep for 1 second and running the publisher app several times quickly thus making the queued messages to spike up significantly.