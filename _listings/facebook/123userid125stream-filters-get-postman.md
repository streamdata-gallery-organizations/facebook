{
  "info": {
    "name": "Facebook Get User Stream Filters",
    "_postman_id": "dacd0aa0-a965-4327-b5de-0e6728581680",
    "description": "User Stream Filters",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "238ff04c-fe94-4c92-a6b4-50c18c6e62d5",
          "name": "getUserStreamFilters",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/stream_filters?200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Stream Filters"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31dcf54b-9a13-408a-a5bc-1a21ef4e1237"
            }
          ]
        }
      ]
    }
  ]
}