{
  "info": {
    "name": "Facebook Get Achievement Type",
    "_postman_id": "4bbfe258-a870-4187-be60-e542c848c029",
    "description": "A games achievement type created by a Facebook App. Not to be confused with an instance of an achievement.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Object",
      "item": [
        {
          "id": "1e29b781-be2b-45ff-99cc-209e31723aa7",
          "name": "getObjectComments",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;object-id&#125;/comments?order=order&total_count=total_count",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This reference describes the /comments edge that is common to multiple Graph API nodes. The structure and operations are the same for each node. The following objects has a /comments edge:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b08834e0-fc9c-4e90-85a7-68bfc1be9403"
            }
          ]
        },
        {
          "id": "b3aad4be-e6d4-4a94-8318-0e7282421927",
          "name": "postObjectComments",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;object-id&#125;/comments?attachment_id=attachment_id&attachment_url=attachment_url&message=message&source=source",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "This reference describes the /comments edge that is common to multiple Graph API nodes. The structure and operations are the same for each node. The following objects has a /comments edge:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09c6d890-8f37-465f-8884-0d4b1ab359a5"
            }
          ]
        },
        {
          "id": "cd274d74-7694-4386-a724-175982cef42a",
          "name": "getObjectLikes",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;object-id&#125;/likes?total_count=total_count",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This reference describes the /likes edge that is common to multiple Graph API nodes. The structure and operations are the same for each node, except that for the following nodes, /likes returns only the profile for the current user if read with a user access token:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c77faac8-ed11-47c4-8d8d-e61999abef34"
            }
          ]
        },
        {
          "id": "61d81e6f-ea92-4792-bf48-3abacaa25226",
          "name": "postObjectLikes",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;object-id&#125;/likes",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "This reference describes the /likes edge that is common to multiple Graph API nodes. The structure and operations are the same for each node, except that for the following nodes, /likes returns only the profile for the current user if read with a user access token:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "318accfb-eb08-4642-bb75-e0da0a4d0679"
            }
          ]
        },
        {
          "id": "a7b7d9c0-c298-4724-9759-ef1c6965f134",
          "name": "deleteObjectLikes",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;object-id&#125;/likes",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "This reference describes the /likes edge that is common to multiple Graph API nodes. The structure and operations are the same for each node, except that for the following nodes, /likes returns only the profile for the current user if read with a user access token:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43465017-7467-474e-bcc6-b15bf7ba4933"
            }
          ]
        }
      ]
    },
    {
      "name": "Achievement",
      "item": [
        {
          "id": "86ac7183-b693-408c-9538-c1f3d693f1db",
          "name": "getAchievementType",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;achievement-type-id&#125;?application=application&context=context&created_time=created_time&data=data&description=description&height=height&id=id&image=image&is_scraped=is_scraped&points=points&title=title&type=type&updated_time=updated_time&url=url&width=width",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A games achievement type created by a Facebook App. Not to be confused with an instance of an achievement."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84a684d6-8421-4a12-8ad7-2388d1cf848b"
            }
          ]
        }
      ]
    }
  ]
}