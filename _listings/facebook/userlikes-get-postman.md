{
  "info": {
    "name": "Facebook Get User Likes",
    "_postman_id": "1d378987-8436-4aa0-8ce6-63afb497dbc1",
    "description": "All the pages this user has liked.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "5e57a955-ea32-4b55-a0e3-1d2fbc136a47",
          "name": "getSearch",
          "request": {
            "url": "http://graph.facebook.com/search?q=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search over all public objects in the social graph"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "113e06dc-16a0-4f6a-af60-df2c88e2b0c2"
            }
          ]
        }
      ]
    },
    {
      "name": "Album",
      "item": [
        {
          "id": "65b9d641-43bd-47c7-9456-5f8ebbcc8955",
          "name": "getAlbum",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":album"
              ],
              "variable": [
                {
                  "id": "album",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A photo album"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc0ae575-895d-4525-9d8d-171b3a11dd3d"
            }
          ]
        },
        {
          "id": "ec34e867-8728-46e0-af85-ecc90d4774f0",
          "name": "getAlbumPhotos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":album/photos"
              ],
              "variable": [
                {
                  "id": "album",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The photos contained in this album"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de99fe9d-a09d-4571-8727-e77bc40abfa3"
            }
          ]
        },
        {
          "id": "72058e34-5707-4b15-9f14-bbd322105739",
          "name": "postAlbumPhotos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":album/photos"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "album",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a photo to the album"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0791aae-3320-4c1d-81bf-b0d54f5c6ac4"
            }
          ]
        },
        {
          "id": "dba66ebe-d106-4b68-8d1b-9db8f6da1a41",
          "name": "getAlbumLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":album/likes"
              ],
              "variable": [
                {
                  "id": "album",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The likes made on this album"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60a7863a-cc0e-48d7-b26c-a7331845f143"
            }
          ]
        },
        {
          "id": "1d7a6df1-7e29-4887-a60b-9e9ae3d8ed4d",
          "name": "postAlbumLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":album/likes"
              ],
              "variable": [
                {
                  "id": "album",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Likes the album"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "441785de-8bc4-4bab-8c39-f9c093df16f5"
            }
          ]
        },
        {
          "id": "7361b9d8-798c-44eb-8287-c60c7bd3459d",
          "name": "deleteAlbumLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":album/likes"
              ],
              "variable": [
                {
                  "id": "album",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unlikes the album"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "132871a8-87b4-40e1-896d-a1b38b8b7ab1"
            }
          ]
        },
        {
          "id": "035b551e-596b-4284-b356-c5fce8b324f0",
          "name": "getAlbumComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":album/comments"
              ],
              "variable": [
                {
                  "id": "album",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The comments made on this album"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "428674c1-7333-4490-b9b7-990b4125b04b"
            }
          ]
        },
        {
          "id": "659c3bac-2f21-4039-ba57-40f2ffbba09f",
          "name": "postAlbumComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":album/comments"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "album",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a comment on the album"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25a0a4c7-5b43-48f8-a9f5-ccfbf5a0ff27"
            }
          ]
        },
        {
          "id": "5fb6c0e2-f64d-47dc-94b7-89e50a4ab4b7",
          "name": "getAlbumPicture",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":album/picture"
              ],
              "query": [
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "album",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The album's cover photo; the first picture uploaded to an album becomes the cover photo for the album."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f08f7737-0c82-42ce-952c-44ff22e920c1"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "13d1ecf8-c94d-4e3a-869f-d9091bef9779",
          "name": "getApplication",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "An application's profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e073ac0-b6b9-4e07-b704-47c0a40485da"
            }
          ]
        },
        {
          "id": "7d523b06-8d4d-4fff-bd80-cd2ebaea6304",
          "name": "getApplicationAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/accounts"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Test User accounts associated with the application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0e02410-6433-40e4-9d11-29cc09afddda"
            }
          ]
        },
        {
          "id": "eae77a18-1131-4489-b702-874e6497e4d1",
          "name": "postApplicationAccountsTestUsers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/accounts/test-users"
              ],
              "query": [
                {
                  "key": "installed",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "permissions",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a test account for the application"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa3795e1-a756-47c7-93da-6bbe16f0329f"
            }
          ]
        },
        {
          "id": "50adf794-5911-4c52-b36c-2a6c00b6f053",
          "name": "getApplicationAlbums",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/albums"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The photo albums this application has created."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9192658e-2895-4772-a998-705882a923c9"
            }
          ]
        },
        {
          "id": "12ada37c-0e16-4701-99a5-25bae432f168",
          "name": "getApplicationFeed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/feed"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The application's wall."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9889bfb6-7373-435d-a67d-793364833b61"
            }
          ]
        },
        {
          "id": "d4dfd378-b5f7-487a-a409-ae5684d751ce",
          "name": "postApplicationFeed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/feed"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a status message on the application's profile page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df7c4089-2e8e-48de-96be-7f2da25657ff"
            }
          ]
        },
        {
          "id": "d95e0b4b-f1ef-4878-8c9d-b1d34463ea7d",
          "name": "getApplicationInsights",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/insights"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Usage metrics for this application"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84d7dacb-3364-407f-9b93-7fdc41560bd7"
            }
          ]
        },
        {
          "id": "7709e955-36e5-481d-b061-b08aeeb8709a",
          "name": "getApplicationLinks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/links"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The application's posted links."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7acbac43-b33f-4e1f-be80-5a392b807036"
            }
          ]
        },
        {
          "id": "3d988954-5646-4744-830a-61ae4924d22f",
          "name": "postApplicationLinks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/links"
              ],
              "query": [
                {
                  "key": "link",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a link on the application's profile page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47bcd228-9951-4a15-89a5-661aaaf06269"
            }
          ]
        },
        {
          "id": "b9575ba3-4540-4e00-91f9-cd12eac6a0e4",
          "name": "getApplicationPicture",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/picture"
              ],
              "query": [
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The application's logo"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80af751a-cfd9-4db3-ac9f-869201330092"
            }
          ]
        },
        {
          "id": "5c0578cf-1ccb-4d89-9eef-0f7d0c87e3dd",
          "name": "getApplicationAdds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/posts"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The application's own posts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0b0372e-6f6d-4ac7-8105-e2696527ed87"
            }
          ]
        },
        {
          "id": "2db52361-3f5d-4f28-99a5-184ce5f300f4",
          "name": "getApplicationReviews",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/reviews"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Reviews of this application"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a8c3557-6282-4537-82bb-db325f1f43ce"
            }
          ]
        },
        {
          "id": "36443c3a-0e12-4096-a060-592fec93b223",
          "name": "getApplicationStaticresources",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/staticresources"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Usage stats about the canvas application's static resources, such as javascript and CSS, and which ones are being flushed to browsers early."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38724d9d-7f0f-403d-aad5-7370ad1f7797"
            }
          ]
        },
        {
          "id": "7fdcc272-366a-4fb7-919a-db2d0d59f476",
          "name": "getApplicationStatuses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/statuses"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The application's status updates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63524289-ee0a-4227-8710-07f95e72ac88"
            }
          ]
        },
        {
          "id": "94a7e53c-b767-4feb-b01a-6090134f729c",
          "name": "postApplicationStatuses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/statuses"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a status message on the application's profile page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "678a10f5-7181-46cd-bdfc-cb659c5a686c"
            }
          ]
        },
        {
          "id": "4b0f699c-aa09-4d20-a01b-8724ecd55cad",
          "name": "getApplicationSubscriptions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/subscriptions"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All of the subscriptions this application has for real-time notifications."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08e7d8a2-0a74-4cfc-afeb-804599db80c8"
            }
          ]
        },
        {
          "id": "b88ebc08-e086-4af9-977f-c4caaeebbb45",
          "name": "postApplicationSubscriptions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/subscriptions"
              ],
              "query": [
                {
                  "key": "callback_url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "object",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "verify_token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a real-time notification subscription for this application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e7150de-bc5b-4c1d-bfd8-af1d837342a3"
            }
          ]
        },
        {
          "id": "493b03db-2a8f-4b00-898e-b86d427daf68",
          "name": "deleteApplicationSubscriptions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/subscriptions"
              ],
              "query": [
                {
                  "key": "object",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a real-time notification subscription for this application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bb9dba0-2b78-49e0-af82-ac3b7eb98ac1"
            }
          ]
        },
        {
          "id": "bfdc4f0d-c640-4aa6-a266-f108d6ea816b",
          "name": "getApplicationTagged",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/tagged"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The photos, videos, and posts in which this application has been tagged."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0256cfd2-6bc1-496e-9313-41e702fc8a02"
            }
          ]
        },
        {
          "id": "b988e088-4e80-49f2-8dd8-9337e21e79b3",
          "name": "getApplicationTranslations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/translations"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The translated strings for this application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26bb620d-72e5-4894-ab9e-91cb5717c72a"
            }
          ]
        },
        {
          "id": "736652a2-ee31-4533-972e-af269c15cbe5",
          "name": "postApplicationTranslations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/translations"
              ],
              "query": [
                {
                  "key": "native_strings",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Uploads translated strings for this application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7f431ef-9549-4d73-b9b1-b7a07a701fec"
            }
          ]
        },
        {
          "id": "d578472b-006e-4dca-bf1e-eff3c981e1d1",
          "name": "deleteApplicationTranslations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/translations"
              ],
              "query": [
                {
                  "key": "native_hashes",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a translation string for this application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38d122b6-dfe3-4984-9616-9d43f807bf02"
            }
          ]
        },
        {
          "id": "cfc87b0a-fae9-47bd-9097-a84f35545e12",
          "name": "getApplicationScores",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/scores"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Scores for the user and their friends."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e4cf4c3f-0a24-4209-8403-7491f261a10e"
            }
          ]
        },
        {
          "id": "05380d20-8321-4971-892b-7838abcf77ba",
          "name": "deleteApplicationScores",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/scores"
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes all the scores for the application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8abd27ff-428d-443a-ae76-d89a8434f64e"
            }
          ]
        },
        {
          "id": "be8fb9e4-6e57-4a27-a630-9c1be577c8a3",
          "name": "postApplicationAchievements",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/achievements"
              ],
              "query": [
                {
                  "key": "achievement",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "display_order",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Registers an achievement for the application"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b8fe8e0-c336-4fea-93fd-8735f327019c"
            }
          ]
        },
        {
          "id": "21427298-3980-473d-ac68-7f5b8cf6b183",
          "name": "deleteApplicationAchievements",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/achievements"
              ],
              "query": [
                {
                  "key": "achievement",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unregisters an achievement for the application"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24a5dc60-5d36-4cf0-9f51-8e5153e51a98"
            }
          ]
        }
      ]
    },
    {
      "name": "Checkin",
      "item": [
        {
          "id": "cf89903b-452c-4e81-9237-f17fd9c7ac56",
          "name": "getCheckin",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":checkin"
              ],
              "variable": [
                {
                  "id": "checkin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents a single visit by a user to a location"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8414066-f36e-4264-99c5-d9d84922f58e"
            }
          ]
        },
        {
          "id": "0bb42b13-5fc5-48cc-8893-a3f32498a2f5",
          "name": "getCheckinComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":checkin/comments"
              ],
              "variable": [
                {
                  "id": "checkin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All of the comments on this checkin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a304b80-15b9-4a1c-832a-f378032ad482"
            }
          ]
        },
        {
          "id": "7819c446-1490-4611-9989-ca9c5f1bda15",
          "name": "postCheckinComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":checkin/comments"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "checkin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a comment to this checkin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af0bc3ff-9e06-4ce0-a275-a327bae42b2a"
            }
          ]
        },
        {
          "id": "d8adcb5d-6dae-4dfa-a6c3-8764e9b5d311",
          "name": "getCheckinLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":checkin/likes"
              ],
              "variable": [
                {
                  "id": "checkin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Users who like this checkin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a1e40f2-cbb4-4f23-ab74-4f1d19301c2f"
            }
          ]
        },
        {
          "id": "373852fc-b10c-417b-850a-67244cf2058d",
          "name": "postCheckinLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":checkin/likes"
              ],
              "variable": [
                {
                  "id": "checkin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Likes this checkin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "748c82d2-3a45-43c9-9b13-959aff31fb2b"
            }
          ]
        },
        {
          "id": "47403248-e9d3-4073-bbf9-488a61a8926b",
          "name": "deleteCheckinLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":checkin/likes"
              ],
              "variable": [
                {
                  "id": "checkin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unlikes this checkin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aaaf7900-0889-4ef1-8b1a-1cce11529a57"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "80ed0fd1-09bb-4fd0-b3e0-705c08742363",
          "name": "getComment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":comment"
              ],
              "variable": [
                {
                  "id": "comment",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a comment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7dddb5d3-b596-46e2-9834-41ca8c0025b6"
            }
          ]
        },
        {
          "id": "e2c5fb1a-a15e-4230-a093-7446edb27bc2",
          "name": "deleteComment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":comment"
              ],
              "variable": [
                {
                  "id": "comment",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a comment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "699af1f6-b4aa-43e4-999d-d4e1f1b94c3c"
            }
          ]
        },
        {
          "id": "a6fd91ec-b8cc-4487-9bcf-991495712f76",
          "name": "getCommentLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":comment/likes"
              ],
              "variable": [
                {
                  "id": "comment",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All the likes on this comment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8d60bb3-9cdb-486c-b9db-281849ba1b9f"
            }
          ]
        },
        {
          "id": "183e2d46-bbb9-452e-a5d9-40295abf11e2",
          "name": "postCommentLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":comment/likes"
              ],
              "variable": [
                {
                  "id": "comment",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Likes the comment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1647d18a-5d9d-4d90-ad1c-01a19e41991a"
            }
          ]
        },
        {
          "id": "286bc1bc-dac5-4b70-8031-3435069a9220",
          "name": "deleteCommentLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":comment/likes"
              ],
              "variable": [
                {
                  "id": "comment",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unlikes the comment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b12d0bb3-7434-4bd9-8ee8-625a5ff48763"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "419f6eeb-8fe1-4016-9b98-39c442236a59",
          "name": "getEvent",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":event"
              ],
              "variable": [
                {
                  "id": "event",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Specifies information about an event, including the location, event name, and which invitees plan to attend."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba8b6892-8723-4002-b49a-10ac976fcc60"
            }
          ]
        },
        {
          "id": "8d4b0469-870d-449f-bb3c-84c59e04794b",
          "name": "getEventFeed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":event/feed"
              ],
              "variable": [
                {
                  "id": "event",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This event's wall"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52e856f6-f414-4793-a240-d632bd857487"
            }
          ]
        },
        {
          "id": "c710d874-3cbf-4384-8458-5e844b99689f",
          "name": "postEventFeed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":event/feed"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "event",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a status message on this event's wall"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a3d2e6d-f7b3-4aab-9537-dccc0770a956"
            }
          ]
        },
        {
          "id": "5669ad7c-4cc8-4c3d-87e4-42692d8b37f7",
          "name": "getEventNoreply",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":event/noreply"
              ],
              "variable": [
                {
                  "id": "event",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All of the users who have been not yet responded to their invitation to this event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8628b139-901f-4b6b-8df5-4d6cb5a482b7"
            }
          ]
        },
        {
          "id": "24a8ff0a-4b71-4521-add2-22d7666d76f4",
          "name": "getEventMaybe",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":event/maybe"
              ],
              "variable": [
                {
                  "id": "event",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All of the users who have been responded \"Maybe\" to their invitation to this event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50f42e60-d223-4b95-b96b-2e5bf11dbdf0"
            }
          ]
        },
        {
          "id": "eea1bff9-06c2-4764-a18a-03bd1797ab02",
          "name": "postEventMaybe",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":event/maybe"
              ],
              "variable": [
                {
                  "id": "event",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "RSVPs the user as a 'maybe' for the event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b156338-be69-44dd-bc20-8eaa9998c900"
            }
          ]
        },
        {
          "id": "78116a60-bc23-4784-95b9-0be53baf0f17",
          "name": "getEventInvited",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":event/invited"
              ],
              "variable": [
                {
                  "id": "event",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All of the users who have been invited to this event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "860072cf-2e74-4fa0-b24f-0bca75ce967c"
            }
          ]
        },
        {
          "id": "a15d60bd-c3a1-4627-9d33-1324bf94cd73",
          "name": "getEventAttending",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":event/attending"
              ],
              "variable": [
                {
                  "id": "event",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All of the users who are attending this event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4211943-3897-4ee5-b7a9-bc5ab32f592d"
            }
          ]
        },
        {
          "id": "95a441ca-05a3-4acb-9084-0132afc49073",
          "name": "postEventAttending",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":event/attending"
              ],
              "variable": [
                {
                  "id": "event",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "RSVPs the user as 'attending' for the event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65b65755-0ad6-44f7-ab72-dcf67a59d385"
            }
          ]
        },
        {
          "id": "bf8b0790-afc8-435a-a3d9-b27c68ae5bd1",
          "name": "getEventDeclined",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":event/declined"
              ],
              "variable": [
                {
                  "id": "event",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All of the users who declined their invitation to this event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e4c4266e-6b7b-4226-b1e2-c44a3590e83e"
            }
          ]
        },
        {
          "id": "fbffda31-ee03-4d9b-a12f-dac09e4e162c",
          "name": "postEventDeclined",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":event/declined"
              ],
              "variable": [
                {
                  "id": "event",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "RSVPs the user as 'declined' for the event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "596d9080-dcd0-4d41-a700-b1db50f793b7"
            }
          ]
        },
        {
          "id": "506ecb20-0ae1-4031-9e4b-2daef59023ea",
          "name": "getEventPicture",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":event/picture"
              ],
              "query": [
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "event",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The event's profile picture"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b95774d5-e279-4a3f-89a1-d2c34ea3157b"
            }
          ]
        }
      ]
    },
    {
      "name": "Friendlist",
      "item": [
        {
          "id": "0c188f61-2a2e-419e-90f6-178b934ecf84",
          "name": "getFriendlist",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":friendlist"
              ],
              "variable": [
                {
                  "id": "friendlist",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A Facebook friend list. This object represents the list itself and not the members of the list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c9fb20a-f7c2-4814-b3c7-82b3fba8622e"
            }
          ]
        },
        {
          "id": "451729cc-a59c-482a-99a3-500e0d5bd52a",
          "name": "deleteFriendlist",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":friendlist"
              ],
              "variable": [
                {
                  "id": "friendlist",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the FriendList."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02186de7-c04d-4849-8297-89d20d849b9c"
            }
          ]
        },
        {
          "id": "034ea514-c9d8-43da-9696-3ae037f401c4",
          "name": "getFriendlistMembers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":friendlist/members"
              ],
              "variable": [
                {
                  "id": "friendlist",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All of the users who are members of this list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e3e40f6-4f5c-4ca7-99f6-c9cf505eb459"
            }
          ]
        },
        {
          "id": "81cd9772-d6dc-4c4e-bf4d-cea4aab696f8",
          "name": "postFriendlistMembersUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":friendlist/members/:user"
              ],
              "variable": [
                {
                  "id": "friendlist",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a user to the friend list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e101964-ad54-4463-8b6e-1977710c5e6b"
            }
          ]
        },
        {
          "id": "6ca8dc76-3d29-4848-968b-81fbb7dce530",
          "name": "deleteFriendlistMembersUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":friendlist/members/:user"
              ],
              "variable": [
                {
                  "id": "friendlist",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a user from the friend list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67747f89-0a8e-4003-b675-36b5940b9233"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "730d4b1b-3834-410d-8a2b-8696ce07188a",
          "name": "getGroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":group"
              ],
              "variable": [
                {
                  "id": "group",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A Facebook group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c98694f-acd5-4b81-83ed-a57259c0ca84"
            }
          ]
        },
        {
          "id": "11c87355-4c11-4526-beeb-b03eb5fad92c",
          "name": "getGroupFeed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":group/feed"
              ],
              "variable": [
                {
                  "id": "group",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This group's wall"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "135998dc-fd6a-41ab-9bb7-ed85a1a4e6f7"
            }
          ]
        },
        {
          "id": "c8a1aa87-abef-46fb-86b9-82999113d81f",
          "name": "postGroupFeed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":group/feed"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a status message on this group's wall"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9bfa92ab-da78-45cd-a5ab-edcfe265db13"
            }
          ]
        },
        {
          "id": "8ca79cb7-aeb1-41b1-b206-4f473090f349",
          "name": "getGroupMembers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":group/members"
              ],
              "variable": [
                {
                  "id": "group",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All of the users who are members of this group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5fad3050-9419-4a2e-9b93-8ca6bc790b47"
            }
          ]
        },
        {
          "id": "6fd74fb4-4066-44fa-918e-6c8c55b3a4af",
          "name": "getGroupPicture",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":group/picture"
              ],
              "query": [
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The profile picture of this group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb5cc935-29d0-4a88-b648-0961ee769a06"
            }
          ]
        },
        {
          "id": "4d9f5512-0923-4173-9729-10c684f5a161",
          "name": "getGroupDocs",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":group/docs"
              ],
              "variable": [
                {
                  "id": "group",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The docs in this group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ea6553f-5b73-4d42-b5eb-65d8ce1aa82d"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "e45326b3-cab9-4300-a007-e0fd2218a48b",
          "name": "getLink",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":link"
              ],
              "variable": [
                {
                  "id": "link",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A link shared on a user's wall"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68884bdf-6e99-438e-989e-6b688de863c2"
            }
          ]
        },
        {
          "id": "da60eee2-54f0-43e1-b3dc-8b28dd2db112",
          "name": "getLinkComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":link/comments"
              ],
              "variable": [
                {
                  "id": "link",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All of the comments on this link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8458c1a6-9e62-4b74-8514-e7b46c1b2b71"
            }
          ]
        },
        {
          "id": "ea17e7f0-3774-4d4a-bcb7-9f00dd912bd3",
          "name": "postLinkComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":link/comments"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "link",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a comment to this link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63fae17c-760c-4f64-8740-a1ef67382514"
            }
          ]
        },
        {
          "id": "34e2eade-394a-4d25-8d9d-1fde8c6c5df8",
          "name": "getLinkLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":link/likes"
              ],
              "variable": [
                {
                  "id": "link",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Users who like this link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a8de53e-4fae-44ae-83bb-7d8c0856387e"
            }
          ]
        },
        {
          "id": "50aebc96-bf97-4b7f-81a8-d833bf9a1485",
          "name": "postLinkLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":link/likes"
              ],
              "variable": [
                {
                  "id": "link",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Likes this link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45c2df10-baf6-4677-9819-854c5299fe27"
            }
          ]
        },
        {
          "id": "6cb97f9f-43d4-422b-bc1e-7555480d8652",
          "name": "deleteLinkLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":link/likes"
              ],
              "variable": [
                {
                  "id": "link",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unlikes this link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc036fe6-8253-4e62-a9cf-f54f0da9f150"
            }
          ]
        }
      ]
    },
    {
      "name": "Note",
      "item": [
        {
          "id": "c4cfdbb8-6819-4ac7-aa7d-3ac5bf1883e3",
          "name": "getNote",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":note"
              ],
              "variable": [
                {
                  "id": "note",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A Facebook note"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ae98198-bfd9-4d82-bf7c-61055a9e850e"
            }
          ]
        },
        {
          "id": "5926928b-8a84-4be5-a0bb-fb2e6f917891",
          "name": "getNoteComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":note/comments"
              ],
              "variable": [
                {
                  "id": "note",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All of the comments on this note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9bcc224-1566-4115-9219-9051ba5e7d07"
            }
          ]
        },
        {
          "id": "dd9a705e-3d21-4f39-b987-533bd41676cc",
          "name": "postNoteComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":note/comments"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "note",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a comment to this note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8b90a8d-13d1-4400-8881-9fe34530e204"
            }
          ]
        },
        {
          "id": "661bcd82-6d9c-4d2a-9d2b-1662feeeef6f",
          "name": "getNoteLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":note/likes"
              ],
              "variable": [
                {
                  "id": "note",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Users who like this note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e4f5e33-9423-4e4e-bd61-304c9687978e"
            }
          ]
        },
        {
          "id": "42c42437-1dd9-4cca-b810-335595862259",
          "name": "postNoteLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":note/likes"
              ],
              "variable": [
                {
                  "id": "note",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Likes this note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "743f03d5-223d-41aa-b70d-e8cb748a278e"
            }
          ]
        },
        {
          "id": "5427bf34-5209-438b-8e75-22f24df3b428",
          "name": "deleteNoteLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":note/likes"
              ],
              "variable": [
                {
                  "id": "note",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unlikes this note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d618dd2-6b28-4171-b561-24d7cff2bce0"
            }
          ]
        }
      ]
    },
    {
      "name": "Page",
      "item": [
        {
          "id": "1404729c-8feb-4fe7-bc2a-c2e1059d99df",
          "name": "getPage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a Page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5108daad-ec1b-4943-a72d-5441cb0f709c"
            }
          ]
        },
        {
          "id": "229af168-8e2b-4246-9a45-135e535cc559",
          "name": "getPageFeed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/feed"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This page's wall"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47aa9923-d0fc-4514-b7a8-121a16bdf60a"
            }
          ]
        },
        {
          "id": "6c363bc9-961b-4674-b664-0056c463ec38",
          "name": "postPageFeed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/feed"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a status message on this page's wall"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be6f5bdf-ef27-4df2-8a4c-f29bf2c1c18f"
            }
          ]
        },
        {
          "id": "59a0409c-5a01-4a28-be55-eacdf4b70b64",
          "name": "getPagePicture",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/picture"
              ],
              "query": [
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The page's profile picture"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f94ac0f3-f7fe-4b46-8b71-8443a65e690f"
            }
          ]
        },
        {
          "id": "bde1cebb-1c37-43d7-84c6-06909300e1d7",
          "name": "getPageSettings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/settings"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The page's post permission settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ced09bb0-c15b-44da-82c8-5de6f117e180"
            }
          ]
        },
        {
          "id": "3c32513d-79b3-4cb8-9e9f-8d6f0c724e2f",
          "name": "postPageSettings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/settings"
              ],
              "query": [
                {
                  "key": "setting",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "value",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The page's post permission settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9726ceab-c24b-4b71-ad69-7e11ce49ebd1"
            }
          ]
        },
        {
          "id": "6229beb7-6717-48f8-a8f7-190133390f05",
          "name": "getPageTagged",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/tagged"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The photos, videos, and posts in which this page has been tagged"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7a7278a-1491-4fb7-a011-c726f69f9c2d"
            }
          ]
        },
        {
          "id": "17102076-f5a8-4b79-a136-a5ad616d00f4",
          "name": "getPageLinks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/links"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The page's posted links"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebaef870-3328-4545-9ecb-80c6504e2632"
            }
          ]
        },
        {
          "id": "eac70d55-18b2-452c-8e0b-eee7de39947d",
          "name": "postPageLinks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/links"
              ],
              "query": [
                {
                  "key": "link",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a link on the page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d7c92b7-beb3-4f7b-8817-986218de1f1e"
            }
          ]
        },
        {
          "id": "eaa70075-2748-47b8-b7f9-2c3f8a0dbaaa",
          "name": "getPagePhotos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/photos"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The photos contained on this page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "631c3a37-4552-47f7-9923-2cc84ce1bd01"
            }
          ]
        },
        {
          "id": "02703ddd-65fc-4d0e-bdbf-6e5452336cdd",
          "name": "postPagePhotos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/photos"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a photo to the page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3dd2fc8-285d-4091-8769-fc3800c032bd"
            }
          ]
        },
        {
          "id": "6db389ec-cb54-441a-9548-b54db5848b19",
          "name": "getPageGroups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/groups"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The groups this page is a member of"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e8d2493-2ef0-4d3d-b3c5-2bd0d44b395c"
            }
          ]
        },
        {
          "id": "901a5b0d-30d0-48d7-95ed-c456928c2e74",
          "name": "getPageAlbums",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/albums"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The photo albums this Page has uploaded"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3dfeaa4d-c943-4f89-9425-8bf8e11dfa21"
            }
          ]
        },
        {
          "id": "5eb07767-47b5-4e00-8c23-1e55899f962d",
          "name": "getPageStatuses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/statuses"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The page's status updates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e896832-fe36-4824-9512-51765649fe7e"
            }
          ]
        },
        {
          "id": "51c2b468-77d6-4a27-9048-b50b9fa5a90a",
          "name": "postPageStatuses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/statuses"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a status message on the page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6eaf8f4-0085-4e77-8512-957a3700eb76"
            }
          ]
        },
        {
          "id": "bb856d70-f944-4f9b-b17e-074be158921d",
          "name": "getPageVeos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/videos"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The videos contained on this page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "609f782e-249d-4dbf-bc3e-ee178c5ac086"
            }
          ]
        },
        {
          "id": "ca0cea01-1ca2-47bb-933c-b5b77fcb6c27",
          "name": "postPageVeos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/videos"
              ],
              "query": [
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Publishes a video to the page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bffe39ac-a1a2-4ebe-b3aa-803c290d27f8"
            }
          ]
        },
        {
          "id": "791e957e-16f1-4b5c-80fd-26f01a0e0db6",
          "name": "getPageNotes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/notes"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The notes contained on this page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f46d287b-33c5-49df-96de-9dc9895ff489"
            }
          ]
        },
        {
          "id": "f0d1a746-8f3e-49ab-bbfa-71d25e713421",
          "name": "postPageNotes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/notes"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "subject",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a note on the page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "739b0b13-1e98-4604-8a39-122f27e7bcbf"
            }
          ]
        },
        {
          "id": "b6e27c4c-7ca2-412a-829c-1a87aeeaff06",
          "name": "getPageAdds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/posts"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The page's own posts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bdc73d9-1f1f-4662-ae4e-111d3b5e0a1f"
            }
          ]
        },
        {
          "id": "e086e345-a975-4a08-81f0-2a294846a241",
          "name": "getPageEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/events"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The events the Page is attending"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6433007-585d-4a35-8ab8-10a13ff3d635"
            }
          ]
        },
        {
          "id": "68b730e1-20b5-48c8-bf6e-e2e44909b5ca",
          "name": "postPageEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/events"
              ],
              "query": [
                {
                  "key": "end_time",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "location",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "privacy_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_time",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an event for the page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d3464e1-71e5-487c-a9c6-a3dc77564d9c"
            }
          ]
        },
        {
          "id": "ab5821cd-bb02-4f0d-a8ca-d72fc2d5cc17",
          "name": "getPageCheckins",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/checkins"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Checkins made to this Place Page by the current user, and friends of the current user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3dd5c20-85e3-4991-98f6-860a4ad2d76c"
            }
          ]
        },
        {
          "id": "3bf0c387-94a3-4a77-90ef-9da507d6492c",
          "name": "getPageTabs",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/tabs"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The page's profile tabs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "101eafb7-b33e-4af0-81da-f1240e9792c0"
            }
          ]
        },
        {
          "id": "a8a9f45e-fbb2-432e-8056-092ac6dc6aa2",
          "name": "postPageTabs",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/tabs"
              ],
              "query": [
                {
                  "key": "app_id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Installs a profile tab at the end of the current list of installed tabs for the page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19b27af2-37c2-41ea-8e9b-f63d25d33263"
            }
          ]
        },
        {
          "id": "65a0dd44-0dac-4e34-9ab9-bb531cb431cf",
          "name": "postPageTabsTab",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/tabs/:tab"
              ],
              "query": [
                {
                  "key": "custom_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_non_connection_landing_tab",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "tab",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates an installed profile tab for a page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2363ac01-7c5c-41bf-8877-511f6ccfe6ec"
            }
          ]
        },
        {
          "id": "15772812-a983-4c1c-b1f8-459e7141915e",
          "name": "deletePageTabsTab",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/tabs/:tab"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "tab",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an installed profile tab (where is_permanent is not true) for a page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78c426e8-7dbc-4222-9f88-54d8168f0db7"
            }
          ]
        },
        {
          "id": "179d7ceb-471a-4bfe-8b2d-0211ed8042de",
          "name": "getPageAdmins",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/admins"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A list of the Page's admins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ac7d178-02b6-46f0-84ef-bfd499142d5d"
            }
          ]
        },
        {
          "id": "a7a832ee-b8df-470e-a306-4a6b4e6a754f",
          "name": "getPageBlocked",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/blocked"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A list of the users blocked from the page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05d1aec8-8f6a-401a-a34e-b2644071680b"
            }
          ]
        },
        {
          "id": "b6552ae8-554f-4fb7-aece-e3a2fac391f5",
          "name": "postPageBlocked",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/blocked"
              ],
              "query": [
                {
                  "key": "uids",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Blocks a user (or users) from posting content to the page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d05e7430-bdec-4da8-b883-5fa654d319ff"
            }
          ]
        },
        {
          "id": "7b4cb617-0ef3-4ccb-b27b-ea5fc45a7ffd",
          "name": "deletePageBlocked",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/blocked"
              ],
              "query": [
                {
                  "key": "uids",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unblocks a user (or users) for the page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "020d707a-c58f-44f3-80d2-dd9471d2d7bb"
            }
          ]
        },
        {
          "id": "c0362bf3-c965-4068-82a3-a84c5d7d8dc7",
          "name": "getPageBlockedUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":page/blocked/:user"
              ],
              "variable": [
                {
                  "id": "page",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Checks if a user is blocked from the page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e26d6438-3211-4ca7-8ff7-3c1980053a1c"
            }
          ]
        }
      ]
    },
    {
      "name": "Photo",
      "item": [
        {
          "id": "39a71103-1fdf-4d0f-bdfe-8129a73f8e82",
          "name": "getPhoto",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":photo"
              ],
              "variable": [
                {
                  "id": "photo",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "An individual photo"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ede5bd2b-8097-40d0-a45c-7c045fc5912a"
            }
          ]
        },
        {
          "id": "0bd6f2dd-d04a-4f7d-b413-f7bc93982133",
          "name": "getPhotoComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":photo/comments"
              ],
              "variable": [
                {
                  "id": "photo",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All of the comments on this photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c684061-16ef-45a6-bf71-2238164d0e81"
            }
          ]
        },
        {
          "id": "9a7f9810-7f9f-4db1-a40b-d1ecf1c2f750",
          "name": "postPhotoComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":photo/comments"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "photo",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a comment to this photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff2ea306-eefc-4d86-ad96-5d8e4918779a"
            }
          ]
        },
        {
          "id": "d9f9bc73-edfd-44e9-9883-caf060ccba08",
          "name": "getPhotoLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":photo/likes"
              ],
              "variable": [
                {
                  "id": "photo",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Users who like this photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5363121-c064-4dba-b8d5-c37900ec1ea0"
            }
          ]
        },
        {
          "id": "fe615790-c80f-4a2c-8c3c-675d78f5a7be",
          "name": "postPhotoLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":photo/likes"
              ],
              "variable": [
                {
                  "id": "photo",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Likes this photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48b11c02-9884-48fa-a88a-a85a620c6964"
            }
          ]
        },
        {
          "id": "20068098-984a-424e-afb3-5ce6797ec2bc",
          "name": "deletePhotoLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":photo/likes"
              ],
              "variable": [
                {
                  "id": "photo",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unlikes this photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c312e99d-3786-4345-9679-ed423bbdf7d2"
            }
          ]
        },
        {
          "id": "8ce29673-8909-4dbe-9be7-3852869334be",
          "name": "getPhotoPicture",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":photo/picture"
              ],
              "variable": [
                {
                  "id": "photo",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The album-sized view of the photo"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "689a8edb-4ab8-47bc-8b7a-fdc73c75c51b"
            }
          ]
        },
        {
          "id": "7bc7c20d-1452-4b75-9deb-ca5def5ce3f0",
          "name": "getPhotoTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":photo/tags"
              ],
              "variable": [
                {
                  "id": "photo",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Tags for this photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "194f0f73-8451-4b41-a305-bc9d4d396fc6"
            }
          ]
        },
        {
          "id": "6e74d031-1c15-45de-992e-9fdc4ea2cc1c",
          "name": "postPhotoTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":photo/tags"
              ],
              "query": [
                {
                  "key": "to",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "x",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "y",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "photo",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a tag on this photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f88853f8-e723-4c87-903f-818cfbc9ed8a"
            }
          ]
        },
        {
          "id": "f2329278-f5c2-4012-add1-ec9bb8f8b78f",
          "name": "postPhotoTagsUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":photo/tags/:user"
              ],
              "query": [
                {
                  "key": "x",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "y",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "photo",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the position of a tag on this photo for the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ccfc585-cfca-400d-b3ad-26c7d0b706c7"
            }
          ]
        }
      ]
    },
    {
      "name": "Post",
      "item": [
        {
          "id": "df9cadcd-3767-4c3e-a256-92364ae80fc6",
          "name": "getAdd",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":post"
              ],
              "variable": [
                {
                  "id": "post",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A Facebook post"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aad315da-e980-4e54-91e6-b1cbac462a34"
            }
          ]
        },
        {
          "id": "0322aa2a-3c2c-47e2-b2eb-b9ef2920aa15",
          "name": "getAddComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":post/comments"
              ],
              "variable": [
                {
                  "id": "post",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All of the comments on this post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4a45214-e706-4b5d-a79f-0395c3a1163e"
            }
          ]
        },
        {
          "id": "cc0ab467-0327-4caa-ab20-e6fc74250cca",
          "name": "postAddComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":post/comments"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "post",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a comment to this post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e42accc0-9c49-4a4d-af20-63d4875823f1"
            }
          ]
        },
        {
          "id": "91e6d419-829e-4094-9166-5d8ded5e86f8",
          "name": "getAddLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":post/likes"
              ],
              "variable": [
                {
                  "id": "post",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Users who like this post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a4e057c-88ea-4265-a40b-1891ecc6f659"
            }
          ]
        },
        {
          "id": "b145b106-140c-482e-9a0d-70734c0727bb",
          "name": "postAddLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":post/likes"
              ],
              "variable": [
                {
                  "id": "post",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Likes this post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6097b981-d53d-4793-9182-a952b85b8be5"
            }
          ]
        },
        {
          "id": "29980681-c0e2-4aa9-9082-8b81768188c2",
          "name": "deleteAddLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":post/likes"
              ],
              "variable": [
                {
                  "id": "post",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unlikes this post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7515c99a-f462-4885-9b7e-29e17ac2c675"
            }
          ]
        }
      ]
    },
    {
      "name": "Status",
      "item": [
        {
          "id": "21a1eba3-d5eb-4f8c-ad2f-d636fbbb5931",
          "name": "getStatus",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":status"
              ],
              "variable": [
                {
                  "id": "status",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A Facebook status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "877b7c22-a41f-4c31-a0fc-9bb22b4f31bd"
            }
          ]
        },
        {
          "id": "97f2ed9f-ada1-4bd9-99d3-ac70ed70bd8d",
          "name": "getStatusComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":status/comments"
              ],
              "variable": [
                {
                  "id": "status",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All of the comments on this status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce8d4ee0-7a60-4c8d-a0ce-11db956278d1"
            }
          ]
        },
        {
          "id": "4b491191-55f9-4398-8865-f4780a38c73b",
          "name": "postStatusComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":status/comments"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "status",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a comment to this status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ed48e4e-55f9-46e1-bd1f-29013da334c1"
            }
          ]
        },
        {
          "id": "4c65be8f-0ebf-46b1-b7d5-e3d67a1c52d1",
          "name": "getStatusLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":status/likes"
              ],
              "variable": [
                {
                  "id": "status",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Users who like this status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08017b8d-13f3-428b-b7c5-22786d90eefa"
            }
          ]
        },
        {
          "id": "571aa590-67e1-4925-aff8-badeb8565c36",
          "name": "postStatusLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":status/likes"
              ],
              "variable": [
                {
                  "id": "status",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Likes this status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74dac5b0-bac0-445d-96bf-84fd55ba7c88"
            }
          ]
        },
        {
          "id": "e14c6c17-4c4d-456b-bb8f-cdb0aa934187",
          "name": "deleteStatusLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":status/likes"
              ],
              "variable": [
                {
                  "id": "status",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unlikes this status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cabce52c-2cce-484a-9ed5-1a6ec711487f"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "95b0b33e-0fc4-4df9-a0db-37171702f00f",
          "name": "getUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A user profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6a9e683-7568-4232-a139-6c08a93b7d6b"
            }
          ]
        },
        {
          "id": "88be8d8c-908d-4897-a2f8-c4f931d16516",
          "name": "getUserAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/accounts"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Facebook apps and pages owned by the current user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dfde4451-dff2-410b-9ac0-f20d5520d1f9"
            }
          ]
        },
        {
          "id": "b23dff2b-6bee-4879-a3f9-96eb8c16ebd3",
          "name": "postUserAchievements",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/achievements"
              ],
              "query": [
                {
                  "key": "achievement",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts an achievement for the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "302ae432-2ae7-4386-8a9f-f3fc2d474f90"
            }
          ]
        },
        {
          "id": "8776d655-5db8-4d10-8224-d098a775031c",
          "name": "deleteUserAchievements",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/achievements"
              ],
              "query": [
                {
                  "key": "achievement",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an achievement for the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e4fba325-d5f3-46b4-a842-1f57fc07d5d8"
            }
          ]
        },
        {
          "id": "d11b7e68-4da5-4842-9cd1-6a86f8965b34",
          "name": "getUserActivities",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/activities"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The activities listed on the user's profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6608dadf-0b84-46da-8828-742a3f418315"
            }
          ]
        },
        {
          "id": "2cc25ded-a999-41db-af4e-6a0ce429a3ed",
          "name": "getUserAlbums",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/albums"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The photo albums this user has created"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59de2c14-abd5-41e8-8367-9ae0027337b5"
            }
          ]
        },
        {
          "id": "e5120fd7-3b80-4918-a3d9-06a5d30ed3c8",
          "name": "postUserAlbums",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/albums"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "privacy",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an album for the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c282041d-1324-440e-b07b-9866f02337b7"
            }
          ]
        },
        {
          "id": "4cf36713-fa08-4a31-a40a-06e5fa55cbf5",
          "name": "getUserApprequests",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/apprequests"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The user's outstanding requests from an app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d177ca06-513e-4f11-8d03-176aaff1a3af"
            }
          ]
        },
        {
          "id": "f3562440-112f-4eb0-86c6-06ef3925ba85",
          "name": "getUserBooks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/books"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The books listed on the user's profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "129ff17f-6a7b-46b2-bd21-1d0c8b208f28"
            }
          ]
        },
        {
          "id": "4002e664-2a6b-4d97-984b-5191411c45d6",
          "name": "getUserCheckins",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/checkins"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The places that the user has checked-into"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "715ab236-ec19-466d-8d1f-d11e2ec807e7"
            }
          ]
        },
        {
          "id": "1224afd7-1591-42f9-a674-e54e9605c38b",
          "name": "postUserCheckins",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/checkins"
              ],
              "query": [
                {
                  "key": "coordinates",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "link",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "picture",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "place",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Checks the user into a place"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f670f7a0-2972-4eea-9400-d536db41c959"
            }
          ]
        },
        {
          "id": "52493e11-dcad-4c7d-b3cb-d5fc63dfea62",
          "name": "getUserEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/events"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The events this user is attending."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c6083f4-8622-4ede-9c46-ee75faa847a4"
            }
          ]
        },
        {
          "id": "989f3fd8-27e0-4a1f-88dc-dfb9fe9ddfa1",
          "name": "postUserEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/events"
              ],
              "query": [
                {
                  "key": "end_time",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "location",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "privacy_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_time",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an event for the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f5a79f9-870a-4649-8634-438c5a12f0bb"
            }
          ]
        },
        {
          "id": "772b6b72-0841-49d5-8616-a12b4dd865e0",
          "name": "getUserFeed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/feed"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This user's wall"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0932efa3-4ef6-4211-a95f-2f5c452e2baa"
            }
          ]
        },
        {
          "id": "50bde865-8e49-4244-8839-5c3a916ac47a",
          "name": "postUserFeed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/feed"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a status message on this user's wall"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3203aed8-2171-420e-97ca-c7fd59c677ed"
            }
          ]
        },
        {
          "id": "c53e0ad2-0d73-4d71-a209-1d79f1517a95",
          "name": "postUserFriendlists",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/friendlists"
              ],
              "query": [
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a FriendList for the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca1dfb2c-3ffc-4765-b43c-c5dff3ceb8be"
            }
          ]
        },
        {
          "id": "0f810f62-ae7c-49f2-916e-1b4aa02e6c42",
          "name": "getUserFriends",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/friends"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The user's friends"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cba9c25d-ce51-4a5e-88d3-7303821e8c34"
            }
          ]
        },
        {
          "id": "9d6ef86f-6d8b-4bbc-9f6c-af749cccb920",
          "name": "getUserFriendsFriend",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/friends/:friend"
              ],
              "variable": [
                {
                  "id": "friend",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Checks if the given user is a friend of the current user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a90c3ce9-1af1-4ca2-bf1b-c2d888d370bf"
            }
          ]
        },
        {
          "id": "4526105e-00c1-463f-ab67-958197250118",
          "name": "getUserGames",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/games"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Games the user has added to the Arts and Entertainment section of their profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d75ce692-ab49-4dfd-a2d8-b303f9be7b2a"
            }
          ]
        },
        {
          "id": "3a2f4128-4348-4b17-b74d-f5150b4c7ba8",
          "name": "getUserGroups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/groups"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Groups that the user belongs to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac3626d1-d91f-47fe-b3bd-c33d64628fe7"
            }
          ]
        },
        {
          "id": "508aeba6-a5f8-460b-9c38-8639abea204f",
          "name": "getUserHome",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/home"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The user's news feed"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7076613-8d95-4527-b3b8-d25c083628bf"
            }
          ]
        },
        {
          "id": "abb1f97c-3f76-477b-9208-6743639124d9",
          "name": "getUserInbox",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/inbox"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The threads in this user's inbox."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6dcf2844-445f-4036-8576-9b27ec5c0ff2"
            }
          ]
        },
        {
          "id": "d13b0f18-05ca-48bd-b880-5eddb46ec0b4",
          "name": "getUserInterests",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/interests"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The interests listed on the user's profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "349fdd59-9b1f-4f1c-8029-7f0c75db7a3b"
            }
          ]
        },
        {
          "id": "33280b98-9ae0-4775-848c-f5f7cea88e1b",
          "name": "getUserLikes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/likes"
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All the pages this user has liked."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2f106d0-6008-42c3-8a4e-0ef3db932b99"
            }
          ]
        }
      ]
    }
  ]
}