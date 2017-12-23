# Architecture
The first point of contact is an nginx server running on an EC2 instance.
This provides a reverse proxy to a (Node.js app)[https://github.com/robertoloja/SmartHive-RPi]
and a (Django app)[http://github.com/robertoloja/bookInventory]. As the Node
app is running outside of its intended context (a beehive), the data is mocked.
