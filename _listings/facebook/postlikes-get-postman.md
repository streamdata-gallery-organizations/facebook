{
  "info": {
    "name": "Facebook Get Add Likes",
    "_postman_id": "ebb88ca6-a5a9-424c-a5b5-1944f03c587c",
    "description": "Users who like this post.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "08988b0d-82d6-4ecc-a83a-201244901754",
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
              "id": "26194f82-d9a6-4c48-818b-f0a77508261e"
            }
          ]
        }
      ]
    },
    {
      "name": "Album",
      "item": [
        {
          "id": "2efebff2-6c68-48c0-b06c-a88b89d3069c",
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
              "id": "518fa91e-c885-4adc-85ff-100934868b31"
            }
          ]
        },
        {
          "id": "0e56dba9-a176-4018-97f4-63b11cd8385a",
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
              "id": "c69a6493-bf0a-44ce-b0d1-b980e1bceff5"
            }
          ]
        },
        {
          "id": "9bf212b0-4c8b-4280-94c8-bea9b4bef771",
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
              "id": "0119c404-e3c3-4043-8091-42612fa41fec"
            }
          ]
        },
        {
          "id": "049da1f5-bcb8-4042-bf91-9e1fc411fd25",
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
              "id": "db738fb4-1bfd-4715-8631-28a679ecd2fb"
            }
          ]
        },
        {
          "id": "adf9d66e-4f32-44aa-8cca-262c1dea8a26",
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
              "id": "1bfb82dd-0f54-4bae-b2e2-dd5adf7bed4d"
            }
          ]
        },
        {
          "id": "b3a0a9a9-88f8-41c1-93bf-8b022c3b79ba",
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
              "id": "5f941a24-a8da-424e-8b54-857080bd84c9"
            }
          ]
        },
        {
          "id": "165fdddf-84d4-4ae4-a243-9429f63e9ef6",
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
              "id": "8e4f3816-e3a9-4d44-9085-51a0af850d20"
            }
          ]
        },
        {
          "id": "6a966e8d-f256-41f3-8bcc-317b15c19582",
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
              "id": "c079ff55-367a-4890-b7fd-f0d155215217"
            }
          ]
        },
        {
          "id": "344a2c38-9595-4710-8512-3700bac222ba",
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
              "id": "9f8742da-b9cb-4b90-81a8-4492fbe83555"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "c329e99a-f7a7-4096-b7e9-7aca86a69c25",
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
              "id": "f8e15831-b8cf-4933-9558-10136db4a921"
            }
          ]
        },
        {
          "id": "361fd3d9-64c7-4b67-86ec-47cb341e549f",
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
              "id": "c647d293-33ac-4746-b1a3-9b9e1a170505"
            }
          ]
        },
        {
          "id": "a7e7ab45-dcf3-4ca2-bb5e-a4cff194ddd2",
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
              "id": "86a133b7-e93e-493b-8560-dcdbd83391e4"
            }
          ]
        },
        {
          "id": "a990794a-bb87-464e-b8a2-4c1a3ad850f9",
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
              "id": "0ffd76cc-f538-402a-8b1d-fc6622d484c1"
            }
          ]
        },
        {
          "id": "f822e33a-f60c-46d3-adaa-09ae8288089c",
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
              "id": "e611b06b-5aab-47d9-ae1b-0dc23dc4b939"
            }
          ]
        },
        {
          "id": "63cc830e-db13-4e78-8c35-d8321cdddadb",
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
              "id": "14b80f40-3605-4f2b-a46c-eefe97a3c3c4"
            }
          ]
        },
        {
          "id": "fe9cbdd4-d12a-4966-b990-7b55260dfd61",
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
              "id": "d93b9ae6-bb7b-42bc-8a59-4f950c1208b9"
            }
          ]
        },
        {
          "id": "1b964968-ed3c-47ff-a74d-a22f0ede56fe",
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
              "id": "32672c0f-41af-47eb-9bf3-27f197c7a8f2"
            }
          ]
        },
        {
          "id": "e86be23e-5799-43c5-bc67-7c1acef36984",
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
              "id": "aca9c74f-de52-4450-9585-f7a927772e4f"
            }
          ]
        },
        {
          "id": "5bdb421a-bcb8-44ef-afa2-7bfe1eb9648c",
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
              "id": "628ba483-aaff-44bd-9c0a-3557eaa161c4"
            }
          ]
        },
        {
          "id": "169c54d3-faa9-449e-ab6e-aa268d7e5ebb",
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
              "id": "4a444254-a91e-45d4-9474-333dff8e68a4"
            }
          ]
        },
        {
          "id": "9b76ec29-2154-40c2-962b-63c9908f99f7",
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
              "id": "f6c28f8e-5452-4a3a-892a-c3e626978105"
            }
          ]
        },
        {
          "id": "5f59122a-e08f-410d-ad63-2125e70ba3b3",
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
              "id": "0dbacbc2-bfcd-4e92-a1ce-20124f17876a"
            }
          ]
        },
        {
          "id": "5f8a57d2-ba35-47d3-bf27-e3fa5a4f56cb",
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
              "id": "57b4868a-271e-4182-aa01-f49435d6204b"
            }
          ]
        },
        {
          "id": "ca8a67e4-d1c6-4e60-94b9-92ba2b64e6e9",
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
              "id": "2b6c1d35-c7f4-49f5-baa8-e4023a4d84f7"
            }
          ]
        },
        {
          "id": "d8399dc3-7d0c-483c-9a7e-a7728bdc1f24",
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
              "id": "7b9b8215-c0e0-49f0-982b-708e452d307a"
            }
          ]
        },
        {
          "id": "cd3d8491-2ae0-4d9d-b53d-4ee8db3f3cb0",
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
              "id": "d5a06f42-b70c-4946-94b9-6574ba79d230"
            }
          ]
        },
        {
          "id": "a9a69de9-00d3-4e61-a696-40d0e997ee78",
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
              "id": "287c8bcd-ac9c-4177-9fb6-51ed854e233b"
            }
          ]
        },
        {
          "id": "3862a38c-5737-456b-9c72-efdb5e8e2182",
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
              "id": "7ebc45b0-c9fb-4771-b002-db162ca7cd1b"
            }
          ]
        },
        {
          "id": "eb670965-a971-42c0-965d-bdec0d58ae73",
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
              "id": "6d3f0c75-b806-479b-ba09-08a5fed71fda"
            }
          ]
        },
        {
          "id": "2dec81bb-8a11-4131-83bd-03709a8b8749",
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
              "id": "1f3531d3-0c02-4774-9ac6-530f6f8650fb"
            }
          ]
        },
        {
          "id": "e4b3c340-77b3-4c90-88b6-5bc28a282609",
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
              "id": "dac240f8-3ed8-454d-adc9-1625206bf8a3"
            }
          ]
        },
        {
          "id": "aecbe4f1-b0bc-4e7f-b298-c98423e86e98",
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
              "id": "bb7980e6-bf30-42c7-80a3-53d77f761058"
            }
          ]
        },
        {
          "id": "936df542-04dd-4a47-acde-ebfc321a3df2",
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
              "id": "21b8505d-d094-45fb-aeaa-db97b3def816"
            }
          ]
        },
        {
          "id": "f60ded7d-6a6f-4a88-a1a2-6f8018276398",
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
              "id": "01ad455f-1758-4cdf-acba-18a52c30b731"
            }
          ]
        },
        {
          "id": "7a51b08f-62f1-4c67-b549-1de7caa438d7",
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
              "id": "35cc4210-713b-497b-ba20-8b46f4e5a8ac"
            }
          ]
        }
      ]
    },
    {
      "name": "Checkin",
      "item": [
        {
          "id": "34a42d29-53bd-44fc-8fcb-00439d9f0ea9",
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
              "id": "5df3bfb0-fd96-4f72-84b7-da9663bb5ac4"
            }
          ]
        },
        {
          "id": "976c5cb8-4792-48ab-8951-ffb5247e3586",
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
              "id": "067c92de-e2ef-401f-8cf9-1f92a18df205"
            }
          ]
        },
        {
          "id": "d41e5648-7af9-4a4b-b049-3bf34ad4eb57",
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
              "id": "272e059a-387a-4b0e-ae2c-1aea13d4567e"
            }
          ]
        },
        {
          "id": "c7c1c7bf-527f-415f-9980-32404e43d089",
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
              "id": "43071872-5e57-45ad-9104-a64f6b28014c"
            }
          ]
        },
        {
          "id": "bd791f1b-0713-48c4-ba63-da8958cb3317",
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
              "id": "ecc9e918-5dd8-4380-8489-af4ad1e52692"
            }
          ]
        },
        {
          "id": "87fb51d6-43c1-4813-80e1-579abdfad8c5",
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
              "id": "f7042086-ba48-4f95-8ef2-c35dfe1bc990"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "444d6c6b-2470-421e-9604-95c881fdce52",
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
              "id": "64475163-0131-41df-9adb-e631179ac5e0"
            }
          ]
        },
        {
          "id": "33a51909-26d2-4171-972c-edc41fd8d82a",
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
              "id": "918146ad-1833-4bc4-ba7c-274654be72d5"
            }
          ]
        },
        {
          "id": "f6bb6152-b218-4da6-8c7e-3203d6890e84",
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
              "id": "9faac8a2-0ad0-434c-b0d3-d9f768b786f1"
            }
          ]
        },
        {
          "id": "1e19f93c-8c87-4673-8663-b81d3ecd8e38",
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
              "id": "e5619dee-1c86-4098-a433-552f33cc1ac6"
            }
          ]
        },
        {
          "id": "e0f4f331-2576-43bc-a4c2-2ddfb7dc5d18",
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
              "id": "c12976c9-e18a-4284-953d-bbf1c28428a1"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "c583a227-280a-4964-8dfa-62fb79dfe318",
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
              "id": "84787f93-989c-458c-a803-597b7576df3c"
            }
          ]
        },
        {
          "id": "14f2c428-6559-488f-82f7-34eefe1607d3",
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
              "id": "b938fa69-70f1-435c-9f88-a73b8a55a2c9"
            }
          ]
        },
        {
          "id": "5155a43c-82c7-48a4-9bab-cbb0620e85ce",
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
              "id": "75b2284c-e19e-427f-a0ce-590622819779"
            }
          ]
        },
        {
          "id": "ddfb54bb-d0de-4ee7-88ae-ba198478c8b4",
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
              "id": "0791c776-4db4-4999-a19a-502d24b68475"
            }
          ]
        },
        {
          "id": "9dcd96cf-f4f3-4e39-9d40-a5582002692d",
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
              "id": "2ebc52da-51d8-4c08-bb12-1bb452cb06cc"
            }
          ]
        },
        {
          "id": "5deac814-6987-449c-b556-5b3a8fc812ba",
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
              "id": "4ceec9df-52b6-49e2-aa4c-5708122303ab"
            }
          ]
        },
        {
          "id": "896c56bd-bdc6-4b34-8b2b-05fe9316027b",
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
              "id": "01f4a175-0b95-4f25-8f1d-144fc4136a61"
            }
          ]
        },
        {
          "id": "ea584a28-9e90-4113-84f0-682dd534e814",
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
              "id": "1dfae591-a69d-461b-a718-5b371501a93e"
            }
          ]
        },
        {
          "id": "007f8268-7fbb-4e67-a9d8-496536121a67",
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
              "id": "65205706-e0bc-480a-a660-181bb482e2fb"
            }
          ]
        },
        {
          "id": "5308b1ca-e19e-48b4-8fa8-619a5ef53a70",
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
              "id": "0adb0e26-de8b-4e78-b257-1e4b6b50a812"
            }
          ]
        },
        {
          "id": "00993258-3f07-4f26-ab77-9c2bc2dc76d2",
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
              "id": "26f64102-8433-4a04-b98b-893248b1d8c0"
            }
          ]
        },
        {
          "id": "e68962fa-d9d6-4098-a1b4-a7a954ff2f32",
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
              "id": "85ed711f-e812-4238-aba7-96a47bbdcb1e"
            }
          ]
        }
      ]
    },
    {
      "name": "Friendlist",
      "item": [
        {
          "id": "654fe21f-15d2-4170-bac0-9dedcad464b3",
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
              "id": "8fc4b336-d551-43cf-8cca-fcb2e905e59d"
            }
          ]
        },
        {
          "id": "146f82c5-f615-44f3-9830-ba5887bd6e1a",
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
              "id": "0e8b3d07-1c92-475e-90d8-6766a5e618f4"
            }
          ]
        },
        {
          "id": "d9f84579-24f3-4277-b73a-31cd0a811e5d",
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
              "id": "92184a7a-0613-4339-a439-5753683d86d8"
            }
          ]
        },
        {
          "id": "4e7b8666-2c4d-4721-a7ac-e3472633fc5a",
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
              "id": "d44eaa4f-947c-44db-9eb1-5d91f528eece"
            }
          ]
        },
        {
          "id": "7d301840-5c67-4228-93ab-d02525add968",
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
              "id": "05733fc9-4c66-43c5-b068-34a63d9030a1"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "85d0e280-7e26-4197-847a-2bd86529b554",
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
              "id": "cdbe5c00-240f-4e27-9c43-b196b12beb0e"
            }
          ]
        },
        {
          "id": "78c19e12-33ac-4af0-a568-87f518b2a114",
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
              "id": "44baf9a7-8159-4484-9252-2ecf12f8fa84"
            }
          ]
        },
        {
          "id": "95117d49-74f3-4238-ba0f-569933a96e84",
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
              "id": "f3eb790d-4a97-4845-bc31-367fbc8b43c6"
            }
          ]
        },
        {
          "id": "f0fbe451-682b-4814-b1f6-cd14ed1acf24",
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
              "id": "7146f427-2330-47e1-b7dd-148f5b33b0da"
            }
          ]
        },
        {
          "id": "fb1c938a-a304-40b9-80fb-cf5ed8d51eac",
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
              "id": "297f078f-8c4d-4db6-8aaf-57f35eee4662"
            }
          ]
        },
        {
          "id": "e73b2e3f-8d3c-43ef-9851-f4ac7d0865f6",
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
              "id": "961aab00-5a8e-4f9d-8c7e-f7d1003b5d0d"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "d6d140a7-e30c-4687-9cee-c1b4c33be767",
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
              "id": "41bd845c-8d4e-47cf-8eb0-e3e042ab4ee7"
            }
          ]
        },
        {
          "id": "0d8eb541-4f0a-43d7-bfd9-bd3c20cb0316",
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
              "id": "d2eee3b6-16d1-488f-b10e-e88203bbd231"
            }
          ]
        },
        {
          "id": "219acf40-8a8f-4eaf-83c2-cea5de541bbf",
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
              "id": "cbe8d3a9-16cd-4f33-9d5e-037ca12f00fa"
            }
          ]
        },
        {
          "id": "ffc4feb4-5746-42ba-8d9e-3b793f0353d4",
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
              "id": "2212deb9-6581-4602-b7ee-d232d017cec6"
            }
          ]
        },
        {
          "id": "651cd270-bec0-47a9-85e6-aa077b5d04dd",
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
              "id": "13a4557e-f0f9-46a1-9def-0231ddc479c1"
            }
          ]
        },
        {
          "id": "415d3c1f-8143-4530-b3d3-9f65219a8fa9",
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
              "id": "dec31d70-123c-4208-8f7c-f08bf3ead4f5"
            }
          ]
        }
      ]
    },
    {
      "name": "Note",
      "item": [
        {
          "id": "86af1e88-6efb-48df-83df-e48a4f5837ff",
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
              "id": "d6ab0b00-bf6b-4a41-b660-cbaa1a9a1872"
            }
          ]
        },
        {
          "id": "ff3838ff-1153-4ff1-9ed9-a56db2cc048d",
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
              "id": "bc071f8c-0e35-4b9d-9162-9c79399e8c88"
            }
          ]
        },
        {
          "id": "e3ba9584-c7e9-484e-8abd-7f4097fc55a6",
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
              "id": "ce9f8fa2-1b85-44bc-8b74-d4f5b1faad68"
            }
          ]
        },
        {
          "id": "efdad50a-ae28-412e-ae62-f411b832e87e",
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
              "id": "9e71de46-cc37-409d-a2ca-71bc88bb04be"
            }
          ]
        },
        {
          "id": "ed3a4a06-6c36-4636-ba8d-6f20e93214bc",
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
              "id": "1b021fcc-fd5c-4da1-b469-202f38f7ca6a"
            }
          ]
        },
        {
          "id": "8e5eb1e3-775e-4561-b473-89069671b36c",
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
              "id": "b650ae48-a439-4cf8-a715-9dd07c1264ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Page",
      "item": [
        {
          "id": "8efac066-e10f-4bd1-a65a-f1b4f7f893a3",
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
              "id": "d0ecda6e-5cb1-442b-928a-455456839578"
            }
          ]
        },
        {
          "id": "18e4506d-5067-40d7-9104-3219851b71e4",
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
              "id": "9d64fd36-2ff2-4a56-b7b7-30c7dbd4cde4"
            }
          ]
        },
        {
          "id": "16f431e9-f09f-4fd5-a54a-71a5ed33efa4",
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
              "id": "b37c4211-80ec-48f2-907d-b9bbcd4a1543"
            }
          ]
        },
        {
          "id": "23288c26-6b9d-4e9d-b6b6-ad0dbe5facda",
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
              "id": "ffd5b703-24da-4595-a93e-c2f443912cd9"
            }
          ]
        },
        {
          "id": "06df5e6f-6286-43b9-a37e-aad2df1c5d5d",
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
              "id": "a0346c85-3abc-4466-ad2f-dc5ba2aa9e34"
            }
          ]
        },
        {
          "id": "9f25c45b-c8b6-4cb3-bcc1-8e47cd01c4c2",
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
              "id": "88bad153-4503-482b-9b2c-521cc67f1762"
            }
          ]
        },
        {
          "id": "94d3f073-ee84-474d-bd1d-49bfee018def",
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
              "id": "c4cf19e5-247f-4a94-8094-a059ef232cb9"
            }
          ]
        },
        {
          "id": "2f0571a5-2269-4e2e-bc06-b9ba7772e8e4",
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
              "id": "1ce0b2d7-02ea-4594-95b1-54ea5acb117e"
            }
          ]
        },
        {
          "id": "7588c6ce-ccf7-4d4e-9fbc-bbeed8244b77",
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
              "id": "fd74c61e-3f8f-46ce-a87d-e328a5636f77"
            }
          ]
        },
        {
          "id": "d1c4665c-0bf5-40ff-a238-4636557c302c",
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
              "id": "86ee82da-5451-4210-8432-1c5481df3c8d"
            }
          ]
        },
        {
          "id": "da806c67-e28d-42c7-a161-f4d900a28648",
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
              "id": "168ae326-ff18-4281-93d8-e0323d13938f"
            }
          ]
        },
        {
          "id": "d0841e31-dea8-4719-82b0-5dca0028e817",
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
              "id": "049416a8-57e7-4de7-9952-5f8eee2e760b"
            }
          ]
        },
        {
          "id": "bbc7b754-e006-40a3-90bc-dc34bca454fb",
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
              "id": "ad52c8d7-e965-4ff4-bc97-a03a18efa66b"
            }
          ]
        },
        {
          "id": "09425996-7b66-41d4-b8df-a3b660ce9270",
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
              "id": "ab24da33-267c-464f-9c64-5c30ade40787"
            }
          ]
        },
        {
          "id": "06719447-f113-458a-8e21-6a0a1625ccda",
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
              "id": "c5ced0d5-3714-407a-8e31-e1fc9dc7e838"
            }
          ]
        },
        {
          "id": "d3533256-5cd3-4aed-81bd-692687126b99",
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
              "id": "c27bc6fe-5b9b-4eac-8346-09e22e196ff9"
            }
          ]
        },
        {
          "id": "cfb6f1d4-06de-4a65-a62c-44e8d17b0caa",
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
              "id": "a16d1632-b058-4057-b16c-de03a0803b89"
            }
          ]
        },
        {
          "id": "7415355e-fab2-4abf-aea1-fbefcca4c95a",
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
              "id": "d22ac7e0-dabd-497e-8fb6-abf3c487fd4a"
            }
          ]
        },
        {
          "id": "7823d9f5-7a66-4b7d-9eaf-e85f4756f815",
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
              "id": "d3a213de-7b9a-4430-a8c6-535df2caaf41"
            }
          ]
        },
        {
          "id": "f7657f43-b3e3-444e-a561-afe17f774b71",
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
              "id": "0c1a1489-46d1-4c04-8dd5-64983430d5c4"
            }
          ]
        },
        {
          "id": "9320a1d4-ff5c-4441-a770-57d53edcd3cd",
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
              "id": "19343088-f173-4854-98c5-ab8883da4b07"
            }
          ]
        },
        {
          "id": "d0b92467-7aed-405e-aa87-2842b8bfc5c3",
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
              "id": "fd48300c-d88d-4d39-9892-bcf08e492e30"
            }
          ]
        },
        {
          "id": "6e82720f-c123-4bba-8857-aa8a8e1757a5",
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
              "id": "37db12d8-2c82-46f5-ba1b-a73799f7e67b"
            }
          ]
        },
        {
          "id": "5d51465d-86c2-4601-8947-9d4f96ba79ad",
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
              "id": "649cdc60-00ab-419c-b3f9-9cad64209972"
            }
          ]
        },
        {
          "id": "faffcce3-9305-455a-a959-b6ac97ef430f",
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
              "id": "932009f7-0d55-4e87-a8d8-ef78ba9ec473"
            }
          ]
        },
        {
          "id": "6630b07c-7fea-464e-ad1b-c0e9c6d3a114",
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
              "id": "024942cf-d630-467d-98ec-8ec1b0d99c2a"
            }
          ]
        },
        {
          "id": "3c3e1f8c-299d-4fc5-addd-7c6d40be361f",
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
              "id": "976ea0fb-77c2-4aed-8412-315964e2a95e"
            }
          ]
        },
        {
          "id": "a328a527-a961-4126-b677-2f9a6d8414e9",
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
              "id": "fdc7ec37-98de-4fcf-908a-4be2864a2b7d"
            }
          ]
        },
        {
          "id": "698691a2-a6f3-4062-9df2-ae49d4d1566d",
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
              "id": "fd37a5cf-eae2-44fd-a9e9-0af80a2abea1"
            }
          ]
        },
        {
          "id": "f14116ba-b2e6-44c3-813f-a847a968fca8",
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
              "id": "1d8bbebe-14e3-4374-ab15-1f7bf5b75dd7"
            }
          ]
        },
        {
          "id": "592a252e-df2e-45f2-9396-c93c7dfea141",
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
              "id": "0ba0140c-b89f-4512-b198-a53a1dc856f5"
            }
          ]
        },
        {
          "id": "36fecc8c-cf24-469c-bd16-a28f3eecb611",
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
              "id": "246fbb6a-5bc2-4ba2-9f6c-f9f882f5e287"
            }
          ]
        }
      ]
    },
    {
      "name": "Photo",
      "item": [
        {
          "id": "fbb88cb6-c6e8-42e1-864c-97bef2bedfb5",
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
              "id": "1e886e59-c4ac-42ff-abb2-e62090ec53f7"
            }
          ]
        },
        {
          "id": "1770c65c-b058-4339-b07d-4ccf95846f39",
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
              "id": "31b486f7-57c6-430d-b021-d4dcacd397e9"
            }
          ]
        },
        {
          "id": "7691fb49-34fc-49ce-8139-3f87509176b4",
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
              "id": "cec31943-bef7-430f-a7b3-498bd5f31ab5"
            }
          ]
        },
        {
          "id": "6eb0cbc0-2780-42d1-9e35-ff1d1969c806",
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
              "id": "93e92155-5470-490a-8599-498d2a0acd52"
            }
          ]
        },
        {
          "id": "fc3d793c-8985-4bb0-a3de-ed1f01af01a3",
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
              "id": "c71f614a-3ed3-4138-9a27-99d9d92200ac"
            }
          ]
        },
        {
          "id": "5fcf1a3e-278b-4fd5-a754-eaa4f4daa4ee",
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
              "id": "d2065d9a-b9d3-4758-95ea-847af3a900ce"
            }
          ]
        },
        {
          "id": "16ff7666-e210-4d83-898b-4a04c2e314e8",
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
              "id": "78e26feb-d582-4639-8f5a-a60e66880b80"
            }
          ]
        },
        {
          "id": "0a70512b-818a-4303-9a2c-16ffbf04f51d",
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
              "id": "5f82f98d-8c28-4b2a-8246-15410254d249"
            }
          ]
        },
        {
          "id": "97f0b1d3-5bc5-47e0-8ce3-dded0431bb95",
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
              "id": "d9cf5b5e-2305-4470-a7c0-2f0a792fd42a"
            }
          ]
        },
        {
          "id": "70cb5ae2-e8d1-41b9-b07e-e64bc1f2755f",
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
              "id": "3d687aa8-854a-4a2b-9283-cf302a117cde"
            }
          ]
        }
      ]
    },
    {
      "name": "Post",
      "item": [
        {
          "id": "20433627-f22c-4c2a-8822-2947eb6fc8ee",
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
              "id": "bca30cb5-860e-45d4-aa54-3a220f42fc47"
            }
          ]
        },
        {
          "id": "31ca936a-daf8-4636-afce-3dc08720d388",
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
              "id": "449398c8-a918-4618-b471-88ddc28c4ce3"
            }
          ]
        },
        {
          "id": "13231654-1c3c-47d1-b51a-af081d627125",
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
              "id": "23c7a76a-9861-4a87-8d5c-90d630c04320"
            }
          ]
        },
        {
          "id": "00caf285-af63-48d8-bf79-526cf312de31",
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
              "id": "ea83360d-536c-42f5-ab87-12d2c7ab0993"
            }
          ]
        }
      ]
    }
  ]
}