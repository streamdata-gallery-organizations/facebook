{
  "info": {
    "name": "Facebook Get Me Friendrequests",
    "_postman_id": "ab73850a-11e6-40fc-b641-1697369d0fc0",
    "description": "A person&#039;s pending friend requests.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "d0343e15-84e4-4a16-965f-7eb70a69801b",
          "name": "getUserApprequests",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/apprequests?100=100&159=159&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Apprequests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55289948-6849-440a-9e55-e11f5a737028"
            }
          ]
        },
        {
          "id": "806e820b-bf96-4859-a0b7-a749b24ffcfc",
          "name": "getUserFavoriteRequests",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/favorite_requests?100=100&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Favorite Requests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e07143d3-f691-4aca-bbb1-ecdb15359411"
            }
          ]
        }
      ]
    },
    {
      "name": "Me",
      "item": [
        {
          "id": "7f9245e9-39be-491f-ac04-2c2dec054b88",
          "name": "getMeFriendrequests",
          "request": {
            "url": "http://graph.facebook.com/v3.0/me/friendrequests?created_time=created_time&from=from&message=message&to=to&unread=unread",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A person&#039;s pending friend requests."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9073612-3cc0-434b-97b6-3afe5deff2a6"
            }
          ]
        }
      ]
    }
  ]
}