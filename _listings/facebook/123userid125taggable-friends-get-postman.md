{
  "info": {
    "name": "Facebook Get User Taggable Friends",
    "_postman_id": "6ee175fe-9ef8-42b7-8383-fc8ae91e1863",
    "description": "User Taggable Friends",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Test",
      "item": [
        {
          "id": "2a2272e0-d4cc-4737-9437-4913ab26eadb",
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
              "id": "29a4e151-c8b5-4ab2-b087-25c3597b2407"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "3e15cda6-f651-4e76-81b9-a4c9eb991167",
          "name": "getUserInvitableFriends",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/invitable_friends?100=100&110=110&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Invitable Friends"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ccec37cb-d00c-419b-9488-1145f3d844e7"
            }
          ]
        },
        {
          "id": "4e0683b7-090a-49ca-9786-9e894178d4f6",
          "name": "getUserTaggableFriends",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/taggable_friends?100=100&110=110",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Taggable Friends"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a024902-0952-4e17-8579-36c6111a320d"
            }
          ]
        }
      ]
    }
  ]
}