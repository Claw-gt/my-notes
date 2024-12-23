The Syslog protocol separates the:
- *Software that generates messages*
- *System that stores them*
- *Software that reports and analyzes messages*

### Syslog layers

- **Content**: storage location for syslog messages
- **Application**: handles message generation, interpretation, routing, and storage
- **Transport**: manages transport of syslog messages

### Syslog key players

#### The Originator

The location where the event occurs
- Creates the **facility code** and the **severity level**
The Syslog client adds:
- The originator process ID
- The timestamp
- The device hostname of IP address

<img src="https://itexamanswers.net/wp-content/uploads/2019/06/2019-06-17_155206-1024x612.jpg">

#### The Collector
The Syslog server collects the messages
#### The Relay Server
Forwards messages from the originator to the collector
#### The Transport Sender
Prepares messages for transport
#### The Transport Receiver
Receives and delivers messages to the Syslog server