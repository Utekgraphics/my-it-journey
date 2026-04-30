# my-it-journey
Daily logs of my self-taught IT journey towards Network Administration &amp; Forensics 🔐

# My IT Journey 🖥️

Hi! I'm documenting my journey from complete beginner to 
Network Administrator and Network Forensics specialist. 
Every day I learn something new and log it here publicly 
to stay accountable and hopefully inspire others on a 
similar path.

**Current Status:* Introduction to IT
**Goal:** CompTIA A+ → Network Administrator → Network Forensics
**Started:** April 2026

---

# 📅 Day 1 - Binary & Number Systems
# Date: 21st April 2026

### What I Learned:
- Every computer communicates using Base 2 (Binary) 
  - meaning it only understands 0s and 1s
- Every file on your device is measured in bytes 
  built entirely on this system
- The reason computers don't use Base 10 like humans 
  do is because it would make them significantly larger 
  and far more expensive to build
- There are 3 core number systems in IT:
  - Binary (Base 2)
  - Decimal (Base 10)
  - Hexadecimal (Base 16)
- Binary shows up everywhere in real life:
  - Machine code
  - Boolean logic (True/False)
  - Hardware states (On/Off)
  - Networking & File storage

### The Interesting Part 🤯
Quantum computers operate on higher bases and that 
is exactly what gives them the ability to process 
information so much faster and more powerfully than 
any regular PC. It's not magic, it's just a higher 
number system working at a completely different level.

### Binary to Decimal Example:
Binary 101 = Decimal 5

| Position | 2² | 2¹ | 2⁰ |
|---|---|---|---|
| Value | 4 | 2 | 1 |
| Binary digit | 1 | 0 | 1 |

4 + 0 + 1 = 5 ✅

---

# 📅 Day 2 - Inside the CPU
**Date:** 22nd April 2026

### What I Learned:
The CPU is the brain of every computer - it processes 
instructions and performs calculations. Inside the CPU 
there are three key components that work together:

| Component | Full Name | Role |
|---|---|---|
| CU | Control Unit | The boss - controls all CPU operations and gives instructions to every other component |
| ALU | Arithmetic & Logic Unit | Handles all calculations and logical operations e.g 1 + 2 = 3 |
| Register | Register | Tiny fast memory that temporarily holds information the CPU is currently working with |

### The Interesting Part 🤯
What looks like a simple computer is actually a 
perfectly organised system where every component 
knows its job and executes it without fail, every 
single second your computer is running.

---

## 🎯 Goals
- [ ] Complete Introduction to IT
- [ ] Start CompTIA A+ 
- [ ] Pass CompTIA A+
- [ ] CompTIA Network+
- [ ] Network Administrator role
- [ ] Network Forensics specialisation

---


## 📅 Day 3 - Data, Storage, RAM & Performance
**Date:** 23nd April 2026
*(Posted a day late — consistency over perfection!)*

### What I Learned:

#### Everything in a Computer is a Number
- Computers are digital - photos, music, text are 
  all represented as numbers
- All operations are a form of arithmetic
- Example: number 228 = 11100100 in binary
- Example: lowercase "j" = 01101010 in ASCII encoding

#### Bits & Bytes
- 8 bits = 1 Byte
- Byte is the standard unit of digital storage

| Unit | Size | Real World Example |
|---|---|---|
| Kilobyte (kB) | 1,000 Bytes | A typical email (~2kB) |
| Megabyte (MB) | 1,000² Bytes | A song (~5MB) or novel (~1.5MB) |
| Gigabyte (GB) | 1,000³ Bytes | A 1080p movie (~5GB) |
| Terabyte (TB) | 1,000⁴ Bytes | Entire major libraries |
| Petabyte (PB) | 1,000⁵ Bytes | All data held by a major tech company |

#### RAM vs Long Term Storage
- RAM (Random Access Memory) = short term, 
  extremely fast intermediate storage
- RAM speed: ~20,000 MBps
- RAM latency: ~10 nanoseconds
- SSD latency: a few microseconds (almost 1000x 
  slower than RAM)
- More RAM = faster and smoother performance

#### Throughput vs Latency
| Term | Definition |
|---|---|
| Throughput | Total amount of data transferred in a given time |
| Latency | The delay before data transfer begins |

#### CPU vs GPU Performance
- Both made up of cores performing one operation 
  at a time
- Both have set clock speeds determining how often 
  operations are performed
- Both measured in watts (energy consumption)
- More powerful devices = more energy = more heat generated

### Key Takeaway 🤯
RAM is almost 1000x faster than even the fastest SSD. 
That single fact explains why RAM matters so much 
for device performance.

### Status: ✅ Completed

---

## 📅 Day 4 - The Origin of the Internet
**Date:** Monday, 27th April 2026

### What I Learned:

#### ARPANET - Where It All Started
- Founded in **1969**, funded by the United States government
- Full name: **Advanced Research Project Agency Network**
- Purpose: Connect supercomputing centers run by 
  government agencies and universities
- This was the very first network, the earliest 
  form of what we now call the internet

#### TCP/IP - The Language of the Internet
- Full name: **Transmission Control Protocol / 
  Internet Protocol**
- Created to provide a **universal standard** for 
  how data is transferred across different networks
- Researched and developed throughout the **1970s**
- Officially adopted in the **early 1980s**

#### How the Internet Was Formed
| Year | Event |
|---|---|
| 1969 | ARPANET launched by US government |
| 1970s | TCP/IP researched and developed |
| Early 1980s | TCP/IP officially adopted |
| After 1980s | Different networks adopted TCP/IP and became interconnected — forming the internet |

### Key Takeaway 🤯
The internet was not invented by one person or one 
company. It evolved from a government funded university 
network into a global interconnected system through 
the adoption of a universal communication standard TCP/IP.

### Status: ✅ Completed

---

## 📅 Day 5 - WWW, Browsers, Servers & Networks
**Date:** Tuesday, 28th April 2026

### What I Learned:

#### The World Wide Web
- Invented by **Tim Berners-Lee in 1989**
- WWW = collection of interlinked websites 
  and web resources
- Important distinction:
  - **Internet** = the global infrastructure 
    (network of networks)
  - **WWW** = what sits on top of the internet 
    (websites, web resources)

#### Web Browsers
- Rose to popularity in the **1990s**
- Introduced a user friendly interface for 
  browsing multimedia content
- Allowed users to interact with each other online
- Transformed the internet from a technical tool 
  to something accessible to everyone

#### How a Browser Requests Data
- Browser sends a request to a server
- Data does not arrive all at once, it comes 
  bit by bit
- Order of loading:
  1. Text loads first
  2. Images follow after
- A single server can distribute data to numerous 
  computers simultaneously

#### What is a Network?
A network is two or more computers or devices 
linked together to share information.

#### Types of Networks
| Type | Full Name | Coverage |
|---|---|---|
| LAN | Local Area Network | Home, office or single building |
| CAN | Campus Area Network | Multiple buildings within a campus e.g university or hospital |
| WAN | Wide Area Network | Cities, countries and continents - the internet is the largest WAN |

### Key Takeaway 🤯
The internet and the World Wide Web are NOT the 
same thing. The internet is the infrastructure. 
The WWW is the collection of websites built on 
top of it. Tim Berners-Lee invented the WWW in 
1989 - one idea that changed how billions of 
people access information forever.

### Status: ✅ Completed
### Next: OSI Model

---

## 📅 Day 6 - The OSI Model
**Date:** Wednesday, 29th April 2026

### What I Learned:

#### What is the OSI Model?
- Full name: **Open Systems Interconnection Model**
- Developed in the **1970s and 1980s**
- A conceptual framework that breaks networking 
  into **7 separate layers**
- Each layer refers to a specific set of functions
- Each layer only communicates with the layer 
  directly above and below it

#### The 7 Layers

| Layer | Name | Key Function | Examples |
|---|---|---|---|
| 1 | Physical | Transmits raw bits over a medium | Ethernet cables (CAT5/CAT6), Bluetooth, Modem, Repeater |
| 2 | Data Link | Node to node transfer, MAC addressing | MAC addresses (48 bit), Switches, NIC, Wi-Fi |
| 3 | Network | Logical addressing and routing | IP addresses, Routers, Data centers |
| 4 | Transport | End to end communication, segmentation | TCP, UDP, Port numbers |
| 5 | Session | Opens, maintains and closes sessions | NetBIOS, APIs, Authentication, Video calls |
| 6 | Presentation | Data translation, encryption, compression | SSL/TLS, JPEG, PNG, MP4, ASCII |
| 7 | Application | Interface between user and network | HTTP, HTTPS, DNS, FTP, SMTP, Web browsers |

#### MAC Address Breakdown (Layer 2)
- Total: **48 bits**
- First 24 bits = Manufacturer identifier
- Last 24 bits = Device specific identifier

#### Memory Trick 😄
To remember all 7 layers in order:

> Please Do Not Throw Sausage Pizza Away

P = Physical
D = Data Link
N = Network
T = Transport
S = Session
P = Presentation
A = Application

### Key Takeaway 🤯
The OSI model is not just theory, every time 
you send a message, load a website or make a 
video call, all 7 layers are working together 
simultaneously to make it happen.

### Status: ✅ Completed

---

## 📅 Day 7 - The TCP/IP Model
**Date:** Thursday, 30th April 2026

### What I Learned:

#### What is the TCP/IP Model?
- A 4 layered conceptual model that describes 
  how data is transmitted across the internet
- More practical than the OSI Model - this is 
  what the internet actually runs on
- Each layer handles a specific set of functions

#### The 4 Layers

| Layer | Name | Key Function |
|---|---|---|
| 1 | Network Access | Sending and receiving data at local network level |
| 2 | Internet | IP addressing and routing |
| 3 | Transport | End to end communication via TCP and UDP |
| 4 | Application | Sessions, data translation and user interaction |

#### TCP vs UDP (Transport Layer)

| Protocol | Full Name | Type | How it works |
|---|---|---|---|
| TCP | Transmission Control Protocol | Connection oriented | Fixed channel, rigorous acknowledgement between sender and receiver |
| UDP | User Datagram Protocol | Connectionless | No fixed channel, lightweight, no acknowledgement required |

#### When to use TCP vs UDP
- **TCP** - File downloads, emails, web browsing 
  (accuracy matters more than speed)
- **UDP** - Video calls, live streams, online gaming 
  (speed matters more than perfection)

#### OSI vs TCP/IP Quick Comparison

| OSI Model | TCP/IP Model |
|---|---|
| 7 Layers | 4 Layers |
| Theoretical framework | Practical implementation |
| Application, Presentation, Session | Application |
| Transport | Transport |
| Network | Internet |
| Data Link, Physical | Network Access |

### Key Takeaway 🤯
TCP and UDP are not better or worse than each 
other — they serve different purposes. TCP 
prioritises accuracy. UDP prioritises speed. 
The internet needs both.

### Status: ✅ Completed

---
