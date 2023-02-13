# Loeng 13. veebruar.

# communication protcol
just rules is just rules

# Rule establishment

source and destination must have established rules before info is sent

Protocols myst account for the following req.

1) An identified sender and receiver
2) Common language and grammar
3) Speed and timing of delivery
4) Confirmation of acknowledgement req.


# Requirements

1) Message encoding

    Turning info into a data type that can be transmitted
    After receiving info it must be turned back to original data type - decoding

    bits are either converted either pattern of light, sound, or electrical impulses.


2) Message formatting and encapsulation

![Alt text](Screenshots/Screenshot%202023-02-13%20085132.png)


3) message size

    When a long mnessage is sent from one host  to another over a network, it is necessary to break the message into smaller pieces.
    The rules that govern the size of the pieces, or frames, communicated across network are very strict.
    They can also be different, depending on the channel used.


4) Message timin

    1) Flow control - manages the rate of data transimssion and defines how much information can be sent and the speed at which it can be delivered.
    2) Reponse timeout - Manages how long a device waits when it does not hear a reply from the the destination.
    3) Acess method - Determines when someone can send a message.


5) Message delivery options

    if message is for one person for the set of people or for everyone.


# network Protocol functions

## Function - Description

### Addressing - identifies sender and receiver
### Reliability - Provides quaranteed delivery
### Flow control - Ensures data flows at an efficient rate
### Sequencing - Uniquely laberls each transmitted segment of data
### Error Detection - Determines if data became corrupted during transmission
### Application Interface - Process-to-process communication between network application

# Protocol interaction

## Protocol - Function
### HTTP - 
    Governs the way web server and a web client interact. Defines content and format

### Transimssion on Control Protocol (TCP) - 
    Managed the individual conversations. Provides quaranteed delivery. Manages flow control
### Internet Protocol (IP) - 
    Delivers message globally from the sender to the receiver.
### Ethernet - 
    Delivers messages from one NIC to another NIC on the same Ethernet Local Area Network (LAN).
# Network protocol Suites

### Protocols must be able to work with the other protocols.

### Protocol suite:
    1) A group of inner relater protocols necessary to perform a communication function
    2) Sets of rules that work together to help solve a problem

### Protocol stack:
    Protocol stack shows how the individual protocol withing a suite a implemented

### The protocols are viewed in therm of layers:
    Higher or upper Layers
    Lower layers-concerned with moving data and provide services to upper layers

# Evolution of Protocol Suites

### Internet Protocol Suite or TCP/IP
    The most common protocol suite and maintaine by the internet Engineering Task Force (IETF) in 1970s
### Open Systems Interconnection (OSI) protocols
    Developed by the International Organization of Standardization (ISO) and the internation Telecommunications Union (ITU) in 1977. Replaced by TCP/IP
### AppleTalk
    Proprieatry suite release by Apple Inc. in 1995 TCP/IP was adopted to replace AppleTalk
### Novell NetWare
    Proprietary suite developed by Novell Inc. in 1995 TCP/IP was adopted to replace IPX

# TCP/IP Protocol Suite

### TCP/IP is the protocol suite used by the internet and includes many protocols.


### TCP/IP:
    An open stadard protocol suite that is freely available to the public and can be used by any vendor
    A standards-based protocol suite that is endorosed by the networking industry and approved by a standards organization to ensure interoperability

# Standards Organizations

## Open Standards
### Encourage -
    Interoperability
    competition
    innovation
### They are:
    vendor-neutral
    non-profit organizations 
    established to develop and promote concept of open standards

# Data encapsulation

## Segmenting messages

### Segmenting
    The process of breaking up messages into smaller units
### Multiplexing
    The processes of taking multiple streams of segmented data and interleaving(mixing) them together.

### Segmenting messages has two primary benefits:
    Increase speed - Large amounts of data can be sent over the nework without tylng up a communictions link

### Increases efficiency
    Only segments which fail to reahc the desitnation need to be retransmitted. not the entire data stream.

# Physical Layer Characteristics

## Physical components

### Physical Layer Standards address three functional areas:
    Physical Components
    Encoding
    Signalin


### Encoding
    # Encoding converts the stream of bits into a format recognizable by the next device in the network path
    # This "coding" provides predictable patterns that can be recognized by the next device.
    # Examples of encoding methods includes Manchester(shown in the figure), 4B/5B and 8B/10B

![Alt text](Screenshots/Screenshot%202023-02-13%20105025.png)

### Signaling

    # The signaling method is how the bit values, "1" and "0" are represented on the physical medium
    # The method of signaling will vary based on the type of medium being used

### Bandwidth
#### Band - Frequency
#### width - how wide is the fequency

## Analogue bandwidth
    # Freguency range used to transmit an analogue signal like radio and TV broadcasting.
    # Uses continues values that are more suseptible to noise and distortion.
    Also reffered to as broadband
## Digital bandwidth
    # The amound of data that can be transmitted over a digital communication channel.
    # Uses discrete values of 0 and 1 and transmitted with less noise and distorion
    Also reffered to as baseband

### Bandwidth and speed
#### bandwidth and speed are used interchangeably, but they are two different things
    # Fiber optic = Fastest speed (light) and highest bandwidth
    # Copper = Medium speed (electricity), medium bandwidth
    # Wireless = Slowest speed (electromagnetic waves), lowest bandwidth
### Bandwidth Terminology
    # Latency - Amount of time, including delays, for data to travel from one given point to another.
    # Throughput - The measure of the transfer of bits across the media over a given period of time
    # Goodput - The measure of usable data transferred over a given period of time

![Alt text](Screenshots/Screenshot%202023-02-13%20111430.png)


## Copper Cabling
### Characteristics of Copper Cabling
#### Copper cabling is the most common type of cabling used in networks today. It is expensive, easy to install, and has low resistance to electrical current flow.

### limitations
    # Attenuation - the longer the electrical singals have to travel, the weaker they get.
    # Susceptible to interference from electromagnetic Interference (EMI) and Radio Frequency Interference (RFI) and Crosstalk.
    # Crosstalk - Crosstalk is a disturbance caused by the electric magnetic fields of a signal on one wire to the signal in an adjacent wire.
### Mitigation
    # Strict adeherence to cable length limits will mitigate attenuation.
    # Some kinds of copper cable mitigate EMI and RFI by using metallic shielding and grounding
    # Some kinds of copper cable mitigate crosstalk by twisting opposing circuit pair wires together.

![Alt text](Screenshots/Screenshot%202023-02-13%20112421.png)

![Alt text](Screenshots/Screenshot%202023-02-13%20112500.png)

### Unshielded Twisted Pair (UTP)
#### UTP has four pair of color-coded copper wires twisted together and encased in a flexible plastic sheath
#### No SHielding is used UTP relies on the following properties to limit crosstalk.
    # Cancellation - Each wire in a pair of wires uses opposite polarity. One wire is negative. the other wire is positive. They are twisted together and magnetic fields effectively cancel each other and outside EMI/RFI
    # Variation in twists per foot in each wire - Each wire is twisted a different amount, which helps prevent crosstalk amongst the wires in the cable
![Alt text](Screenshots/Screenshot%202023-02-13%20113525.png)
### Shielded Twisted Pair (STP)

    # Better noise protection than UTP
    # More expensive than UTP
    # Harder to install than UTP
    # Terminated with RJ-45 connectors
    # Interconnects hosts with intermediary network devices

#### Key Characteristics of STP
    # The outer jacket protects the copper wires from physical damage
    # Braided or foil shield provides EMI/RFI protection
    # Foil Shield for each pair or wires provides EMI/RFI protection
    # Color-coded plastic insulation electrically isolates the wires from each other and identifies each pair













