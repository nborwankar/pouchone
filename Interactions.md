/**
 * Created by nitin on 12/27/15.
 */

Peer Bootstrap
--------------

A peer with a PouchDB instance is initialized by creating the databases mentioned in Storage.md
An initialized "peer-to-be" connects to a canonical bootstrap URL and pull-replicates the bootstrap record
and a list of peer-groups

Bootstrap record contains

a url for the root database (initially identical to bootstrap database but can be different after bootstrap)
a set of operations exposed to the outside, described via triple of (url, input json, output json)
a list of databases

Peer-group list

contains a list of groups and policies for joining
initially all groups are closed by default except the bootstrap group which contains all peers in the pouch_1 realm




Interactions

Poll for messages

Push messages





