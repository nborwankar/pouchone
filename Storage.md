/**
 * Created by nitin on 12/27/15.
 */


dbs = { # these are a set of couchdb databases that are in each pouch_1 node
    "main": "pouch_1",  # all docs that are not messages or attachments
    "inbox": "in",
    "outbox": "out",
    "attachments_in": "att_in",
    "attachments_out": "att_out",
    "address_book": "abook"
}