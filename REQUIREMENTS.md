# Chord-P2P-System-and-Simulation-F#-Actor-Model-AKKA.NET

PROBLEM DEFINITION - 
We talked extensively in class about overlay networks and how they can be used to provide services.  The goal of this project is to implement Scala using the actor model the Chord protocol and a simple object access service to prove its usefulness. The specification of the Chord protocol can be found in the paperChord: A Scalable Peer-to-peer Lookup Service for Internet Applicationsby  Ion  Stoica,  Robert  Morris,  David  Karger,  M.  Frans  Kaashoek,  Hari  Balakrishnan. https://pdos.csail.mit.edu/papers/ton:chord/paper-ton.pdf (Links to an external site.).  You can also refer to the Wikipedia page: https://en.wikipedia.org/wiki/Chord(peer-to-peer) (Links to an external site.) The paper above, in section 2.3 contains a specification of the Chord API and of the API to be implemented by the application.

REQUIREMENTS - 
You have to implement the network join and routing as described in the Chord paper (Section 4) and encode the simple application that associates a key (same as the ids used in Chord) with a string.  You can change the message type sent and the specific activity as long as you implement it using a similar API to the one described in the paper.

Input: The input provided (as command line to yourproject3.scala) will be of the form:

project3 numNodes  numRequests
Where numNodesis the number of peers to be created in the peer-to-peer system and numRequests is the number of requests each peer has to make.  When all peers performed that many requests, the program can exit.  Each peer should send a request/second.

Output: Print the average number of hops (node connections) that have to be traversed to deliver a message.

ACTOR MODELLING - 
In this project, you have to use exclusively the AKKA actor framework (projects that do not use multiple actors or use any other form of parallelism will receive no credit).  You should have one actor for each of the peers modeled.

*README file In the README file you have to include the following mate-rial:*

Team members
What is working
What is the largest network you managed to deal with.
