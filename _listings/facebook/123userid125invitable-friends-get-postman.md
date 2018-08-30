{
  "info": {
    "name": "Facebook Get User Invitable Friends",
    "_postman_id": "0b35f024-9d59-4c5f-ab1d-2c1cad590615",
    "description": "User Invitable Friends",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Test",
      "item": [
        {
          "id": "f4002e41-f523-4134-b094-ea3563310884",
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
              "id": "9598a415-a12b-414e-88db-021c9b665934"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "c7a28318-cf3d-45ca-9745-2c894dd1b83d",
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
              "id": "e017aba9-ac0b-49a4-a5ac-ccd9712ed1b2"
            }
          ]
        }
      ]
    }
  ]
}