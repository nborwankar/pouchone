/**
 * Created by nitin on 12/27/15.
 */

PouchOne
========

PouchOne is a placeholder name.

PouchOne is a technology for rebooting early-Internet-style distributed communication using modern technology, specifically JSON based message
formats and HTTP based interactions.

More important-sounding-ly:-

PouchOne is a fabric of protocols (message formats and interactions) to facilitate hub-less communication between trusted parties,
in any or all of 1-1, 1-n, m-n modes.

PouchOne does not build infrastructure technologies but uses existing proven technologies to build an overlay network.
Hence all innovation in PouchOne is intended to be in the upper layers.

Why?

The early Internet consisted of a number of not-Web protocols and was based on trust between independently operated peers and peer domains.

USENET was an early Internet application based on NNTP and other protocols.  It was based on peering and store/forward.

And trust. Between server peers.

Email was another early Internet protocol based first on UUCP and then DNS + SMTP.  It was also based on peering and store/forward.

And trust. Between server peers.

We now have web based discussions and web-based email and mobile messaging and cloud-based everything. And yet, from an interpersonal communications point of view,
something has been lost.

Trust.

We have delegated trust to mega-hubs and have been disappointed to various degrees.
Trust can no longer be assumed from hubs, and so even the network cannot be trusted.
Mega-hubs that hold, route and process communication have eroded any expectation of communications privacy,
which they have done primarily for business reasons.

And yet the need to communicate, 1-1, 1-n and m-n, remains and is a fundamental part of human social existence.
Mega-hub message topologies driven by economies of scale are not necessarily natural topologies for all human communication,
We cannot all be asked to gather in a giant single location (FB/Gmail/Twitter) whenever we want to talk, connect and collaborate
with a person or small group.

How to fix this?  Technologies exist to regain some of the lost flavor, but we need to rethink some of this anew and operate
it as a non-commercial  entity until we have worked out the details of how to avoid the mistakes of the past two decades.


What?

PouchOne is a mega-hub-free substrate for spontaneous loose collaboration between distributed groups with minimal set-up overhead.
Pairwise and group communications can be easily setup and dissolved without need for "permission" from an admin or vendor and need for
new identities and accounts on multiple mega-hubs.
Small-group communications can be fully meshed (hub-less) or with a human-consensus-elected mini-hub or with trusted intermediaries.

How?


Interactions

PouchOne peer (server) level interactions are implemented via HTTP-based JSON message transfer between peer nodes (control messages)
These are usually generated and consumed by machines.

PouchOne application level communication is achieved by the HTTP-based JSON message transfer between address endpoints (interpersonal messages)
These are usually created and consumed by humans.  Address endpoints are abstractions that may or may-not be tied to any particular peer.

Peers are not assumed to be online at all times. Temporary message stores are implemented using "CouchDB API compliant" databases.


Message Formats

PouchOne aims to enable simple flexible message format and exchange standards that are "almost-obvious".
PouchOne messages are weak imitations of MIME message types, embodied in JSON objects.
  All MIME types are NOT represented in PouchOne. Exhaustive translation of all MIME formats to JSON is an explicit non-goal.

Technology

PouchOne uses the brilliant PouchDB in the browser and PouchDB Server in the cloud.
(However we encourage others to implement the server side using other CouchDB compatible implementations, while adhering to
message and interaction standards)

PouchOne uses the following technologies from CouchDB/PouchDB

* bi-di replication (message exchange for protocol and )
* JSON storage in database (store for forwarding, inbox, outbox, forum groups)
* subset of CouchDB's REST-ful API
* document id's and revisions - to track versions of config documents

====

Inspirations:
MIME
SMTP
JXTA
Usenet

