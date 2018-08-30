{
  "info": {
    "name": "Facebook Get Object Sharedadds",
    "_postman_id": "575164f0-61f8-404f-9d31-b4a71af7d681",
    "description": "The /sharedposts edge that is common to multiple Graph API nodes. The structure and operations are the same for each node.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Object",
      "item": [
        {
          "id": "e867661e-54b7-4659-84e8-020750eae85c",
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
              "id": "89fe25ed-b349-484d-b048-6c6bef94ee50"
            }
          ]
        },
        {
          "id": "da66d65d-b191-4fe9-9f9f-3477a578341d",
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
              "id": "6594f587-cdd3-4513-aa43-d65c9418fbe8"
            }
          ]
        },
        {
          "id": "522ad61f-83dd-4c39-9b69-044d2cb80bf4",
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
              "id": "d376f749-6655-4003-9ea8-ca2095a0d2e8"
            }
          ]
        },
        {
          "id": "1e44a0dd-f719-486b-b65e-4d5d1040870f",
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
              "id": "41e09a6d-0e66-481e-8155-f65ca7ca5c0b"
            }
          ]
        },
        {
          "id": "996a9cac-dc85-4d47-8c85-7d311961a282",
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
              "id": "76eb8015-edf4-466e-8ff7-7cbec791d106"
            }
          ]
        },
        {
          "id": "406841a4-92f1-464e-993a-b05962514e4d",
          "name": "getObjectSharedadds",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;object-id&#125;/sharedposts",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The /sharedposts edge that is common to multiple Graph API nodes. The structure and operations are the same for each node."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07a75e26-d7c3-4020-8be7-ae8e0933ee91"
            }
          ]
        }
      ]
    },
    {
      "name": "Achievement",
      "item": [
        {
          "id": "3b20d73c-36f8-4839-b789-e12c40f83dbe",
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
              "id": "a3b0da57-8f93-4a87-86ac-968b38acd85e"
            }
          ]
        }
      ]
    },
    {
      "name": "Album",
      "item": [
        {
          "id": "b58af89b-f926-404c-9178-2ccc66279263",
          "name": "getAlbum",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;album-id&#125;?can_upload=can_upload&count=count&cover_photo=cover_photo&created_time=created_time&description=description&event=event&from=from&id=id&link=link&location=location&name=name&place=place&privacy=privacy&type=type&updated_time=updated_time",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents a photo album. The /&#123;album-id&#125; node returns a single album."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c24aaf2-52b5-42f4-a3ff-25a01c4b4ad9"
            }
          ]
        },
        {
          "id": "64433a82-7c1c-4589-8d19-042fbd49e819",
          "name": "getAlbumPicture",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;album-id&#125;/picture",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The cover photo of a photo album."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3620bbc-de2a-4030-8ac2-e3f8c10ce1c8"
            }
          ]
        },
        {
          "id": "64722bba-c901-4c21-8b9e-8509389a947b",
          "name": "getAlbumPhotos",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;album-id&#125;/photos",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The photos in an album on Facebook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83c76339-3a72-466c-a5e8-a3fd7f84a8c7"
            }
          ]
        }
      ]
    }
  ]
}