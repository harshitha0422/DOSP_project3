# Distributed Operating Systems Principle 
## Team Members:
Harshita Patel Velpula, ufid: 2765-9435</br>
Vishesha Sadu, ufid: 2956-6305

## RUNNING THE PROGRAM:
- Create a node : `erl -name <username>@<IPAddress>` 

- Compile the chordserver file : `c(chordserver.erl).` 

- Run start method in chordserver module with appropriate arguments : `chordserver:start(numNodes, numRequests).` 

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

## WHAT IS THE LARGEST NETWORK YOU MANAGED TO DEAL WITH

Average hops count = total hops count / total number of requests

The largest network we managed to deal with is for 70,000 nodes with an average hops
count of 6.99 

## OBSERVEATIONS:

As the total number of nodes entering the network increased, so did the average number of hops.</br>

As the number of requests from each node to the same network increased, the average number of hops decreased.





