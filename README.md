*REFLECTION*
# Tutorial 8 - Publisher

a. In a single run, the publisher program sends five distinct messages to the message broker. This is determined by the fact that it invokes the "publish_event" function five times within its main function, each time with different data payloads.

b. The URL amqp://guest:guest@localhost:5672 being the same in both the publisher and subscriber programs indicates that they are configured to connect to the same AMQP server using identical connection parameters. Here's a breakdown:

amqp:// specifies that the AMQP protocol is being used for messaging.
guest:guest represents the credentials for authentication, with "guest" as both the username and the password.
localhost:5672 points to the host and port where the AMQP server is accessible, indicating that the server is hosted locally on the default AMQP port, 5672.

# Running RabbitMQ as message broker
<img width="1459" alt="Screenshot 2024-04-24 at 02 08 43" src="https://github.com/mariagrizelda/tutorial8-publisher/assets/134635504/3fb62ddf-0e8f-49d0-aa80-a40e44b7bced">
