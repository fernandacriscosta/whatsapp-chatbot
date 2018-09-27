WhatsApp Chatbot
================

webhook
-------
```
{
  "messages": [
    {
      "from": "91XXXXXXXXXX",
      "id": "ABEGkZUDJVmVAgo-sLp9pUGxXuVe",
      "text": {
        "body": "start"
      },
      "timestamp": "1537263693",
      "type": "text"
    }
  ]
}

{
 "messages": [
   {
     "from": "91XXXXXXXXXX",
     "id": "ABEGkZhzABQGAhBPeMjHS2v6fHwEyJhAoiTS",
     "image": {
       "file": "/usr/local/wamedia/shared/014d/4293/130b45998a19438abdfc6610",
       "id": "014d4293-130b-4599-8a19-438abdfc6610",
       "mime_type": "image/jpeg",
       "sha256": "4ca1d8cde4c1fc706b34f746d9afc4a84e77df6af3506d5e47484f5fa77d9098"
     },
     "timestamp": "1537262673",
     "type": "image"
   }
 ]
}

{
    "context": {
         "from": "sender_wa_id_of_context_message",
         "group_id": "group_id_of_context_message",
         "id": "message_id_of_context_message",
         "mentions": [ "wa_id1", "wa_id2" ]
    },

    "from": "sender_wa_id",
    "group_id": "group_id",
    "id": "message_id",
    "timestamp": "message_timestamp",
    "type": "audio | document | image | location | system | text | video | voice",

    # If there are any errors the errors field (array) will be present.
    # The errors field can be returned as part of any callback event.
    "errors": [ { ... } ],
    
    "audio": {
        "file": "absolute_filepath_on_coreapp",
        "id": "media id",
        "link": "link to audio file",
        "mime_type": "media mime type",
        "sha256": "checksum"
    }

    "document": {
        "file": "absolute_filepath_on_coreapp",
        "id": "media id",
        "link": "link to document file",
        "mime_type": "media mime type",
        "sha256": "checksum",
        "caption": "document caption"
    }

    "image": {
        "file": "absolute_filepath_on_coreapp",
        "id": "media id",
        "link": "link to image file",
        "mime_type": "media mime type",
        "sha256": "checksum",
        "caption": "image caption"
    }

    "location": {
        "address": "1 hacker way, menlo park, ca, 94025",    
        "latitude": latitude,
        "longitude": longitude,
        "name": "location name"
    }
    
    "system": {
        "body": "system message content"
    }
    
    "text": {
        "body": "text message content"
    }

    "video": {
        "file": "absolute_filepath_on_coreapp",
        "id": "media id",
        "link": "link to video file",
        "mime_type": "media mime type",
        "sha256": "checksum"
    }
    
    "voice": {
        "file": "absolute_filepath_on_coreapp",
        "id": "media id",
        "link": "link to audio file",
        "mime_type": "media mime type",
        "sha256": "checksum"
    }
}
```
