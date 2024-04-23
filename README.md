*REFLECTION*
# Tutorial 8 - Publisher

a. In a single run, the publisher program sends five distinct messages to the message broker. This is determined by the fact that it invokes the "publish_event" function five times within its main function, each time with different data payloads.

b. The URL amqp://guest:guest@localhost:5672 being the same in both the publisher and subscriber programs indicates that they are configured to connect to the same AMQP server using identical connection parameters. Here's a breakdown:

amqp:// specifies that the AMQP protocol is being used for messaging.
guest:guest represents the credentials for authentication, with "guest" as both the username and the password.
localhost:5672 points to the host and port where the AMQP server is accessible, indicating that the server is hosted locally on the default AMQP port, 5672.

# Running RabbitMQ as message broker
<img width="1459" alt="Screenshot 2024-04-24 at 02 08 43" src="https://github.com/mariagrizelda/tutorial8-publisher/assets/134635504/3fb62ddf-0e8f-49d0-aa80-a40e44b7bced">

Essentially, the publisher sends messages to the RabbitMQ broker, and the subscriber retrieves and processes these messages, as seen on their respective consoles. This setup illustrates how data is transmitted from the publisher to the subscriber, with RabbitMQ serving as the intermediary.

<img width="1134" alt="Screenshot 2024-04-24 at 02 38 42" src="https://github.com/mariagrizelda/tutorial8-publisher/assets/134635504/5060f1f0-9f1c-4e13-8afc-a5afb1e47353">

The chart in the image displays the publisher's activity in terms of message transmission. By observing the 'message rates last minute,' it is possible to assess whether the publisher is experiencing a high or low load in message delivery. This information is useful for gauging the volume of messages being sent and processed.
<img width="1450" alt="Screenshot 2024-04-24 at 02 48 25" src="https://github.com/mariagrizelda/tutorial8-publisher/assets/134635504/8761a7f2-b116-46e1-b6d8-48195b70e527">
