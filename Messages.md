/**
 * Created by nitin on 12/27/15.
 */



msg_header = {
    "From": "%s",
    "To": "%s",
    "Date": "%s",
    "Subject": "%s"
}


bcast_header = {
    "From": "%s",
    "ToList": "%s", # list of recipient addresses
    "Date": "%s",
    "Subject": "%s"
}

forum_header = {
    "Topic": "%s",
    "Date": "%s",
    "Author": "%s"
}

text_body = {
    "content": "%s"  # value is utf-8
}

attachments = { # initially there is an arbitrary fixed limit of 3 attachments per message but this is only advisory.
    "1": "%s",  # value is base64-encoded blob
    "2": "%s",  # value is base64-encoded blob
    "3": "%s"   # value is base64-encoded blob
}

addr = {
     "fullname": "%s", # any non-null string - can be a nickname
     "username": "%s", # non-null, unique
     "pouch_1_url": "%s", # non-null, your pouch_1 base URL
     "twitter": "%s", # non-null  needed for identity verification
     "email": "%s" # can be null
}

envelope_entry= {
        ">From": "%s"
        }

envelope = {
        "entries": [] # envelope entries
        }


msg structure
        {
          {envelope},
          {hdr},
          {body},
          {attachments}
        }

hdr = msg_hdr for 1-1 messages
hdr = bcast_hdr for 1-n messages
hdr = forum_hdr for m-n messages

envelope, body and attachments are not dependent on whether a message is of type msg, bcast or forum
