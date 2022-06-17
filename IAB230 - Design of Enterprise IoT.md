# IAB230 Study Guide | 2022 Year 1 Semester 1

Written by Brook Jeynes (Chooky) using the QUT course content and many other sources
<br>

<h1>Table of Contents</h1>
<ul>
	<li><a href="#IAB230">IAB230: Design of Enterprise IoT</a></li>
	<ul>
		<li>Intro to the topic | Tips for the unit</li>
		<li><a href="#week1">Week 1</a>: Introduction to Enterprise IoT</li>
		<li><a href="#week2">Week 2</a>: IoT Methodology</li>
		<li><a href="#week3">Week 3</a>: IoT Devices</li>
		<li><a href="#week4">Week 4</a>: IoT Network</li>
		<li><a href="#week5">Week 5</a>: Fog and Cloud Computing</li>
		<li><a href="#week6">Week 6</a>: IoT System Deployment</li>
		<li><a href="#week7">Week 7</a>: Consolidation Week</li>
		<li><a href="#week8">Week 8</a>: Security and Privacy</li>
		<li><a href="#week9">Week 9</a>: </li>
		<li><a href="#week10">Week 10</a>: </li>
		<li><a href="#week11">Week 11</a>: </li>
		<li><a href="#week12">Week 12</a>: </li>
		<li><a href="#week13">Week 13</a>: </li>
	</ul>
</ul>

---

<br />

<h1 id="IAB230">IAB230: Design of Enterprise IoT</h1>
<p>This unit introduces the components of a mobile ubiquitous system, including stand alone and wearable sensors and wireless network protocols. It introduces the Internet of Things context and develops the skills in designing products and applications that use mobile and ubiquitous sensors and smart devices. The ability to critically review real case studies, expand awareness of interconnections between technologies, networks and user contexts and design a solution to a smart IT context problem is a requirement for a range of graduate positions. This is the first unit in the Mobile Application Development minor and builds on the skills that you developed in IFB103 IT Systems Design, and IFB104 Building IT Systems. IAB330 Mobile Application Development builds on this unit in which you design and build a working prototype system that uses mobile and ubiquitous system components.</p>

<br />

<h2 id="week1">Week 1: Introduction to Enterprise IoT</h2>

### IoT Essentials

IoT, also known as the Internet of Things, is the concept of a network of connected devices all sharing information with each other. This network can consist of many things such as: sensors, phones, computers and many more. At its core, any device connected to a network is an IoT device. IoT devices must have identifiers attached to them, whether this be internal identifiers, QR codes or device names. This allows us to identify which device is sending which information and allows us to individually interact with each device. We then use software to tie all these devices together to manage and support the IoT devices and to receive the data being sent.

Using sensors as an example:

- The sensors act as our IoT device
- Each sensor has an internal identifier or QR code on it so we can individually manage and or identify each device
- Each sensor sends data over the network to another device running software to capture that data
- And each device is connected to each other over the internet

There are four components IoT attempts to connect:

1. People
2. Data
3. Processes
4. Things (mobile devices, sensors, computers, watches)

These processes allow things to connect with each other over the internet to exchange and share data with different people and things.

IoT devices can be used in a variety of places and projects:

- Wearables: Fitbits, apple watches and more are all wearable IoT devices which help keep track of fitness, health and important information such as the time.
- Nest: Security cameras, smart lights and thermostats and home monitoring can all be accomplished using IoT nests (a collection of related IoT devices all working together)
- Roadside Lights: IoT devices can be used to save energy and reduce light pollution
- Smart Waste System: Notify management when bins are filled, rude operational costs by optimising collection schedules and routes

### IoT Framework

When we think about the framework of an IoT solution it's easier to break it down into 4 main categories.

1. IoT Applications: This refers to the specialised applications running on the management software
2. IoT Services Platform: This refers to the management software used to manipulate and communicate with the IoT devices used
3. IoT Network: This refers to the network and network devices that connect all IoT devices together
4. IoT Devices: This refers to the IoT devices used in the solution
5. Other: Agricultural, energy, mining, enterprise, finance, healthcare, industrial, retail, transportation, etc

### IoT Layered Architecture

As well as the framework we saw above we can also look at the architecture of an IoT app and break it down into 3 categories:

1. Cloud: This consists of dashboard, management and analytic applications. This layer relates to the Applications and Services Platform layer.
2. Edge: This consists of the pre-processing and filtering of the data before it gets sent to the dashboard applications This layer relates to the Services Platform and Network layer.
3. Devices: This consists of all the devices used whether that be sensors, routers or actuators. This layer relates to the Network and Devices layer.

### IoT Eco-systems

As we've seen we can use IoT devices for a wide variety of applications but who uses these implementations?

- Consumer (consumer based):
  - Vehicle: Autonomous vehicles
  - Health: Illness monitoring
  - Fitness: Health monitoring
  - Home: Energy management, smart lighting
  - Entertainment: Smart TV, google home
- Government (non-consumer based):
  - Surveillance: Security cameras
  - Energy/Utilities: Smart lights
  - Transport: Vehicle scheduling and management
  - Environment: Air monitoring, waste management
- Enterprise (non-consumer based):
  - Customers: Self-checkouts
  - Manufacturing of goods: Automated quality checks
  - Health: Emergency services

<br />

<h2 id="week2">Week 2: IoT Methodology</h2>

### Stages of an IoT Solution

An IoT solution general follows a cycle of 5 different steps. These steps all link forward and backwards to a step and continue in an infinite cycle detailing how our solution works.

1. Create
2. Communicate
3. Aggregate
4. Analyse
5. Act (then looping back to step 1 Create)

![[Screen Shot 2022-03-21 at 20.19.03.png]]

### Create

In our first step create, we create some type of data from an IoT device. This could be the creation of data from a sensor or a list of shopping items for a receipt when a credit card gets scanned.

### Communicate

The next step is communicate. This is when the data generated and created in the first step gets sent somewhere. This could be to a database or some analysis software.

### Aggregate

In our aggregate step we aggregate (or combine) all the data collected from our sources. This can be data sent from multiple IoT sensors in a project or a list of items bought from a store in a given day for stock checks.

### Analyse

We then analyse and work with the retrieved data. This could be to find patterns and relationships between data (such as which product is bought more at which store) or to provide future predictions from data (such as weather predictions).

### Act

Our final step in the process before we loop back is act. Now this step could be our final step or our first step depending on the action being taken. When we act we're either acting in response to our IoT device or acting to initiate a response from the IoT device. An example of an act initiating our process could be the scanning of items when shopping. We first act using our sensor to scan our items then causing the chain process described earlier. An example of an act being our final step could be in response to data retrieved from sensors. The data retrieved could say our crops are too dry and so we act to fix the problem shown from our data.

### IoT Methodology

When creating an IoT project we need to look at things from both an enterprise level and a project level. From an enterprise level, we need to make sure we first have an IoT strategy, that is to say, we need to have a strategy for the implementation of IoT devices in the business model. This means we need to make sure that the business model can support and actually successfully implement these IoT devices. We then need to create an IoT portfolio to manage and support the IoT projects and devices for the business. From a project level however, we need to create a plan to actually build, not only the sensors (building, programming, testing), but also an architectural model to support the sensors. After we've planned out our initial stages we can then start the process of building and testing our IoT solution. This step is iterative and can repeat as many times is felt needed by the development team to make sure all requirements are met and allow room for changes. Once everything is built to a standard we can then deploy our IoT devices into the project. It's important to note that just because the solution is deployed does not mean that we stop this iterative pattern of planning, building and testing.

### IoT Execution Strategy

When executing the creation of an IoT solution we can generally break the whole process down into 4 broad steps:

1. IoT strategy planning
2. IoT solution delivery
3. IoT centre of excellence
4. IoT platform

### IoT Strategy

In this step we are focusing on many of the pre-planning stages of the project. What our visions and goals are for the project and some guidelines to follow, budgeting and marketing including money management and investor meetings, portfolio management and tracking of the projects progress.

### IoT Solution Delivery

This step can essentially be broken up into 3 more smaller categories:

- IoT opportunity identification: This step is based around idea generation and refinement
- IoT opportunity management: This step is based around assessing the impacts and risks while also developing the business model
- Initiation: The final step here is the internal setup of the project.

### IoT Center of Excellence and IoT Platform

The final two levels in our strategy execution strategy is really based around consultation and the actual implementation of our IoT project. Here we setup any networking servers and finalise any standards that need to be followed as well as actually deploying our project into the world.

### PACT Analysis

PACT analysis is an analysis system we can step through when deciding and determining the requirements we may need for our IoT solution. There are many ways we can conduct a PACT analysis such as brainstorms, pictures, sketches, workshops with relevant users of the system or even user stories. It consists of 4 main steps:

1. People: In this step we analyse the different characteristics a person using our system has, whether physical, mental or social.
2. Activities: In this step we analyse the different activities the users using the IoT solution will need to undertake. We focus on the complexity, cooperation, safety, and how regular or infrequent the activity is.
3. Contexts: In this step we analyse the context of which the users undertake the activities in. We focus on the physical environments, social context and organisational context. For example, when designing an ATM we analyse the context and make sure not the place the machine in the sun to not obscure the screen.
4. Technologies: In this step we analyse the technologies and interactive systems of the IoT solution. We focus on the input, output, communication and content of the technology in our IoT solution.

<br />

<h1 id="week3">Week 3: IoT Sensors</h1>

### Sensors and Actuators

When we refer to the 'things' in our IoT solution we're really referring to two main components:

- Sensors: A device that detects events or changes in the environment around it. Used to identify and collect information for analysis, monitoring and diagnosis.
- Actuators: These convert signals into electrical signals to take some action when our sensor provides information or instructions. There are many types of actuators such as electrical, mechanical linear, hydraulic, pneumatic and manual.

Sensors will receive data from the world, process it, and then send it to an actuator which will then produce a desired action in the world.

### Simple and Smart Sensors

There are generally two types of sensors:

1. Simple sensors: These sensors are only designed to collect information and send it off over some network for analysis.
2. Smart sensors: These sensors are simple sensors with additional software to enhance them such as on-sensor data filtering.

There are many sensors used for multiple different reasons. We can break these up into 4 main categories:

1. Pressure sensors: Pressure sensors measure pressure or touch. These are most commonly seen in touchscreens.
2. Flow sensors: Flow sensors measure liquid metrics. These can be found in many places such as brewing machines used to detect and record the rate of fluid flow.
3. Imaging sensors: Imaging sensors are used to capture image data and are used in cameras, medical imaging machines and night vision equipment.
4. Noise sensors: Noise sensors measure the sound produced from their environment. These can be used for many things such as noise pollution measuring.

### RFID

RFID, or Radio Frequency Identification, is a two part wireless system composed of a tag and a reader. The reader is a small device that sends out radio waves and receives signals back from the RFID tags. These are typically used in traffic toll machines ad smart scan systems.

### Video Tracking

Video tracking is the process of capturing and analysing video feeds of certain locations, objects or people of interest. We can use it to measure and analyse movements, visual attention, behaviour and much more. A major weakness of this system however is how time consuming the analysis phase can be due to the software needing to, in most circumstances, analyse frame by frame.

### Smart Cards

Smart cards are generally hard plastic cards that contain microprocessors on them that enable two-way communication, on-board computing and a small amount of storage for information. These work similar to how RFID tags work in the sense that a reader sends out a radio frequency that activates the chip in the card causing a signal from the card to be sent back to the reader.

<br />

<h1 id="week4">Week 4: IoT Network</h1>

### IoT Security and Privacy

Due to the wide range of ways IoT solutions are being implemented it's a no surprise that there have been people trying to compromise the security of these devices. The range of severity security attacks on IoT devices have can be insignificant to catastrophic damage and may even result in the loss of life if the correct device is compromised.

Current encryption and authentication protocols have two major problems when it comes to their incorporation into IoT devices:

1. Protocols are extremely resource hungry and demand higher capabilities from the chips present in IoT devices.
2. The authentication and authorisation protocols used are high-touch. This means that they require a lot of user input for provisioning and configuring the authentication details.

### IoT Connection

There are many ways we can connect sensors and IoT devices together over a network. Depending on the needs of the IoT solution the incorporation of networking devices such as hubs, gateways, routers, network bridges, switches and more are very common. The first step we need to take before we transfer information from an IoT device over the internet is to uniquely identify each devices on said network. We can use networking protocols to set rules to define how these devices identify each other.

### IoT Protocol Stack

When looking at the IoT protocol stack we generally used a slightly modified version of the OSI model.

| Layer       | Main function                                                            | Example of main devices | example of main protocol |
| ----------- | ------------------------------------------------------------------------ | ----------------------- | ------------------------ |
| Application | Provides network services and applications to the user                   | Server, Computer        | HTTPS                    |
| Transport   | Establishes a connection and transmits data using transmission protocols | Firewalls               | TCP, UDP                 |
| Network     | Decides which path the data will take upon transmission                  | Routers                 | IPv4, IPv6               |
| Data Link   | Defines the format the data will take upon transmission                  | Switches                | IEEE 802.1 (Ethernet)    |

### Link Layer Challenges

There are many challenges we may face when implementing the link layers in our IoT protocol stack. One of the challenges that may be faced is the fact that network communication is resource and power hungry at times. This is a problem due to the fact that for most IoT solutions the IoT devices are low-powered devices which don't have much on-board processing. Another problem we may face is time-sensitive data constraints. This means that, depending on the needs of the system, the IoT devices may need to be able to send highly accurate data without buffering or delays. The range of which devices can connect is also a challenge that may be faced. Depending on the solution data may need to be sent a really long distance or a short distance but either way the data still needs to be accurate and delivered in a timely fashion. The last set of challenges that are generally faced is the scalability of the IoT solution. IoT solutions may only start off with a small amount of devices but see themselves growing in the future. It is important that the scalability of the network can adapt and change to suit the needs of the devices connected.

### IoT Network Terminologies

It's important we understand the terminologies and shorthands used when describing networking means.

- LAN: Local Area Network
- WAN: Wide Area Network
- FAN: Field Area Network
- PAN: Personal Area Network
- NAN: Neighbourhood Area Network
- IEEE 802.15.4: A technical standard defining the operation of a low-rate wireless PAN
- LPWAN: Low Power Wide Area Network (uses a long-range star topology)
- FFD: Full Function Device
- RFD: Reduced Function Device
- LTE (Long Term Evolution): A standard for wireless broadband communication for mobile devices.
- NB-IoT: Narrowband IoT
- 6LoWPAN: IPv6 over Low-power Wireless Personal Area Networks

### Network Topologies

There are three main network topologies used depending on the needs of the IoT solution.

1. Star: A network topology where all devices communicate through a single central controller. ![An introduction to network topology - Cablify](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.cablify.ca%2Fwp-content%2Fuploads%2F2018%2F04%2FStar-Topology.jpg&f=1&nofb=1)
2. Mesh: A network topology where all devices can communicate with each other (peer-to-peer). ![Network Diagram Drawing at GetDrawings | Free download](https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fgetdrawings.com%2Fimages%2Fnetwork-diagram-drawing-2.png&f=1&nofb=1)
3. Cluster Tree: A network topology where devices are chained to each other. In the centre of the chain is a PAN coordinator. ![6 Best Network Topologies Explained - Pros & Cons ...](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fcdn.comparitech.com%2Fwp-content%2Fuploads%2F2018%2F11%2FTree-Topology.jpg&f=1&nofb=1)

### Network Layer Challenges

Most IoT solutions use low-power and lossy networks (LLN) and these come with their own set of challenges when working with the network layer. Due to networking being some-what resource heavy we find our IoT devices draining their battery and power faster. It's because of this that we need to incorporate a sleep/awake cycle solution to optimise the rate at which our devices consume energy. Another challenge we may face is the fact that the links in an LLN can be unreliable at times with varying time and packet loss characteristics.

### Low-Power Wireless Technology Comparison

|              | Wi-Fi                                 | Bluetooth                         | ZigBee                                 | 6lowPAN                                |
| ------------ | ------------------------------------- | --------------------------------- | -------------------------------------- | -------------------------------------- |
| Network      | LAN                                   | PAN                               | LAN                                    | LAN                                    |
| Topology     | Star                                  | Star                              | Mesh, star, tree                       | Mesh, star                             |
| Data Rate    | Up to 1.4Gbps                         | 2.1mbps                           | 250kbps                                | 200kbps                                |
| Range        | Up to 100m                            | < 100m                            | 10-20m                                 | 10-20m                                 |
| Application  | Any device with cellular connectivity | Network for data exchange headset | Sensor networks, Industrial automation | Sensor networks, Industrial automation |
| Network Size | Medium                                | Small                             | Very large                             | Very large                             |

<br />

<h1 id="week5">Week 5: Fog and Cloud Computing</h1>

### Cloud Layer

The cloud is a model that attempts to provide users with access to computer resources over a network that are scalable, sharable and accessible at all times. There are three main types of cloud services:

1. Infrastructure as a service (IaaS)
2. Platform as a service (PaaS)
3. Software as a service (SaaS)

We can think of these 3 types as a pyramid that builds itself up with each layer targeting a different users.

| Layer | Title | Targeted Users      | Example of Product                             |
| ----- | ----- | ------------------- | ---------------------------------------------- |
| 1     | SaaS  | End users           | Gmail, Salesforce CRM, Office 365, Google Docs |
| 2     | PaaS  | Software developers | Google App Engine, Heroku                      |
| 3     | IaaS  | IT administrators   | Microsoft Azure, Google compute engine         |

### Infrastructure as a Service (IaaS)

With IaaS, IT infrastructure is rented out on a pay-as-you-go basis from a cloud provider. This service includes services such as servers, virtual machines, online storage, networks, online operating systems and more.

### Platform as a Service (PaaS)

PaaS refers to cloud computing services that can supply an on-demand environment for developing, testing, delivering, and managing software applications. PaaS is designed to make it easier for developers to create web and mobile applications without the need to worry about setting up or managing the accompanying infrastructure that comes along with it. Servers, storage, network and databases are such things generally included in PaaS.

### Software as a Service (SaaS)

SaaS refers to actually providing the software itself as a service over the cloud to an end user. With SaaS, cloud providers host and manage the software application and all underlying infrastructure (including maintenance such as software upgrades and security patching). Users connect to these applications through web browsers on their devices such as phones, tablets and PC's.

### Edge/Fog Layer

The fog layer is a platform that sits between the cloud and the data source. It attempts to bring cloud computing functions closer to where the data is actually being produced or consumed. The fog layer provides computing, storage and network services within the proximity of the IoT devices.

Cloud computing is not always a viable option for IoT devices because the amount of data generated by the IoT devices would be too costly and time consuming. Fog computing attempts to reduce the bandwidth needed by these devices and reduce the back-and-forth communication between sensors and the cloud. These two things are very important in an IoT solution as speed and performance are usually extremely important factors.

By using the fog in combination with the cloud we can create an application that can sustain its speed and performance when analysing data but still provide long term analysis of data. The IoT devices/sensors don't have to computer and store all the resources obtain, they can send this data directly to the fog for short term fast analysis. This new collection of aggregated and analysed data can then be sent to the user and the cloud to provide long term storage and analysis so the data in the fog can then be cleared to allow for new data.

Benefits of fog:

- Cope with vast volumes of large and fast data
  - Filter and triage data for better insight
  - Take action on data in real-time
- Strengthen security and ensure compliance
  - Reduce the exposed attack surface
  - Make the edge more technically robust
- Improve reliability and availability
  - Remove the points of network failure
  - Minimize the application downtime

### Fog vs Cloud Layer

| Fog                                                                                              | Cloud                                                                   |
| ------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------- |
| Receive feeds from IoT devices using any protocol (in real time)                                 | Receives and aggregates data summaries from many fog nodes              |
| Run IoT-enabled applications for real-time control and analytics, with millisecond response time | Performs analysis on the IoT data and data from other sources           |
| Provide transient storage, often 1-2 hours                                                       | Can send new application rules to the fog nodes based on these insights |
| Send periodic data summaries to the cloud                                                        |                                                                         |

|                             | Fog                                  | Cloud                                    |
| --------------------------- | ------------------------------------ | ---------------------------------------- |
| Response Time               | Seconds to minutes                   | Minutes to days to weeks                 |
| Application Examples        | Visualisation, simple analytics      | Big data analytics, Graphical dashboards |
| How long IoT data is stored | Short duration: hours, days or weeks | Long duration: months or years           |
| Geographical Coverage       | Wide area (field or building)        | Global                                   |

| Requirements                    | Cloud Computing | Fog Computing  |
| ------------------------------- | --------------- | -------------- |
| Latency                         | High/Medium     | Low            |
| Location of service             | Within internet | Network edge   |
| Distance between data resources | Multiple hops   | Single hops    |
| Geographical distribution       | Centralised     | Distributed    |
| Number of nodes                 | Large           | Larger         |
| Support for mobility            | No              | Yes            |
| Data analytics                  | Data at rest    | Data in motion |

<br />

<h1 id="week6">Week 6: IoT System Deployment</h1>

<br />

<h2 id="week7">Week 7: Consolidation Week</h2>

<br />

<h2 id="week8">Week 8: Security and Privacy</h2>

### Security

Security is, at its core, creating counter measures to overcome threats and attacks on some system. We are generally protecting and securing the privacy of some data whether that be confidential documents, personal information or just information we don't want leaked. It's extremely important to consider security and privacy when developing an IoT solution. This is because in our IoT solution, it only takes a single device to be compromised to, in most cases, gain access to all other nodes and devices connected to the compromised device. We need to always be considering:

- What can you do to protect the data?
- Who's responsible to ensure privacy and security of data?
- What happens if things go wrong?
- What is the effect if the data is leaked?
- How can we prevent these malicious attackers

These IoT devices are collecting large amounts of information and data each day and a compromised device leaking this data could be catastrophic. Think about how much data wearable devices collect? Devices like smart watches are collecting information such as your location, environmental data, sleep patterns and much more. IoT medical devices are collecting much more privacy-sensitive information and if exposed or compromised could be disclosed to third-parties or worse.

When handling devices which collect information about the user it's important to:

1. Give the individual a choice of sharing the information or not.
2. Not overcomplicate the way these systems are designed and display these options of users to select. The system should be straight forward and up-front to the user about what settings they can and can't change.
3. Notify individuals whose information is used or sold to third parties.
4. Ensure to the user any information taken off-site will be updated and remain correct. These should abide the legal frameworks provided by existing privacy policies.
5. Provide the user a location to go or a person to contact if any of the legal obligations in regards to privacy are breached. The user should know who they can contact and when.

### IoT Security Challenges

There are a couple main security challenges we face when developing IoT solutions.

1. Multiple Technologies: Each technology used in the solution has different vulnerabilities and each vendor has a different way of addressing them.
2. Multiple Verticals: The security requirements for each vertical (i.e. eHealth, industrial) are vastly different from each other.
3. Scalability: An IoT solution must be scalable and cost-efficient and thus our privacy and security solutions must also be able to scale efficiently.
4. Big Data: An IoT solution may intake large amounts of data every day. Our solution needs to be able to efficiently secure large streams of data from various devices all at a single time.
5. Availability: Our security measures must be operational 100% of the time and are a high priority that they stay this way.
6. Resource Limitations: We must make sure our security is efficient but also do able on our IoT device. Many devices have limited resource capabilities and we must take this into account when considering security options.
7. Remote Locations: Many IoT verticals require IoT devices to be secured in unmanned locations that are difficult to reach.
8. Delay-Sensitive Service: We must make sure that our devices are secure from attacks that will delay or degrade the service time or cause disruptions in the data flow.
9. Mobility: Some sensors are expected to change location from time to time. It's important we account for this movement of environments when developing security and privacy systems.

### Security and Data Solutions

There are a few things we can do to prevent a majority of the attacks on our devices.

1. Make sure our devices do not have a single point of failure and can adjust if a node fails or is attacked.
2. When retrieving address and objects containing confidential information the user must be authenticated to prove who they are. By limiting access to only authenticated or specific users we can minimise the range of attacks and affects of compromised accounts.
3. We can provide access control to data essentially only allowing certain user groups to have access to certain data.

### IoT Security Requirements

We must make sure that our IoT device, at a minimum, follows these requirements:

1. Confidentiality of data: Only the sender and intended receiver should be able to understand the information/message being sent. By doing this we can make sure any man in the middle attacks are met with encrypted data that is useless without a key.
2. Integrity: We must be able to confirm that the data being sent has not been tampered with in any way. With integrity we can confirm that the data we are receiving is the data that was sent.
3. Authentication: By authenticating users we can validate that they are who they say they are. This can cut down on an attackers ability to impersonate someone and gain access to our systems that way.
4. Availability: We must also make sure that the service is always available. We must protect our servers and devices from DNS attacks or any attack that could affect the availability of the content.
5. Non-repudiation: Once an entity proceeds with an action we must make sure that they cannot take back what they have done. By providing non-repudiation, we can make sure that a secure transaction is never reverted or that an entity cannot deny their actions.
6. Freshness: We must always make sure that the data is fresh and that there exists no outdated or stale information floating around in our system.

### Cloud Domain Vulnerabilities

A cloud domain could be hosting ten to hundreds of VM's a day. It's because of this that security is a top priority for these providers. There are many risks that come along with this business model such as:

- Lots of different companies applications could be running on the same physical system. A compromise of this system could result in a compromise in every other VM hosted on this system.

There are however many countermeasures applied in such a business model. One of the main countermeasures is isolating VM's. By doing this, a single compromised VM can not bring down the whole network. 

### Cloud Domain Attacks
Here are a few of the most popular security attacks in the cloud domain.

#### Hidden-Channel Attacks
Hidden channel attacks occur when a VM leaks data into another VM. The typical strategy for attack with this vulnerability occurs is:
1. Locate the target VM that is leaking data
2. Rent a VM and find the internal IP address of the target VM. This is generally done via a query to the DNS server to identify which server the target VM resides on
3. Rent a VM located in that server
4. Cross-VM data leakage via malicious data in the shared data and instruction cache

There are a few ways we can counter this attack:
1. Randomise the cluster location on initial VM rental
2. Prevent VM's from issuing probing packets such as `trace_route`
3. Hard Isolation - Each VM has a separate cache
3. Flush and refresh the cache on hand-over to a new VM

#### VM Migration Attacks
- A migration flooding attack occurs when more VM's than a server can support are moved into the server. This overload causes a DNS attack on the server.
- A false resource advertisement attack occurs when a server advertises spare resources. This can attract other services to offload VM's to the new server, this gaining access and control over these migrated VM's.
- Data plane attacks can occur in multiple ways but generally what happens is when a VM is moved from one server to another a sniffing attack or man-in-the-middle attack occurs and the attacker can read, store, and pass the VM back along the network like nothing happened.

#### Theft of Services Attack
This attack occurs when a malicious VM is assigned more resources than it needs limiting other VM's and degrading their services.

### Cloud Domain Attacks Overview

| Attack                  | Vulnerability Reason                                                                                           | Security Violation                       | Countermeasures                                                                                       |
| ----------------------- | -------------------------------------------------------------------------------------------------------------- | ---------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| Hidden-Channel Attack   | Shared hardware components among the server's VM's                                                             | Confidentiality                          | - Hard Isolation - Cache Flushing - Noisy Data Access Time - Limiting Cache Switching Rate            |
| VM Migration Attacks    | - VM Migration software bugs - VM Migration is performed without authentication - Memory pages copied in clear | Confidentiality, Integrity, Availability | - Server authentication - Encrypting migrated memory pages                                            |
| Theft of Service Attack | Periodic sampling of VM's used resources                                                                       | Availability, Non-Repudiation            | - Fine grain sampling using high precision clocks - Random sampling                                   |
| VM Escape Attack        | Hypervisor software bugs                                                                                       | Confidentiality, Availability, Integrity | Add an isolation domain between the hypervisor and hardware                                           |
| Insider Attacks         | Lack of trsut in the cloud administrators                                                                      | Confidentiality, Integrity               | - Homomorphic Encryption - Secret storage through data chopping and permutation based on a secret key |

### Fog Domain Attacks
Fog devices act on sensor data through many means such as:
- Collection
- Aggregation
- Pre-processing
- Providing intermediate storage
- and many more

However, due to the high similarities between the fog and the cloud, the fog typically becomes susceptible to most, if not all, cloud domain attacks.

On top of all the cloud domain attacks the fog also becomes susceptible to a few other specific attacks such as:
- Location attacks: Due to the sensors typically being in plain sight there is an increased risk of physical damage or access
- Mobility: Due to the fog device being mobile, it could be moved closer to the sensor leading to increased risk of data access
- Lower computing power: Due to these devices having low power and low computing resources there are less resources to provide for stronger security protocols or mechanisms
- Authentication and Trust Issues: The identity of the fog device owner can be faked.
- Higher migration security risks
- Higher vulnerability to DoS attacks
- Privacy issues: Most transmissions are sent through in plain text rather than being encrypted

### Sensing Domain Attacks
There are many popular attacks that can occur in the sensing domain:
- Jamming attacks: Stopping the sending/receiving of data from/to an IoT device
- Vampire attack
- Selective-forwarding attack
- Sinkhole attack

#### Transmission Jamming
Transmission jamming occurs when the information being sent to and from an IoT device is blocked. There are many types but the most common are
- Constant
- Deceptive
- Reactive
- Random

Some countermeasures that could be applied to this attack could be:
- Frequency hopping
- Spread spectrum: The conversion of narrow band signals to wide band
- Directional Antennae
- Jamming detection and suppression

#### Vampire Attacks
Vampire attacks occur when an IoT device is forced to consume more power and resources than it should. This can occur in a variety of ways such as:
- Denial of sleep: Sending a control signal to the IoT device to prevent it from sleeping
- Flooding attacks: Flooding the server nodes with dummy data
- Carousel attacks: The exploitation of the OSI stack to circulate data
- Stretch attack: The exploitation of the OSI network stack to send data through the longest route possible rather than the shortest

#### Selective Forward Attack
This attack occurs when a malicious node captures some data and blocks it from being sent further, This can cause for holes in the data at the server endpoint.

#### Sinkhole Attack
This attack occurs when a malicious node claims to be the closest one, capturing and dropping some, or all, of the received data.

| Attack                  | Target OSI Layer   | Vulnerability Reason | Security Violation  | Countermeasures   |
| ----------------------- | ------------------- | -------------- | ------------------------- | --- |
| Hidden-Channel Attack   | Shared hardware components among the server's VM's                                                             | Confidentiality                          | - Hard Isolation - Cache Flushing - Noisy Data Access Time - Limiting Cache Switching Rate            |
| VM Migration Attacks    | - VM Migration software bugs - VM Migration is performed without authentication - Memory pages copied in clear | Confidentiality, Integrity, Availability | - Server authentication - Encrypting migrated memory pages                                            |
| Theft of Service Attack | Periodic sampling of VM's used resources                                                                       | Availability, Non-Repudiation            | - Fine grain sampling using high precision clocks - Random sampling                                   |
| VM Escape Attack        | Hypervisor software bugs                                                                                       | Confidentiality, Availability, Integrity | Add an isolation domain between the hypervisor and hardware                                           |
| Insider Attacks         | Lack of trsut in the cloud administrators                                                                      | Confidentiality, Integrity               | - Homomorphic Encryption - Secret storage through data chopping and permutation based on a secret key |