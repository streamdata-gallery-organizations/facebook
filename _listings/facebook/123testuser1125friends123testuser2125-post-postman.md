{
  "info": {
    "name": "Facebook Post Test User 1 Friends Test User 2",
    "_postman_id": "5d177f7b-67be-4cb3-928a-a32fb86ac8b7",
    "description": "The friends of a test user. This is identical to the /&#123;user-id&#125;/friends edge aside from the publishing operation explained below.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Test",
      "item": [
        {
          "id": "d7f064ab-32e0-44e3-9e20-1dd827861724",
          "name": "postTestUser1FriendsTestUser2",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;test-user-1&#125;/friends/&#123;test-user-2&#125;",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The friends of a test user. This is identical to the /&#123;user-id&#125;/friends edge aside from the publishing operation explained below."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d0c0100-12a4-485f-a89a-4f98f885c4bd"
            }
          ]
        }
      ]
    }
  ]
}