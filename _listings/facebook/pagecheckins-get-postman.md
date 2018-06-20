{
  "info": {
    "name": "Facebook Get Page Checkins",
    "_postman_id": "5e0e006f-223b-49a1-ab0d-9ad7e5fa3a30",
    "description": "Checkins made to this Place Page by the current user, and friends of the current user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "47544dd0-b175-49eb-97a8-4c243ae898fb",
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
              "id": "90395188-7dfa-4d0a-996a-384368f32029"
            }
          ]
        }
      ]
    },
    {
      "name": "Album",
      "item": [
        {
          "id": "9ecb9ecb-559b-42c6-b107-8bcda31df9a2",
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
              "id": "1c67fa5b-f153-4289-8505-1aa6d46a2b9e"
            }
          ]
        },
        {
          "id": "bb18cb88-e055-46ac-90d6-ef7e17387222",
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
              "id": "6ef5b45a-f1c0-4bc1-aad6-064329776bef"
            }
          ]
        },
        {
          "id": "78140b09-2f78-45af-951f-ee0d9ba9661f",
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
              "id": "224a8e24-d6e7-45d7-ad6e-59a8b0c77e8b"
            }
          ]
        },
        {
          "id": "471c16bd-6974-4425-a152-79f9c0817cc4",
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
              "id": "c1492703-18df-4473-a6f9-ae50775ca9ee"
            }
          ]
        },
        {
          "id": "337ee10b-4694-4458-abcd-82d746f6e8ed",
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
              "id": "bb73a4c4-2a8a-4277-b218-52763a934547"
            }
          ]
        },
        {
          "id": "9712194d-33d1-4b9a-990e-c16c33244b5e",
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
              "id": "8f65e339-8e65-4668-a7c1-21881269eaa8"
            }
          ]
        },
        {
          "id": "e1fd23dc-8983-46f7-a34c-15bf90dbe189",
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
              "id": "c2878610-4c86-46ed-bdcc-249e8641ecf8"
            }
          ]
        },
        {
          "id": "8f386e35-bf8b-49e5-b23a-d0a6394fb30b",
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
              "id": "3825c28c-47f1-42eb-be72-eb689031f4bb"
            }
          ]
        },
        {
          "id": "f3fd6388-cc8b-4f13-920d-c47748837c8e",
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
              "id": "53a8c067-734e-47a8-8d9e-5fea3257e4e3"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "336fb961-79f7-421b-a2a1-0888931db52b",
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
              "id": "cc0a20b0-8869-4713-b148-fa4e8792f0af"
            }
          ]
        },
        {
          "id": "67d5b81b-f363-4691-a367-b2dbe02339b8",
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
              "id": "51b4cfae-c493-4199-9109-3274dd024255"
            }
          ]
        },
        {
          "id": "017aaf69-42f0-4908-aaf0-68612b85d473",
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
              "id": "95a5c0e9-0f61-4aea-81b8-7b4a356e511f"
            }
          ]
        },
        {
          "id": "3061621e-3378-4bfe-b28b-9e4d91b4fef1",
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
              "id": "4ca3ccb8-e56a-4416-a376-8ad40c064c0e"
            }
          ]
        },
        {
          "id": "07ab0510-4844-4b2c-a304-43c23bd88f16",
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
              "id": "fc95c3ac-42f9-40b9-8d6e-a127dd6f526e"
            }
          ]
        },
        {
          "id": "4789cb52-2a81-4943-9d51-5697253fa415",
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
              "id": "6c9785c3-8c38-413a-b19a-496547b39d98"
            }
          ]
        },
        {
          "id": "8f55cbba-2443-440e-87c6-d028971236ea",
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
              "id": "21deeb63-4b68-4a0c-9352-085ed7af4e55"
            }
          ]
        },
        {
          "id": "0204d933-9df1-4600-b896-2dc0ee511f28",
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
              "id": "314124ce-1f2d-4be5-b79e-4bbb068d9487"
            }
          ]
        },
        {
          "id": "a444c312-c701-446d-aa3b-45f6e8a56e86",
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
              "id": "34520c6f-1618-4261-ab50-668c6278a003"
            }
          ]
        },
        {
          "id": "c4461f2a-74f1-4d1f-b121-bdc9b1be912e",
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
              "id": "ee56e080-e709-4042-9f3e-e4316a2557da"
            }
          ]
        },
        {
          "id": "acb4a4ac-88ee-4e97-b270-07c5455914b7",
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
              "id": "57e6217e-b5c2-4bb9-b57f-1d921575ee12"
            }
          ]
        },
        {
          "id": "d2b47872-38e5-4e1c-92af-31f641f10b86",
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
              "id": "ee187342-803d-41bf-bac0-3329119b737b"
            }
          ]
        },
        {
          "id": "a9b48a83-b335-4df6-9f54-c04e9db45005",
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
              "id": "29782e72-0c0d-4ead-a357-41bbee586076"
            }
          ]
        },
        {
          "id": "6a52f6d5-595f-4627-bc89-b7b7296b03ff",
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
              "id": "8fd4c432-feb6-4021-8357-c7b8e6dd24af"
            }
          ]
        },
        {
          "id": "c40e6dba-f723-42f4-8c25-7e361b798e79",
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
              "id": "76578f11-820f-4318-bf9e-0f91ace93704"
            }
          ]
        },
        {
          "id": "41d1cdbb-a7bd-4e38-be93-78ef748ff551",
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
              "id": "5f16be5f-e136-489a-ad2f-2bab847b4663"
            }
          ]
        },
        {
          "id": "82055832-e96d-456d-bfe6-1403e79d8eb1",
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
              "id": "b7328b43-ea28-41f6-9d13-aa62a2a7e24f"
            }
          ]
        },
        {
          "id": "e76f4849-179e-4d0c-a91c-f682c1fa073c",
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
              "id": "fb65120d-0c1c-4039-8a53-5419dd9c6478"
            }
          ]
        },
        {
          "id": "b9d1f7d8-f63b-45c6-8ad6-cc2d49c53201",
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
              "id": "21a2e34e-86f2-4d24-9991-96901efc33ab"
            }
          ]
        },
        {
          "id": "ba72ff0a-610f-491a-b36d-cc74f45a0359",
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
              "id": "0b955ff9-cf1b-4b11-958f-61180b0d8ab0"
            }
          ]
        },
        {
          "id": "dda6cef8-3109-4e67-9aa5-05e389d8651d",
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
              "id": "68f6d096-28cc-4772-9c08-bb065fe2915c"
            }
          ]
        },
        {
          "id": "ea0f2add-38d4-4cd1-9c20-86f9a7b211e2",
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
              "id": "31f63225-4da8-4c2c-8d21-ec39f8e5c44d"
            }
          ]
        },
        {
          "id": "cdb21701-0ecf-471b-bd8e-b62e522ee458",
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
              "id": "2f24fbdf-1e6f-4b10-a782-b269614c6a27"
            }
          ]
        },
        {
          "id": "f4498b64-eb61-4349-9402-a596fafee17d",
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
              "id": "da63df49-f23f-4641-aae3-605606237e33"
            }
          ]
        },
        {
          "id": "8f9d7e13-6ba8-46e1-a190-bcc890def12e",
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
              "id": "ed596ff3-263e-4fe8-a1fe-0ca78a209e93"
            }
          ]
        },
        {
          "id": "c1ca97de-495b-4024-b6e4-74767c3d4939",
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
              "id": "5cc2f204-aec5-44ea-94c9-6db2180cb45b"
            }
          ]
        }
      ]
    },
    {
      "name": "Checkin",
      "item": [
        {
          "id": "d4293431-7f62-45fd-8957-2f1630e61723",
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
              "id": "8c4774a5-fa08-4df8-978c-bb8be67e4a5a"
            }
          ]
        },
        {
          "id": "cf20e33d-7a2e-4901-9ff0-a32712c181c9",
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
              "id": "a900e663-138d-4fa9-b299-685241951e9b"
            }
          ]
        },
        {
          "id": "ee3866cf-632f-4194-aac9-fc7ac7989767",
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
              "id": "ca36e071-8c4c-45ac-b20c-9196a3b7a512"
            }
          ]
        },
        {
          "id": "58351844-0628-4d2e-b56c-ddb1653db10f",
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
              "id": "319d80a2-4571-4d72-a3d6-7aea6ab85538"
            }
          ]
        },
        {
          "id": "43f0b45e-b254-426b-bd7b-3d4a6df2a4c1",
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
              "id": "44a1a93e-759e-45b9-8e05-091d45e12c1c"
            }
          ]
        },
        {
          "id": "d925230c-992b-4a9a-8385-e7e69409a5ef",
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
              "id": "20d6654c-8234-4ae0-bc69-70c357f11bc1"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "906bc8a3-a9c4-4d26-9b37-67a208693f71",
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
              "id": "06219641-0f01-44f0-abae-dadc5ddda8df"
            }
          ]
        },
        {
          "id": "00d939e9-e81f-4da0-8212-90d00a1ec623",
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
              "id": "ce6485b7-7dfa-4eeb-853a-fc4c3c95d56c"
            }
          ]
        },
        {
          "id": "590b9b44-cf1c-4f9c-b72a-f4db4933cddf",
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
              "id": "a0304e18-d9df-4f25-8fbb-6f275cf50dcf"
            }
          ]
        },
        {
          "id": "4eeff427-ad71-4b80-b535-2c214ddaf810",
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
              "id": "cd000916-ddb8-4a90-b5c5-70f395469dbe"
            }
          ]
        },
        {
          "id": "8d3162e1-4659-4778-b555-492b74f702da",
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
              "id": "a7bce0ad-55c4-411d-968c-bf678be8b4f0"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "0fb04933-3772-445d-8914-9f372aa65ec3",
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
              "id": "6747a520-d167-4d5c-b455-ff2e19d98a07"
            }
          ]
        },
        {
          "id": "3a00bf10-0470-4b52-bd23-7f2d35e7d8a2",
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
              "id": "2944d8dc-55c5-4948-b7df-c2fa353ed361"
            }
          ]
        },
        {
          "id": "032d5f6c-2186-4fab-8990-5da59a26f10c",
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
              "id": "4dc01d04-6d3b-414b-aef4-6d231f2c047a"
            }
          ]
        },
        {
          "id": "5dce5785-d5ea-4746-a211-e7530d8ea353",
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
              "id": "c3b33d0b-fbd7-4d6e-be8e-73b6fb9e1485"
            }
          ]
        },
        {
          "id": "acdd333c-c290-4ff1-b2c9-5856fe671d22",
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
              "id": "39e52ba5-a269-4752-bc9b-aa72d05373dd"
            }
          ]
        },
        {
          "id": "db460670-7ad5-4fa3-958b-c1154c3d94d4",
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
              "id": "82784be1-f7f6-44af-9e90-26e70acc5f42"
            }
          ]
        },
        {
          "id": "a88b0084-3225-46e4-9622-1848d4bec911",
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
              "id": "b67c5835-cd95-44b5-adbf-d6d9fb131ebe"
            }
          ]
        },
        {
          "id": "b6bbc512-d69f-4d57-9274-54565e601a4d",
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
              "id": "61aa8d65-07a5-42ef-b0b2-0c3bd6060eef"
            }
          ]
        },
        {
          "id": "139fb63f-67aa-4a5e-8563-fa8efda2db30",
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
              "id": "e7105e0f-d9cf-4291-b6c5-51f34459fa82"
            }
          ]
        },
        {
          "id": "95e96d49-dcf9-407a-bb57-dd8add8a6f3d",
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
              "id": "25470b92-6555-4143-a95d-61ef4a74bee1"
            }
          ]
        },
        {
          "id": "ac4b3fc2-4d3d-41ea-92ec-5bd9c0ba6338",
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
              "id": "52b371ed-95dc-4c5e-a6c9-4b953cf4a392"
            }
          ]
        },
        {
          "id": "004494c4-1c71-42eb-905d-3e5ef811cd7c",
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
              "id": "a985dba9-9740-4e88-bb3c-3792a9e2c7e2"
            }
          ]
        }
      ]
    },
    {
      "name": "Friendlist",
      "item": [
        {
          "id": "b1c5f46a-787a-4d41-a8ba-65e274025343",
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
              "id": "f2bf0591-9457-4034-85a6-83ae02189376"
            }
          ]
        },
        {
          "id": "3af3a39f-9b3f-44b3-8107-180de5c1e9d4",
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
              "id": "0666eeaf-97f6-4652-9a2a-11bd9e1e5d71"
            }
          ]
        },
        {
          "id": "eb48122a-f80f-4ac0-9f4a-2b2e52b63de3",
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
              "id": "875181fe-580e-4c65-b3ca-481840f8665a"
            }
          ]
        },
        {
          "id": "6791e9cc-e3c2-461a-93e1-cd3fff1c4dea",
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
              "id": "cf0a47b7-dd17-454b-a701-268cd031213a"
            }
          ]
        },
        {
          "id": "75bce361-d9a4-4e31-b19a-2ceed96f8596",
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
              "id": "d022b8e3-992b-468c-85a3-3edae7041326"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "11490c39-ebf8-492b-86d6-3a546cac5e7e",
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
              "id": "91d9c902-e794-486b-9c16-20194afaba59"
            }
          ]
        },
        {
          "id": "741de549-8714-4012-a58c-3e11f1d1efbe",
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
              "id": "43fbd102-eb34-4bcb-aa05-c6fc41fce61b"
            }
          ]
        },
        {
          "id": "0e4feff8-20a1-4e0a-b81d-e7e95be84b6b",
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
              "id": "f02208a9-da56-4c93-8ee6-69de20b035f7"
            }
          ]
        },
        {
          "id": "137235f9-27c3-48d0-931d-e3837485394c",
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
              "id": "e84d2204-5158-4d0d-91a3-d460464b3b1b"
            }
          ]
        },
        {
          "id": "49961795-97e7-4dba-a479-7e2961ebe412",
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
              "id": "fd3968af-94bf-4f43-b8f7-81b00ba54002"
            }
          ]
        },
        {
          "id": "d7364bec-4708-4647-aa98-92c0349bc727",
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
              "id": "03b4742c-d0b3-425e-a086-0e422be861d9"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "7b0fb507-afa2-419e-bcfb-2db116b84b49",
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
              "id": "95d6060e-e6bd-4479-985c-3c173232d119"
            }
          ]
        },
        {
          "id": "90d55564-2d27-40cf-b5d4-8f34fb575827",
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
              "id": "d1aa8f8d-6af3-4966-a254-493b9f6b6a9d"
            }
          ]
        },
        {
          "id": "275c5733-ceea-43f1-9e5a-64341293bd0c",
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
              "id": "47e17e01-177d-4657-889d-c41a08a9aa5b"
            }
          ]
        },
        {
          "id": "2422b05b-0af0-475c-9386-134e1f0f4a4d",
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
              "id": "ffad2391-52f5-4dfb-ae9d-e8ede449e609"
            }
          ]
        },
        {
          "id": "3fdc9ebf-cf4e-460b-adeb-1667b7a9ebf2",
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
              "id": "4a3a0e6b-3b41-4a02-acaa-e7fd9df5062f"
            }
          ]
        },
        {
          "id": "1f0c2b81-cd71-491f-b974-79fbcfe4e5c9",
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
              "id": "de3d0823-1356-4fb9-882b-a29ac6c0d7b9"
            }
          ]
        }
      ]
    },
    {
      "name": "Note",
      "item": [
        {
          "id": "aba4bd15-f122-4da1-a186-9245b3a288f2",
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
              "id": "9d1364de-093c-4a50-abd8-0152f3ad446f"
            }
          ]
        },
        {
          "id": "3488bf1e-e1fe-4437-a252-acccdbbd8c14",
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
              "id": "8b3e97bb-c9a8-42ae-94c9-9d2937fd1b76"
            }
          ]
        },
        {
          "id": "cd67b333-0705-438e-95d2-918b4e55999f",
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
              "id": "b38cc253-985f-4ed0-935d-34fbf1e63fee"
            }
          ]
        },
        {
          "id": "6a85e72b-6453-4882-845e-feff8050af8d",
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
              "id": "c903e512-ed0c-48c0-b065-542dc1e4ada9"
            }
          ]
        },
        {
          "id": "0b980431-7a0a-4a57-b097-05f1c7cc9ee8",
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
              "id": "92523dcb-d28e-4f11-bf90-f8806fb40f87"
            }
          ]
        },
        {
          "id": "2ab3b0b9-9848-419c-a85b-5c75488c04e8",
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
              "id": "5ada7ac7-d38e-457a-af13-81e51f103109"
            }
          ]
        }
      ]
    },
    {
      "name": "Page",
      "item": [
        {
          "id": "80069568-09ba-4e5a-9cee-3aae90222acf",
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
              "id": "370c3c1d-6ffe-44a4-825a-5c319371e3c7"
            }
          ]
        },
        {
          "id": "493ecb95-2ca3-4efe-8700-0b647539a571",
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
              "id": "90439134-d155-4969-ab72-b1a5e7269a89"
            }
          ]
        },
        {
          "id": "74ca8d34-66a5-4262-9908-e5d7a835267f",
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
              "id": "884c01a5-f8db-42ae-97b4-9a2086d86518"
            }
          ]
        },
        {
          "id": "2fec19d5-352a-4008-809e-304e71e7ef61",
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
              "id": "22f53322-89ff-4137-9eab-50bcdfed7d16"
            }
          ]
        },
        {
          "id": "2bc4bc6f-bd2b-4c79-9dbc-72f6b6736fc4",
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
              "id": "6bcfaa6b-64b1-4ec2-b784-627093076481"
            }
          ]
        },
        {
          "id": "8c53774a-83f7-47c8-afd9-72f839d194c1",
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
              "id": "0aade081-3b8c-4d4b-9bbd-4a810060cd96"
            }
          ]
        },
        {
          "id": "342a8fa5-73a4-433f-adbf-c180c2c652e4",
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
              "id": "4a86d65f-f108-4819-8a6c-585bfc5ca556"
            }
          ]
        },
        {
          "id": "5601f3b3-9551-4a4e-8b2c-e727b5112960",
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
              "id": "990725ba-4590-4077-989a-94a607dc9762"
            }
          ]
        },
        {
          "id": "800ddb9e-4827-487d-b6ec-6a3574a3ae12",
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
              "id": "be0bb94d-1887-4ae0-8be8-efb089a0cda7"
            }
          ]
        },
        {
          "id": "0eb60c28-3035-4bd3-91cf-71bae3ba277f",
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
              "id": "d213785d-13f9-4414-a928-0dc4c45aa0f2"
            }
          ]
        },
        {
          "id": "050c1a2c-05a9-4a43-a9f5-0b2b861c95ac",
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
              "id": "d1c74eee-c018-4bc6-bcc9-d72cac8c282c"
            }
          ]
        },
        {
          "id": "0244235f-3d76-4f89-841e-87f3b71bf285",
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
              "id": "3c707aae-8f54-4174-b338-58c06c8305d7"
            }
          ]
        },
        {
          "id": "b3775910-b25e-408f-8fd3-d470f13e0557",
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
              "id": "c2f7acb7-e16b-40a2-930b-172fc6881f2f"
            }
          ]
        },
        {
          "id": "3c8b318e-5935-4c15-aab7-d69b5e230799",
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
              "id": "2b7acc57-9e82-4f6e-b023-a3ffed71508a"
            }
          ]
        },
        {
          "id": "bdbfe054-5117-4786-bfc9-f13ad8a06f3b",
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
              "id": "180f4a20-f922-4127-992e-a1c2354e54e7"
            }
          ]
        },
        {
          "id": "f3b6bba6-0412-4be4-accb-ec19cdda11f5",
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
              "id": "4aad53d1-15ba-480a-9ea9-030f39906cc2"
            }
          ]
        },
        {
          "id": "0db0f6db-6e6a-4ab8-b7d2-2d488ac3b9b4",
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
              "id": "141b7bef-e80a-4c4d-ad98-4bf5a9077c2f"
            }
          ]
        },
        {
          "id": "72ffa90f-8859-4635-97fa-7fa630ef71b7",
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
              "id": "c6181cc1-83aa-4aec-979b-87a4b99c18c4"
            }
          ]
        },
        {
          "id": "b4d74cbb-59d4-4148-937a-71b5c4cd1247",
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
              "id": "20b6bf51-c578-4628-a1d7-d08a5bb272b9"
            }
          ]
        },
        {
          "id": "c0cbb90b-ba64-4d6a-9034-9e4e65f6e376",
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
              "id": "85a5af74-5d4c-402a-b21d-31ac4ad5d3da"
            }
          ]
        },
        {
          "id": "a764a1ab-8c3a-472c-9528-3d3626fbf3a7",
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
              "id": "2139c33a-4e25-4076-a913-43a3481e72b7"
            }
          ]
        },
        {
          "id": "efea008a-44dc-469e-8c43-320092d3272e",
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
              "id": "fcdd82ef-a9c7-4814-a14c-120b8f426cba"
            }
          ]
        },
        {
          "id": "8425cdb6-ba77-495b-a7c5-332424618ed6",
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
              "id": "775b00bc-7d38-4ae9-91a5-c6793209b673"
            }
          ]
        }
      ]
    }
  ]
}