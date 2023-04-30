---
toc: true
comments: true
layout: post
title: Computers and Networks (Unit 4)
description: Add Definitions from Unit 4 Computer Systems and Networks
categories: []
type: ap
week: 29
---

## Requirements
> Work through College Board Unit 4... blog, add definitions, and pictures.  Be creative, for instance make a story of Computing and Networks that is related to your PBL experiences this year.


### How a Computer Works
> As we have learned, a computer needs aa program to do something smart.  The sequence of a program initiates a series of actions with the computers Central Processing Unit (CPU). This component is essentially a binary machine focussing on program instructions provided.  The CPU retrieives and stores the data it acts upon in Random Access Memory (RAM). Between the CPU, RAM, and Storage Devices a computer can work with many programs and large amounts of data.

List specification of your Computer, or Computers if working as Pair/Trio
- Processor GHz: 3.30
- Memory in GB: 32
- Storage in GB: 951
- OS: windows and ubuntu

Define or describe usage of Computer using Computer Programs. Pictures are preferred over a lot of text.  Use your experience.
- Input devices
> - These are devices that allow users to input data or commands into a computer. Examples include a keyboard, mouse-pad, microphone, and scanner/webcam.
- Output devices
> - These are devices that allow a computer to communicate information back to the user. Examples include a monitor, printer, and speakers.
- Program File
> - A program file is a file that contains instructions for a computer program to execute. Examples include an executable file (.exe), a script file (.sh), and a batch file (.bat).
- Program Code
> - Program code is a set of instructions written in a programming language that tells a computer what to do.
- Processes
> - A process is a program that is currently running on a computer.
- Ports
> - A port is a physical interface on a computer that allows it to connect to other devices. Examples include USB ports, HDMI ports, and Ethernet ports. Ports
- Data File
> - A data file is a file that contains information that can be used by a computer program. Examples include a text file (.txt), a spreadsheet file (.xls), and an image file (.jpg).
- Inspect Running Code
> - Inspecting running code allows programmers to monitor the behavior of their programs as they run.
- Inspect Variables
> - Inspecting variables allows programmers to view the current values of variables in their programs.


![Computer Hardware]({{site.baseurl}}/images/cpu.jpeg)


### The Internet
> Watch/review College Board Daily Video for 4.1.1

- Essential Knowledge
    - A computing device is a physical artifact that can run a program. Some examples include computers, tablets, servers, routers, and smart sensors.
    - A computing system is a group of computing devices and programs working together for a common purpose.
    - A computer network is a group of interconnected computing devices capable of sending or receiving data.
    - A computer network is a type of computing system. 
    - A path between two computing devices on a computer network (a sender and a receiver) is a sequence of directly connected computing devices that begins at the sender and ends at the receiver.
    - Routing is the process of finding a path from sender to receiver.
    - The bandwidth of a computer network is the maximum amount of data that can be sent in a fixed amount of time.
    - Bandwidth is usually measured in bits per second

- Complete Vocabulary Matching Activity.  Incorporate this into your learnings from year.  To analyze measure path and latency use `traceroute` and `ping` commands from Linux Terminal.  
    - Path 
    > - A sequence of directly connected computing devices that begins at the sender and ends at the receiver.
    - Route
    > - The process of finding a path from sender to receiver.
    - Computer System
    > - A group of computing devices and programs working together for a common purpose.
    - Computer Device
    > - A physical artifact that can run a program, such as a computer, tablet, or smart sensor.
    - Bandwidth
    > - The maximum amount of data that can be sent in a fixed amount of time.
        Computer Network - A group of interconnected computing devices capable of sending or receiving data.

> Watch/review College Board Daily Video 4.1.2

- Complete True of False Questions

- Essential Knowledge
    - The internet is a computer network consisting of interconnected networks that use standardized, open (nonproprierary) communication protocols.
    - Access to the internet depends on the ability to connect a computing device to an internet connected device.
    - A protocol is an agreed-upon set of rules that specify the behavior of a system.
    - The protocols used in the internet are open, which allows users to easily connect additional computing devices to the internet.
    - Routing on the internet is usually dynamic; it is not specified in advance
    - The scalability of a system is the capacity for the system to change in size and scale to meet new demands.
    - The internet was designed to be scalable
    - Information is passed through the internet as a data stream. Data streams contain chunks of data, which are encapsulated in packets. 
    - Packets contain a chunk of data and metadata used for routing the packet between the origin and the destination on the internet, as well as for data reassembly.
    - Packets may arrive at the destination in order, out of order, or not at all
    - IP, TCP and UDP are common protocols used on the internet.
    - The world wide web is a system of linked pages, programs, and files.
    - HTTP is a protocol used by the world wide web
    - The world wide web uses the internet

- Go over AP videos, vocabulary, and essential knowledge.  Draw a diagram showing the internet and its many levels. A preferred diagram would using your knowledge of frontend, backend, deployment, etc.  Picture would highligh vocabulary by illustration. The below illustration have some ideas

![Full Stack]({{site.baseurl}}/images/fullstack.png)


- Often we draw pictures of machines communicating over the Internet with arrows.  However, the real communication goes through protocol layers and the machine and then is trasported of the network.   For College Board and future Computer Knowledge you should become familiar with the following ...

```
     User Machine  <---> Frontend Server <---> Backend Server
    +-----------+         +-----------+         +-----------+
    |  Browser  |         |  GH Page  |         |   Flask   |
    +-----------+    ^    +-----------+    ^    +-----------+
    |    HTTP   |    |    |    HTTP   |    |    |    HTTP   |
    +-----------+    |    +-----------+    |    +-----------+
    |    TCP    |    |    |    TCP    |    |    |    TCP    |   
    +-----------+    |    +-----------+    |    +-----------+
    |     IP    |    V    |     IP    |    V    |     IP    |
    +-----------+         +-----------+         +-----------+
    |  Network  |  <--->  |  Network  |  <--->  |  Network  |
    +-----------+         +-----------+         +-----------+
```

The "http" layer is an application layer protocol in the TCP/IP stack, used for ***communication between web browsers and web servers***. It is the protocol used for transmitting data over the World Wide Web.

The "transport" layer (TCP) is responsible for providing reliable data transfer between applications running on different hosts.  The TCP protocol segments the data into smaller ***chunks called "segments"***. Each segment contains a sequence number that identifies its position in the original stream of data, as well as other control information such as source and destination port numbers, and checksums for error detection.

The "ip" layer is responsible for packetizing data received from the TCP layer of the protocol stack, and then ***encapsulating the data into IP packets***. The IP packets are then sent to the lower layers of the protocol stack for transmission over the network.

The "network" layer is responsible for ***routing data packets between networks*** using the Internet Protocol (IP). This layer handles tasks such as packet addressing and routing, fragmentation and reassembly, and ***network congestion*** control.


### Fault Tolerance
> Watch both Daily videos for 4.2

- Complete the network activity, summarize your understanding of fault tolerance.
> - Fault tolerance is the ability of a system to continue operating in the event of a hardware or software failure. It involves designing a system in such a way that it can detect and recover from errors or failures without causing disruption or data loss. Fault tolerance can be achieved through a variety of techniques such as redundancy, replication, and graceful degradation.

### Parallel and Distributed Computing
> Review previous lecture on Parallel Computing and watch Daily vidoe 4.3.  Think of ways to make something in you team project to utilize Cores more effectively.  Here are some thoughts to add to your story of Computers and Networks...

- What is naturally Distributed in Frontend/Backend archeticture?  
>  - In a frontend/backend architecture, the frontend is typically distributed naturally across multiple clients, such as web browsers or mobile devices. Each client runs its own instance of the frontend code and interacts with the backend over the network.

On the other hand, the backend is usually centralized and runs on one or more servers. The backend code typically handles tasks such as data storage, processing, and business logic, and serves data and functionality to the frontend clients over the network.
- Analyze this command in Docker: ```ENV GUNICORN_CMD_ARGS="--workers=1 --bind=0.0.0.0:8086"```.   Determine if there is options are options in this command for parallel computing within the server that runs python/gunicorn.  Here is an [article](https://medium.com/building-the-system/gunicorn-3-means-of-concurrency-efbb547674b7)


> Last week we discussed parallel computing on local machine.  There are many options.  Here is something to get parallel computing work with a tool called Ray.
- Review this [article](https://www.anyscale.com/blog/writing-your-first-distributed-python-application-with-ray)...  Can you get parallel code on images to work more effectively?  I have not tried Ray.

- Code example from ChatGPT using squares.  This might be more interesting if nums we generated to be a lot bigger.

```python
import ray

# define a simple function that takes a number and returns its square
def square(x):
    return x * x

# initialize Ray
ray.init()

# create a remote function that squares a list of numbers in parallel
@ray.remote
def square_list(nums):
    return [square(num) for num in nums]

# define a list of numbers to square
nums = [1, 2, 3, 4, 5]

# split the list into two parts
split_idx = len(nums) // 2
part1, part2 = nums[:split_idx], nums[split_idx:]

# call the remote function in parallel on the two parts
part1_result = square_list.remote(part1)
part2_result = square_list.remote(part2)

# get the results and combine them
result = ray.get(part1_result) + ray.get(part2_result)

# print the result
print(result)

```

```python

import ray
import numpy as np
from PIL import Image

ray.init()

# Define a function to process a single image tile
@ray.remote
def process_tile(tile):
    # Do some image processing on the tile
    processed_tile = np.mean(tile, axis=-1)
    return processed_tile

# Load the image and break it up into tiles
image = Image.open('my_image.jpg')
tile_size = (256, 256)
tiles = [np.array(image.crop((x, y, x+tile_size[0], y+tile_size[1]))) 
         for x in range(0, image.width, tile_size[0]) 
         for y in range(0, image.height, tile_size[1])]

# Process the tiles in parallel using Ray
results = ray.get([process_tile.remote(tile) for tile in tiles])

# Combine the processed tiles into a single output image
output = np.vstack([np.hstack(row) for row in np.split(results, image.height // tile_size[1])])
output_image = Image.fromarray(output.astype(np.uint8))

# Save the output image
output_image.save('processed_image.jpg')

```