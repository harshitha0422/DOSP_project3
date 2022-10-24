# Distributed Operating Systems Principle 
## Team Members:
Harshita Patel Velpula, ufid: 2765-9435</br>
Vishesha Sadu, ufid: 

## RUNNING THE PROGRAM:
- Create a node : erl -name <username>@//<IPAddress>` 

- Compile the chordserver file : `c(chordserver.erl).` 

- Begin the chordserver in the node : `chordserver:start(numNodes, numRequests).` 

Where, numRequests is the number of requests that each peer must make, and            numNodes is the number of peers that must be generated in the peer-to-peer system.


## PROBLEM DEFINITION:

Based on the Chord protocol, the Chord system provides an effective distributed lookup service. The single action that the Chord protocol permits is to identify, given a key, the node in charge of keeping track of the value of the key. The key/value pairs and entries in the routing table that point to a subset of carefully chosen Chord servers are kept in part by each node. The purpose of this project is to construct Erlang and demonstrate its utility using the actor model, the Chord protocol, and a straightforward object access service.

## WHAT IS WORKING:

The Chord protocol is used to achieve the following functionalities: 
- messaging between network nodes; 
- stabilizing the chord network whenever a node is added; 
- updating the finger table; and
- determining the average number of hops. 
- Add nodes to the network






