{
  "info": {
    "name": "Facebook Get User Favorite Requests",
    "_postman_id": "b656d683-7b7b-4c5c-b6d3-0260e2cce143",
    "description": "User Favorite Requests",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "6df491d5-1951-4ef4-bac0-8281fa8ceda5",
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
              "id": "402232e8-8deb-4e1d-91e2-5a38f47eb151"
            }
          ]
        },
        {
          "id": "d4f6bf88-893f-4e81-8a9c-d9c23066c42b",
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
              "id": "0fe98c77-5715-4773-9152-508a275db77f"
            }
          ]
        }
      ]
    }
  ]
}