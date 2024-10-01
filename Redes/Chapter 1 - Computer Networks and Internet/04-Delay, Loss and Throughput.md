# Packet-Switched Networks
- A packet starts in a host, passes through a series of routers, and ends its journey in another host.
- As a packet travels from one node to the subsequent node along this path, the packet suffers from several types of delay at each node along the path.

## Processing Delay
- Time required to examine the packet's header and determine where to direct the packet.

## Queuing Delay
- The packets experiences a queuing delay as it waits to be transmitted onto the link.
- The lenght of the queuing delay of a specific packet will depend on the number of earlier-arriving packets that are queued and waiting for transmission onto the link.

## Transmission Delay
- Amount of time required to push all of the packet's bits into the link.
- Our packet can be transmitted only after all the packets that have arrived before it have been transmitted.

## Propagation Delay
- Once a bit is pushed into the link, it needs to propagate to router B.
- The time required to propagate from the beginning of the link to router B.
- Dependes on the physical medium of the link.
- Is the distance between two routers divided by the propagation speed.