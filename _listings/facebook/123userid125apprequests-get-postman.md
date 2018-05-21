{
  "info": {
    "name": "Facebook Get User Apprequests",
    "_postman_id": "b0ee199e-c4ec-47a3-aebc-0f205212cb8a",
    "description": "User Apprequests",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "e2815a63-fb7f-4463-878f-1e423353555f",
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
              "id": "3d512fdc-53d3-4481-bc17-c844d700476e"
            }
          ]
        }
      ]
    }
  ]
}