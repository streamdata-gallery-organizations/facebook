{
  "info": {
    "name": "Facebook Get User S For Business",
    "_postman_id": "8ffacd5e-ffbc-44cd-8cfa-982ebf108892",
    "description": "User IDs for Business",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "b603e177-9db7-4507-a453-c5239da85b52",
          "name": "getUserBusinessActivities",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/business_activities?100=100",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Business Activities"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45684c67-0097-4964-8bf7-a721d4cb2b07"
            }
          ]
        },
        {
          "id": "2635f2ac-7ea2-4094-b619-960b79d8d14c",
          "name": "getUserBusinesses",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/businesses?permitted_rolesliststring=permitted_rolesliststring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Businesses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd97f30a-b116-4bb0-9b79-a7d0c3426409"
            }
          ]
        },
        {
          "id": "78b1370f-6e23-4b23-8e74-959cafc136e5",
          "name": "getUserSForBusiness",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/ids_for_business?100=100&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User IDs for Business"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f97c7b6f-07e9-43d5-8f28-3ce71afdbac0"
            }
          ]
        }
      ]
    }
  ]
}