---
title: Factors that affect the performance of networks
author: Nikky Leone
date: 2022-09-09 20:55:00 +0800
categories: [Year 7, Computers]
tags: [factors that affect performance]
---

By the end of this lesson, you will be able to:

- Identify things that affect how well a network performs
- Explain how they impact performance
- Suggest ways to improve network performance 


# Factors

**Network performance is about response time - how fast a message can be sent or how quickly a document can be retrieved.** The performance of a network can be affected by various factors:

- the number of devices on the network
 - the bandwidth of the transmission medium
 - the type of network traffic
 - network latency
 - the number of transmission errors
 - Any network can be affected by one or a combination of these factors.

**Bandwidth is a measure of the amount of data that the medium can transfer over a given period of time.** Each transmission medium has a different bandwidth:



| Medium                       | Typical brandwith                  | 
|:-----------------------------|:-----------------------------------|
| Twisted copper wire          | Up to 1 gigabit (Gb) per second    | 
| Fibre-optic cable            | Over 40 terabits (Tb) per second   | 
| Wi-Fi                        | About 54 megabits (Mb) per second  |
| Business Wi-Fi               | Up to 1 gigabit per second         |


**Each connected device requires bandwidth to be able to communicate. The bandwidth of the medium is shared between each connected device.** For example, **a home Wi-Fi network with one device would allocate 54 Mb per second to that device. If a second device joins the network, the bandwidth would be split between the two, giving 27 Mb per second to each, and so on.** If ten devices were connected, the bandwidth allocated to **each device would drop to 5.4 Mb per second, thereby reducing the rate at which data can be sent to any particular device.**

> In reality, however, things are more complicated. **Different types of network traffic usually have different bandwidth requirements. For example, streaming a high definition video requires more bandwidth than streaming a low definition video.** **Some network switches are capable of determining the type of traffic and adjusting the bandwidth allocated to a particular device to accommodate the traffic's requirements.**
{: .prompt-info }



# Latency

**Network latency is a measure of how long it takes a message to travel from one device to another across a network. A network with low latency experiences few delays in transmission, whereas a high latency network experiences many delays. The more delays there are, the longer it takes to transmit data across a network.**

Latency is affected by the number of devices on the network and the type of connection device.

**A hub-based network will usually experience higher latency than a switch-based network because hubs broadcast all messages to all devices.** Switch-based networks transmit messages only to the intended recipient.

**The greater the number of devices connected to a network, the more important the choice of transmission medium becomes. Wi-Fi generally handles less traffic than twisted copper wire (TCW), which in turn handles less traffic than fibre-optic cable.** Many networks include a combination of all three media:

- fibre-optic cables allow high data transmission between different buildings
- TCW runs from switches within buildings to individual devices
- Wi-Fi allows guest devices to connect to the network


# Transmission errors

**Inevitably there will be times when devices try to communicate with each other at the same time. Their signals collide with each other and the transmission fails.** It is similar to when two people speak to each other simultaneously - neither person is able to clearly hear what the other person is saying.

> A collision occurs when two devices on a network try to communicate simultaneously along the same communication channel.
**The greater the number of devices on a network, the more chance of a collision occurring, and the longer it takes to transmit a message**.
{: .prompt-tip }
