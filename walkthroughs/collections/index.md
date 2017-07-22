### MongoDB Collections
----

[comment]: <> (List of Collections)

We define all new collections we've created in `lib/collections.js`.

```
Learnings = new Mongo.Collection("learnings");
Hangouts = new Mongo.Collection("hangouts");
Notifications = new Mongo.Collection('notifications');
RSVPnotifications = new Mongo.Collection("rsvp-notifications");
Comments = new Mongo.Collection('comments');
ArchivedUsers = new Mongo.Collection("archived-users");
Migrations = new Mongo.Collection("migrations");
```

### Users
The `users` collection is implicitly given to us by Meteor. Here's an example user: 
```
{
  "_id": "8iT63HQuAkq4gdP2K",
  "roles": {
    "CB": []
  },
  "profile": {
    "time_zone": "America/Indiana/Indianapolis",
    "time_zone_label": "Eastern Standard Time",
    "time_zone_offset": -18000,
    "firstname": "",
    "lastname": "",
    "avatar": {
      "default": "https://secure.gravatar.com/avatar/c347be2945fbc4f9a3a24f9f361d17d8.jpg?s=72&d=https%3A%2F%2Fa.slack-edge.com%2F66f9%2Fimg%2Favatars%2Fava_0015-72.png",
      "image_192": "https://secure.gravatar.com/avatar/c347be2945fbc4f3a4a24f9f361d17d8.jpg?s=192&d=https%3A%2F%2Fa.slack-edge.com%2F7fa9%2Fimg%2Favatars%2Fava_0015-192.png",
      "image_512": "https://secure.gravatar.com/avatar/c347be2945fbc4f3a4a24f9f361d17d8.jpg?s=512&d=https%3A%2F%2Fa.slack-edge.com%2F7fa9%2Fimg%2Favatars%2Fava_0015-512.png"
    }
  },
  "username": "phoenix_arrow20",
  "createdAt": "2017-03-05T06:57:42.429Z",
  "services": {
    "slack": {
      "id": "A44F76GMW",
      "accessToken": "[REDACTED]"
    },
    "resume": {
      "loginTokens": [
        {
          "when": "2017-05-07T02:22:34.811Z",
          "hashedToken": "[REDACTED]"
        },
        {
          "when": "2017-05-18T04:42:02.928Z",
          "hashedToken": "[REDACTED]"
        },
        {
          "when": "2017-07-22T19:49:00.536Z",
          "hashedToken": "[REDACTED]"
        }
      ]
    }
  },
  "email": "example_user@example.com",
  "status": {
    "online": true,
    "lastLogin": {
      "date": "2017-07-22T19:49:00.690Z",
      "ipAddr": "127.0.0.9",
      "userAgent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/59.0.3071.115 Safari/537.36"
    },
    "idle": false
  },
  "statusHangout": "collaboration"
}
```

### Learnings
```
{
  "_id": "CqMJRSX7ExauB9i2u",
  "title": "Learned how to exit vim!\n",
  "userId": "8iT63HQuAkq4gdP2N",
  "username": "ronald_weasley",
  "created_at": "2017-04-23T06:17:39.213Z",
  "hangout_id": "homepage",
  "kudos": 0
}
```

### Hangouts
```
{
  "_id": "MRmCDion3e9qCHf3Y",
  "topic": "\"Real Python\" Chapters on Web Interaction & Scientific Computing/Graphing",
  "slug": "\"real-python\"-chapters-on-web-interaction-&-scientific-computing/graphing",
  "description": "In this meeting, we will work through the Review Exercises in the latter half of\nthe \"Interacting with the Web\" section (1.14) of \"Real Python\" by Fletcher\nHeisler . This part of the chapter offers some techniques for interacting with\nweb forms and timed web scraping using Python.\n\n\n\nIf time permits, we will also begin to work on the next chapter, which deals\nwith Scientific Computing and Graphing.\n\n\n\nYou will need to obtain your own copy of The Real Python, and supporting files\nfor the exercises can be found here:\n\n\n\nhttps://github.com/realpython/book1-exercises\n\n\n\nAlso, for the next session, it is recommended that you install the Mechanical\nSoup, Numpy, SciPy and Matplotlib libraries. To do this with pip in Python 3,\nplease enter each of these commands into the Terminal/Power Shell:\n\n\n\npip3 install MechanicalSoup\n\npip3 install numpy\n\npip3 install scipy\n\npip3 install matplotlib",
  "description_in_quill_delta": {
    "ops": [
      {
        "insert": "In this meeting, we will work through the Review Exercises in the latter half of the \"Interacting with the Web\" section (1.14) of \"Real Python\" by Fletcher Heisler .  This part of the chapter offers some techniques for interacting with web forms and timed web scraping using Python.\n\nIf time permits, we will also begin to work on the next chapter, which deals with Scientific Computing and Graphing.\n\nYou will need to obtain your own copy of The Real Python, and supporting files for the exercises can be found here:\n\nhttps://github.com/realpython/book1-exercises\n\nAlso, for the next session, it is recommended that you install the Mechanical Soup, Numpy, SciPy and Matplotlib libraries.  To do this with pip in Python 3, please enter each of these commands into the Terminal/Power Shell:\n\npip3 install MechanicalSoup\npip3 install numpy\npip3 install scipy\npip3 install matplotlib\n"
      }
    ]
  },
  "start": "2017-07-22T19:49:00.000Z",
  "end": "2017-07-22T21:49:00.000Z",
  "duration": 120,
  "type": "collaboration",
  "host": {
    "id": "8iT63HQuAkq4gdP2K",
    "name": "legend27",
    "avatar": "https://secure.gravatar.com/avatar/c347be2945fbc4a9a4a24f9f361d17d8.jpg?s=72&d=https%3A%2F%2Fa.slack-edge.com%2F66f9%2Fimg%2Favatars%2Fava_0015-72.png"
  },
  "attendees": ["2iT63aaAkdq4gdP2K","ai3aaAkdq34gdP2K"],
  "users": [
    "8iT63HQuAkq4gdP2K"
  ],
  "day_reminder_sent": true,
  "hourly_reminder_sent": true,
  "views": 1,
  "visibility": true,
  "created_at": "2017-07-22T19:49:12.134Z"
}
```


### RSVPnotifications
```
{
  "_id": "mdYr7ucuihB7K4ybe",
  "hangoutId": "BSJyidFdy4k3H7Xfw",
  "createorId": "8iT63HQuAkq4gdP2K",
  "seen": false,
  "date": "2017-07-06T08:00:44.224Z",
  "count": 0
}
```

