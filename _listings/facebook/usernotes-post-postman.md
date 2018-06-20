{
  "info": {
    "name": "Facebook Post User Notes",
    "_postman_id": "66d7ac4a-6816-4ebb-b17b-056d86971024",
    "description": "Creates a note on behalf of the user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "333ae510-f590-4d26-b5e0-1bb11e41f6ab",
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
              "id": "2c138db6-ab4c-42d7-a143-de276f5c8f43"
            }
          ]
        }
      ]
    },
    {
      "name": "Album",
      "item": [
        {
          "id": "aa16a211-f2a0-44e4-a1b3-d3d12241fb2c",
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
              "id": "7c3f4961-ea5d-44de-bf44-2e5e914e859c"
            }
          ]
        },
        {
          "id": "3f4ebcbc-006f-42c9-a3d6-543b286041b6",
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
              "id": "352d0fee-5b31-43c8-aa0c-b7bbd0594d5e"
            }
          ]
        },
        {
          "id": "cdba640e-d67d-4e4a-8379-2f584fea0e7a",
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
              "id": "e5efd4a0-f72d-4166-a05d-958a779579eb"
            }
          ]
        },
        {
          "id": "a9859f6b-2327-48ff-8df9-1a23e6da54e0",
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
              "id": "43b8b5bd-11d8-4488-ac0e-27fa022805e9"
            }
          ]
        },
        {
          "id": "08915e0d-af6a-4278-81b3-818c1332bd46",
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
              "id": "4597be20-81e8-43fb-a1aa-5a89b53899e2"
            }
          ]
        },
        {
          "id": "216e5449-09d7-4703-b54c-7f621948be52",
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
              "id": "7e96a6fb-5504-4f2e-a8ce-f7a1a682c6c7"
            }
          ]
        },
        {
          "id": "cebaa365-233c-4abe-b7bd-e22405e969f7",
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
              "id": "1e030e26-f896-4709-988e-21228ee27c37"
            }
          ]
        },
        {
          "id": "44fe9f46-3131-4d42-93ba-1272f273bcf2",
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
              "id": "881bde0b-49c1-4ed9-9427-af5aca46ebd7"
            }
          ]
        },
        {
          "id": "c2c66813-2ba1-485f-86d3-caa1246a6c55",
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
              "id": "48dee17d-fff9-4669-b4e9-44106ccc2605"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "10866541-d2af-449e-8c4b-09409f1908ff",
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
              "id": "bc3ae91c-7a67-4a13-9f44-f0e3a490bc5d"
            }
          ]
        },
        {
          "id": "02056e79-d74f-40de-880c-a4e26e71d41f",
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
              "id": "49a81154-c711-4997-b6a9-95aa8ffa75d6"
            }
          ]
        },
        {
          "id": "f1bc9f2e-3fd8-4a26-84c6-ac29fb63045e",
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
              "id": "5fc42b51-9a6d-4630-9fd5-a6da26d41fcf"
            }
          ]
        },
        {
          "id": "f160ddc3-230e-4b7e-9ad4-754e17f94526",
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
              "id": "f9432e4a-e890-40d0-ba41-55be53ac8fe4"
            }
          ]
        },
        {
          "id": "04e90240-e2ae-460d-b101-8c357b0ea125",
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
              "id": "8dfdf6c1-a0a9-4c2c-b0ce-c05b4661286d"
            }
          ]
        },
        {
          "id": "76d8494e-efd1-402d-abe6-fb8e3ccf960e",
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
              "id": "1c92337f-dee2-4334-8ecf-2a7a80ed8e9b"
            }
          ]
        },
        {
          "id": "6480a103-b493-4faf-a284-e74b5b1f6e4f",
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
              "id": "5a49b41b-7414-4a9b-9e46-5c289297fdfe"
            }
          ]
        },
        {
          "id": "1217b01b-fb87-43c7-be02-0589a94647b4",
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
              "id": "8e8e85ff-2544-4c06-a913-ba46729abf8a"
            }
          ]
        },
        {
          "id": "13f891ba-cf3c-472a-9d58-91ee87409dd5",
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
              "id": "2fb9bd7b-4fe3-49f2-804a-4c62ba4dcf5f"
            }
          ]
        },
        {
          "id": "263f4dc2-e889-4787-b749-8f51cbde2e2c",
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
              "id": "5bfbc8c8-7cdc-4731-9d05-3d7e4d9bcff2"
            }
          ]
        },
        {
          "id": "58170750-97aa-4c08-b1c3-0a0e28a7ad72",
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
              "id": "a1352d49-c8c7-4508-b9a4-fcfd553e07e0"
            }
          ]
        },
        {
          "id": "cf24935d-f709-4fb6-ba5a-ff6bc4789ffe",
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
              "id": "a8d2726e-e67a-4003-ae16-14dbe64c4540"
            }
          ]
        },
        {
          "id": "18488f2b-8832-4a5b-b72b-2f2f687d12a6",
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
              "id": "4f73cf9e-5b5b-4276-b79a-fc824b4b3b52"
            }
          ]
        },
        {
          "id": "fb434536-d0e5-40fd-8293-14078abed471",
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
              "id": "d55b2e55-4f63-4f40-81a1-efb63f9e9a55"
            }
          ]
        },
        {
          "id": "91837003-5e80-4766-b002-c3d42d5a1a7d",
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
              "id": "5f43027f-9fa6-4eea-a86b-8f6a979c845b"
            }
          ]
        },
        {
          "id": "33671eac-52cb-4d5b-9484-bab688ab2f21",
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
              "id": "1cf94b79-5e56-4a07-af24-b219924426df"
            }
          ]
        },
        {
          "id": "6e457502-2d15-450e-87a3-7dd07d5b7afc",
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
              "id": "9c9d6eaf-4158-4548-afc7-837472c55320"
            }
          ]
        },
        {
          "id": "852925af-81c8-461a-8d0f-811319a99c2d",
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
              "id": "8588d40e-a613-443b-8061-624303fb6aef"
            }
          ]
        },
        {
          "id": "2a91aa10-c24a-409a-80e6-efc6f3228af0",
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
              "id": "f3c580e7-a80a-4c71-bc2c-1862aedb48ac"
            }
          ]
        },
        {
          "id": "465c1941-2ed9-4e14-a07d-891667285d53",
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
              "id": "4d3fa100-85ef-4d28-8dbf-e5da69054cfb"
            }
          ]
        },
        {
          "id": "f12a68c8-a9ec-464b-b7d5-dbc738a77faa",
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
              "id": "b974342e-87ee-4d6f-a9bc-dfc87423e7c7"
            }
          ]
        },
        {
          "id": "adb7455f-3b37-4b7e-a580-a9d4c17c951e",
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
              "id": "3c1231ca-a1cc-4379-bce4-170c6b623606"
            }
          ]
        },
        {
          "id": "5be06e4b-ec64-4a90-a2d6-09689f6ee084",
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
              "id": "78e8523a-d346-4265-8e15-39c909ac6d0a"
            }
          ]
        },
        {
          "id": "d50f929c-f444-470f-bcb7-d194addb3e22",
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
              "id": "aeb30f54-acd4-435f-a2da-2725de9c716b"
            }
          ]
        },
        {
          "id": "d5088e6f-581d-4a10-ac63-8b3b2de4eb36",
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
              "id": "7f207edf-aaf3-40d0-803d-b7f28252f393"
            }
          ]
        },
        {
          "id": "7ad7c2cf-323f-4314-bb9c-057d95e437ee",
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
              "id": "a4c36583-95aa-443a-889e-77904a126066"
            }
          ]
        }
      ]
    },
    {
      "name": "Checkin",
      "item": [
        {
          "id": "66a0975a-1a68-434b-bcd0-68b6c188834f",
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
              "id": "ce1defcf-8d33-4c4c-bf92-dbea5f6bb696"
            }
          ]
        },
        {
          "id": "5349d377-3358-446a-bbe6-a6748ba3964f",
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
              "id": "a5b349a2-d313-4b95-8a01-938b91ebdf37"
            }
          ]
        },
        {
          "id": "a1f55e02-5b42-433e-8879-ea904d580f2e",
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
              "id": "c1d368e4-dfe0-4b27-813d-7f6caf8980da"
            }
          ]
        },
        {
          "id": "2e427055-3ef1-4fb4-b7f4-ca75ab36c5bf",
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
              "id": "b869d380-8dcf-482b-9967-36243e6178b4"
            }
          ]
        },
        {
          "id": "1762535c-2e43-4982-9268-fa1c751f26d4",
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
              "id": "efee47da-5936-40ad-b90f-1ea3fb2aa058"
            }
          ]
        },
        {
          "id": "f9d4a227-d095-4b74-8c78-b6277e447dd3",
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
              "id": "bf4dff79-6a4f-4bc4-9a2f-2f6f2dcbee11"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "65c3222b-6989-4f19-a9f2-9d4feeaf7087",
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
              "id": "9328bf34-0c1d-46f6-9555-b69c6cfc88d5"
            }
          ]
        },
        {
          "id": "2fc9456c-4eae-488f-b342-d837521cf563",
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
              "id": "3dbe7354-7021-456b-a7ef-628210b6eaf1"
            }
          ]
        },
        {
          "id": "7c322457-a1ef-4133-9498-9e29c2da7a51",
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
              "id": "d312432b-c60d-46c4-b97a-ab7ee5a13cec"
            }
          ]
        },
        {
          "id": "59a9a367-4df0-4dc0-a41b-74b1408859e8",
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
              "id": "3a0b36cf-6c55-490d-a282-6a37c5c88705"
            }
          ]
        },
        {
          "id": "e31ad684-e72a-40b9-aa64-36afb48a3dba",
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
              "id": "150e05bd-e7b2-43c2-bdb4-b963f97af4c0"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "18fb7833-236b-496f-b433-4e2906f99ec8",
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
              "id": "fe75a5ad-0be7-407c-be3d-6059d02d3254"
            }
          ]
        },
        {
          "id": "81d36f76-9036-4479-b21b-66c7c32c6103",
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
              "id": "065d16e9-847c-4c54-bee4-1e6db0912acb"
            }
          ]
        },
        {
          "id": "3916a4aa-7700-4b5a-969f-0c7f36349345",
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
              "id": "5368683a-20cc-4653-954f-4daf881068b7"
            }
          ]
        },
        {
          "id": "9dbd2cfa-dfef-4d18-a53e-7438b1572886",
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
              "id": "ffcbcfcf-0609-41f9-917d-493c2180695e"
            }
          ]
        },
        {
          "id": "a64f45dc-6fd5-485e-9322-0efa37f30950",
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
              "id": "a8455367-4dc7-421d-98fa-194cb0fb64f9"
            }
          ]
        },
        {
          "id": "2d3eb837-f143-4342-b131-c59e7b6badce",
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
              "id": "67e3709b-60eb-42ab-95cf-d027487b558a"
            }
          ]
        },
        {
          "id": "f36b65be-5314-4861-9e7c-0368755b869d",
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
              "id": "b2399512-7101-44c0-b73d-a1f089e295c8"
            }
          ]
        },
        {
          "id": "00363bdd-7f79-43d5-89de-5f52ad418544",
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
              "id": "262f9359-fecd-4c59-a685-c77c84ffed5e"
            }
          ]
        },
        {
          "id": "7d3af03d-a838-4f55-9f96-9d49b6ed1488",
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
              "id": "cb7a2517-69b8-4ca6-b166-495ab9978c83"
            }
          ]
        },
        {
          "id": "8f1a5d6d-d041-4632-bb26-561f30a19198",
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
              "id": "0d1a404a-526f-4131-b179-9f97a9c46215"
            }
          ]
        },
        {
          "id": "5b435e09-0b66-4898-824e-ca603e88be10",
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
              "id": "2d96f26d-0c6e-44be-8520-b552aca9076e"
            }
          ]
        },
        {
          "id": "41717d04-4b06-4f9b-9379-794ce0a1f5a3",
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
              "id": "607a0c2f-93cb-4cf7-be95-30f4a86aea9d"
            }
          ]
        }
      ]
    },
    {
      "name": "Friendlist",
      "item": [
        {
          "id": "e9d575f5-baf1-4764-9f63-47020f6cdda7",
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
              "id": "61aed9d9-eb02-46d7-9428-ba38f2757938"
            }
          ]
        },
        {
          "id": "4f44685a-1cf8-49cd-befa-85487c9a71b6",
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
              "id": "859a63f4-7e90-47ea-942d-939dd6b60011"
            }
          ]
        },
        {
          "id": "0c4183d2-34cd-4af1-9899-cf657cfc0600",
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
              "id": "bb7bf2c5-9466-4180-8428-1f3e40d4d618"
            }
          ]
        },
        {
          "id": "01de542a-e8b9-4bae-af93-e6837b92f91c",
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
              "id": "ca1272d7-f785-4bb8-957e-bf273cbe8e6f"
            }
          ]
        },
        {
          "id": "a4384329-c384-4104-8127-5618f297ce90",
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
              "id": "dfa25b41-3df7-4c67-a630-a1c7f8a86e09"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "ddacd2d3-569b-4e8d-ae3f-a16830b5e070",
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
              "id": "a724f792-b5c1-4ae6-9cbe-ab7df28583fa"
            }
          ]
        },
        {
          "id": "71362535-5748-4944-afe4-ef589ccc0591",
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
              "id": "c068297a-29e8-42dc-a9c2-d91e60e82ca9"
            }
          ]
        },
        {
          "id": "8b5538dd-4f38-4ba2-855d-6f1de787ba69",
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
              "id": "27a43dc8-2b41-45c0-90f6-90e7e487048a"
            }
          ]
        },
        {
          "id": "c1c7f928-b334-4b4f-8ad8-c54ad8888d70",
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
              "id": "c7af06db-89b6-4fe3-b6e0-2a677f0091b9"
            }
          ]
        },
        {
          "id": "202833e6-bcea-4239-98c7-bc63262bf601",
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
              "id": "03496959-99c7-44e4-ace1-243757900293"
            }
          ]
        },
        {
          "id": "74295c23-da45-4e3e-9cfc-eb995b5d1344",
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
              "id": "3941c388-6ad5-4a26-869a-e1fad864aba3"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "050e28ac-4d2c-44bb-a07d-bf608ea3ebca",
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
              "id": "2ce55841-6dae-4235-b32f-add70108e07d"
            }
          ]
        },
        {
          "id": "68e8f3b9-c2e6-485a-a864-010d2a06f455",
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
              "id": "f0ec666c-2afa-4d77-a18c-b943dc3b3193"
            }
          ]
        },
        {
          "id": "2ff29f28-7cc5-495d-8cad-ba8b64fcc0a3",
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
              "id": "7caeb5e9-d5d6-48b3-82da-7713897e434e"
            }
          ]
        },
        {
          "id": "b5a5b8c5-2484-46f2-b88d-26be49bc391c",
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
              "id": "08c83710-d15f-45d7-8b2b-53d3e611eaf2"
            }
          ]
        },
        {
          "id": "a1b45146-b9d7-49ef-9019-704699c314c8",
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
              "id": "572f260c-8a84-4f3d-ad72-ae507b75bf1a"
            }
          ]
        },
        {
          "id": "ad1ac486-3137-417b-b008-939fddb4a7e9",
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
              "id": "63502ec1-b0cd-44b4-94df-59bc916a9714"
            }
          ]
        }
      ]
    },
    {
      "name": "Note",
      "item": [
        {
          "id": "b8343a34-3e7c-4522-bac0-d95c913cdbc1",
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
              "id": "db367301-537e-441a-9d48-810bb297f9b9"
            }
          ]
        },
        {
          "id": "ea4b0bca-5a78-4b6c-ad9c-35b2abcc56f5",
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
              "id": "b2a61af0-caf9-4f09-8e76-215bb832867a"
            }
          ]
        },
        {
          "id": "e36cf06b-05bc-402e-96ef-d5bfc96183e5",
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
              "id": "6c03e89c-8cfc-4150-91d4-041cc7a694d5"
            }
          ]
        },
        {
          "id": "edc761e3-1d71-4bfa-93a1-377a167d65d6",
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
              "id": "34f6b870-3bce-422f-a2bd-cdfb2860baae"
            }
          ]
        },
        {
          "id": "a5266b7a-38ee-4cbb-a49c-d56fd8c6f2f5",
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
              "id": "c7b86fc0-f4ac-4150-ba3b-8aab35aa15fe"
            }
          ]
        },
        {
          "id": "5eae2b77-2452-44cd-83e8-b97b1b73694f",
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
              "id": "99729810-7fc8-46b0-84da-d2e3c6212da0"
            }
          ]
        }
      ]
    },
    {
      "name": "Page",
      "item": [
        {
          "id": "92c2f7e7-d648-42f6-a261-e7ca1ac87a2f",
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
              "id": "f122a537-36c3-4b72-a138-ce7f2684269b"
            }
          ]
        },
        {
          "id": "9fa04bf9-08f2-43ac-ab3f-c1d3dfcc40d1",
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
              "id": "b1c1fb9e-daa8-4676-bd42-791898535802"
            }
          ]
        },
        {
          "id": "9d907ffb-bf2e-4c5a-8578-665cdee74c9c",
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
              "id": "01766645-86e4-405b-b46c-7986028df4f3"
            }
          ]
        },
        {
          "id": "1f44b291-02cf-40a2-acac-6738d2f4b5c1",
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
              "id": "1d0fa70a-0216-4271-8d2c-899749d743e2"
            }
          ]
        },
        {
          "id": "e747f830-4bb3-49a3-90df-fb7fee401c4d",
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
              "id": "f8121a07-392e-42d9-b79b-ca5dbdc0fce8"
            }
          ]
        },
        {
          "id": "f083b5ce-133f-448e-b416-669928b74cfa",
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
              "id": "c53b2dcc-9b78-41b2-9e0f-95f2bfdf7486"
            }
          ]
        },
        {
          "id": "ed216fde-c3cd-44c5-b935-ef6ff29e7961",
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
              "id": "522d9fbd-9a0c-4eb2-9560-c191c0d5a977"
            }
          ]
        },
        {
          "id": "d1349461-7e45-4ccc-9075-29996d62ddab",
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
              "id": "ff4af40c-e0e3-4184-95b6-c5788e269151"
            }
          ]
        },
        {
          "id": "0ed70520-0675-4aa1-b26a-83ea45e29eaf",
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
              "id": "ab892dca-a1ab-4e5b-9dc8-5e7bbd7922c4"
            }
          ]
        },
        {
          "id": "ccca1deb-22a4-4ef0-869f-69b4b5e93ea7",
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
              "id": "be739f88-fab5-41e7-b13a-2213db02f3da"
            }
          ]
        },
        {
          "id": "34c79440-eed8-4114-871a-c24aaedb1c43",
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
              "id": "7ea1cf15-eb5d-49f5-b95d-159f0fa8e8d8"
            }
          ]
        },
        {
          "id": "066c5800-4e58-46cd-8d86-37ba9757c453",
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
              "id": "69bbc9df-46c2-4ebd-8358-86718163bb80"
            }
          ]
        },
        {
          "id": "e9977fbe-e7a1-43b6-ad39-3645019799a4",
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
              "id": "42d8f4fa-d113-4586-a2f6-55e1a0b8ab98"
            }
          ]
        },
        {
          "id": "f8b9b764-07e3-4a9a-b21b-5412ced5da6e",
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
              "id": "07021700-59fe-45bb-86ea-d6756379ffff"
            }
          ]
        },
        {
          "id": "43e3b1d3-b1c8-46c1-8b04-63bdca85e256",
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
              "id": "c905d5e4-abdc-4721-8c07-94d00c8ddfd0"
            }
          ]
        },
        {
          "id": "f4087264-0dec-4e97-bcce-c962982d6265",
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
              "id": "a55a7301-6e0a-4079-8de8-693ef26ed82b"
            }
          ]
        },
        {
          "id": "e6c2cb8c-837a-4dc8-bb87-c384f7c1887a",
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
              "id": "4e79986b-5781-4029-b7e7-97b17ad15b7c"
            }
          ]
        },
        {
          "id": "fc3f216d-10ff-47c1-8b08-d699397db957",
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
              "id": "6170c5dc-74d3-4af2-85e2-41cd297e6fd5"
            }
          ]
        },
        {
          "id": "46b42762-9a2a-4b63-a748-0996bbd0b77a",
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
              "id": "14360180-4559-4f44-bb75-2b2c6d568157"
            }
          ]
        },
        {
          "id": "2b89f26d-7d67-4560-acb5-59481cc8daf7",
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
              "id": "8202d247-09ef-4939-851a-b118f8ef7748"
            }
          ]
        },
        {
          "id": "a3effe0e-b62e-451b-88ea-2cf6d6e2a694",
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
              "id": "acdc02a3-2e85-4e05-93d4-9c578255918d"
            }
          ]
        },
        {
          "id": "ad6d0e61-5e9f-48dc-b8c1-96f5e87da1c7",
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
              "id": "8797476f-ec80-46d2-aa63-f86c7282dc58"
            }
          ]
        },
        {
          "id": "06ebb7aa-1c27-432a-a7dc-9ef848f67046",
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
              "id": "a0a0e3c8-5469-40e8-bbb9-8b5b7e1da58a"
            }
          ]
        },
        {
          "id": "5e58430e-968b-44e3-9321-942644c513b8",
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
              "id": "fe0abda3-87ec-4221-bbd8-529ad3f8a997"
            }
          ]
        },
        {
          "id": "aaa4735e-9419-4b1b-a6bc-a9a8943ec11c",
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
              "id": "95193477-cb90-4c42-a3ee-dc4fccaab633"
            }
          ]
        },
        {
          "id": "f21facea-41b6-46a2-82b7-e58e3911d7d4",
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
              "id": "1cba0e6d-5ab7-4c8f-90d2-b76e23970673"
            }
          ]
        },
        {
          "id": "79be3457-78b7-4afd-aa17-2d9abf60dad1",
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
              "id": "cf163c13-3965-4627-a630-3b6d20c0b190"
            }
          ]
        },
        {
          "id": "4685881b-b3ee-493f-aad2-0f9f99e8d2d1",
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
              "id": "e657234a-506a-4dd4-9dc2-415f4664b9c2"
            }
          ]
        },
        {
          "id": "328b31ed-fe40-4a93-bbfe-9ad88ca06cb9",
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
              "id": "f4ff050f-c397-4c0c-affc-e0b657087ef6"
            }
          ]
        },
        {
          "id": "774b9b79-1037-41d7-9d27-d8ef0d5c84f6",
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
              "id": "ee35b2db-6bc6-4ee1-9212-f5a43de0a714"
            }
          ]
        },
        {
          "id": "e942cf7f-39d1-4174-8562-5fe3e6b513c8",
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
              "id": "04cdc2e5-8f08-4717-ace0-a83e22332375"
            }
          ]
        },
        {
          "id": "64ff0565-80c7-4d01-9928-25f242641f1c",
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
              "id": "98c58ee8-e5ce-400f-9d61-3caefed656b0"
            }
          ]
        }
      ]
    },
    {
      "name": "Photo",
      "item": [
        {
          "id": "64edd3fb-ee76-4411-bc43-82400f6bc4a7",
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
              "id": "fab1cd97-c6a6-44d2-b261-dc60cfe1c957"
            }
          ]
        },
        {
          "id": "ccade8ff-80e7-4154-9531-93ce160f0f13",
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
              "id": "086f2ef5-b24e-4638-bfa4-3c9ca5a80b39"
            }
          ]
        },
        {
          "id": "cb2c1f4b-313c-40b2-844e-6f40a249a514",
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
              "id": "954a2561-5b47-46e0-b96a-1f0f6ffa4ab9"
            }
          ]
        },
        {
          "id": "53207855-1a6b-41db-86bb-751844ab337d",
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
              "id": "5f13265a-b937-4d24-9039-119729c84b64"
            }
          ]
        },
        {
          "id": "17657913-d664-440c-85ef-d70ac363513e",
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
              "id": "d6541e61-ed4f-4456-8736-5e51773be862"
            }
          ]
        },
        {
          "id": "e9e627d7-b35a-4cdb-91a0-6637a5ade73c",
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
              "id": "f2a3cd5b-b010-40e9-9292-60de1cd34ece"
            }
          ]
        },
        {
          "id": "4a1c4d7d-e66e-4d52-ae79-5fd207e8fd1d",
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
              "id": "9a5ba624-8634-48b8-ab1e-db226e9c88b8"
            }
          ]
        },
        {
          "id": "bc66fd00-8b4f-4356-97bc-21f0278abad9",
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
              "id": "6c2b7205-16e0-478f-af5a-7f3f1c2472d6"
            }
          ]
        },
        {
          "id": "0f54e0c8-8676-4883-b73a-6ffb6d26f75e",
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
              "id": "8069512b-8eef-4942-9746-caa719702865"
            }
          ]
        },
        {
          "id": "3fcce7c1-ce98-4e77-a620-5d82085881d2",
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
              "id": "1b05e47e-44b0-49c9-bb31-892c31c664b3"
            }
          ]
        }
      ]
    },
    {
      "name": "Post",
      "item": [
        {
          "id": "908e579b-ce55-490a-ac04-c9a2b82d4dbd",
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
              "id": "7de2d621-4e41-428c-a674-722e839fc831"
            }
          ]
        },
        {
          "id": "22588c8f-f013-43b7-9642-0f19be3aaf2e",
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
              "id": "302967bf-7f31-409c-ae94-ff3c5b21450c"
            }
          ]
        },
        {
          "id": "44da8906-48e1-4a3a-8a57-ca5253cafc5e",
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
              "id": "4fe91c9e-6660-4e5b-a59a-b09d64f2943a"
            }
          ]
        },
        {
          "id": "eae58a54-7ab3-4ae9-920b-9ee54e39eee2",
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
              "id": "ba09a929-2762-4c67-919a-83b6845ced24"
            }
          ]
        },
        {
          "id": "54ac6692-6c4b-40c2-8917-1aedc39210cb",
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
              "id": "96f8c847-3244-4a06-999f-7267a3aebbb2"
            }
          ]
        },
        {
          "id": "5bd7afa0-a3d5-445c-a6f4-0e0582720f93",
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
              "id": "b08a56fd-0f43-48bb-9920-79a445b9bafe"
            }
          ]
        }
      ]
    },
    {
      "name": "Status",
      "item": [
        {
          "id": "594dec4a-29ef-4929-af98-4e4ac87fc3bc",
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
              "id": "468cd613-ec6a-4492-b547-9e4ff0853693"
            }
          ]
        },
        {
          "id": "d8764ccb-eceb-4540-b01d-fbd826658a1d",
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
              "id": "940741ac-e689-4361-b786-55cb6acdf879"
            }
          ]
        },
        {
          "id": "578f625b-b145-44cc-85ef-cb7f446011c1",
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
              "id": "1aebf0b9-72ca-4e9d-a0db-4ff9bd39d26c"
            }
          ]
        },
        {
          "id": "a927c361-1be7-489f-ad5f-a340fdfd88ac",
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
              "id": "0cd165fa-3e31-44da-b853-831cb031f4b1"
            }
          ]
        },
        {
          "id": "69a82f07-631f-4dc2-97e8-9c5c71ad3278",
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
              "id": "9c612147-51cd-4f5b-b507-2055bc63149c"
            }
          ]
        },
        {
          "id": "1f094389-9f17-49a7-b426-ca2155e73a28",
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
              "id": "1c6ff709-f3e2-41b0-84c3-e63067991f10"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "53666c15-d874-4b97-a663-89a77a23074f",
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
              "id": "10e1ba04-cfd2-4d03-9441-20c710f7aec1"
            }
          ]
        },
        {
          "id": "a2f0819b-6fc4-4575-ab1c-fed10ef3afde",
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
              "id": "24a9e73f-d0e8-460f-9343-7f47d51a9236"
            }
          ]
        },
        {
          "id": "76026106-9b41-4d05-9e9b-4c921d3e02ad",
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
              "id": "4a47a9b0-84ef-4ca0-bbbf-288a291522ae"
            }
          ]
        },
        {
          "id": "f5b15f04-6808-41ab-95b9-00a95d09da82",
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
              "id": "446303fa-3d06-4e50-a58f-b1bad3b42a35"
            }
          ]
        },
        {
          "id": "d5904e6e-c2bf-4092-a86a-358d2f22b588",
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
              "id": "fcbc6b56-405f-4a34-b36b-9797ee8e55f0"
            }
          ]
        },
        {
          "id": "11716232-4957-4051-b0f7-873714e0352d",
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
              "id": "b972a0ee-c5e0-4c2f-b179-966e20a99779"
            }
          ]
        },
        {
          "id": "90f533f4-67b5-4a87-8c63-1e19d7c775dd",
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
              "id": "e97513e8-f034-4e5a-9488-8ed66979ec4c"
            }
          ]
        },
        {
          "id": "3ad0c980-3202-4873-84b5-ed0b13dc7fdc",
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
              "id": "529e2f6f-9f49-49b2-b79d-2555d8d000b1"
            }
          ]
        },
        {
          "id": "1ea4c429-7ad9-4685-9df8-a29fff1f0684",
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
              "id": "f7f83747-ced3-4c4c-ba2b-78d8fb8d1c1a"
            }
          ]
        },
        {
          "id": "7d69e0d0-e23a-449e-b495-5ac306947e17",
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
              "id": "71041d61-28b1-4349-9f0e-726e2878b930"
            }
          ]
        },
        {
          "id": "346b97ed-5935-483c-9855-73ca962cfb59",
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
              "id": "63bebd6a-8f53-43f4-9c14-99e5a86d66c1"
            }
          ]
        },
        {
          "id": "710bb3d9-dd72-4d5b-b2d5-2e197d1507e6",
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
              "id": "6a09cf8f-7234-48c6-b4fb-12a507a1a33d"
            }
          ]
        },
        {
          "id": "b3ad2c91-a694-43f6-972e-b5251944f342",
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
              "id": "623b6ba1-b904-44d9-a167-189828e26fa4"
            }
          ]
        },
        {
          "id": "8c5c6514-0691-4ce8-b161-cf2f2c82842f",
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
              "id": "5ed1359f-573d-4c09-b7b1-356c11d7f8d5"
            }
          ]
        },
        {
          "id": "83a429d2-0fd6-4d6c-8e3c-ec6467cd652c",
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
              "id": "6ea0d938-3684-4865-ba8e-ce6d940a93bb"
            }
          ]
        },
        {
          "id": "4acbbaee-564a-4643-9642-dad3971fe0c3",
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
              "id": "d94fe1a2-0a39-48d9-a6a5-d5f078ff00d4"
            }
          ]
        },
        {
          "id": "f848208d-364c-4149-996a-78d1dc55b4af",
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
              "id": "c585b58c-f3fc-42ec-be10-06f8c685ea7a"
            }
          ]
        },
        {
          "id": "ca4546a5-77b0-4aab-84f0-db706bec8708",
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
              "id": "4e26e316-d669-491b-ac95-b022831bfb91"
            }
          ]
        },
        {
          "id": "01a73378-3748-4570-8bf8-3cd6a5498064",
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
              "id": "5dca4a97-cea9-4a6c-a3a3-b19a7d31b0ad"
            }
          ]
        },
        {
          "id": "ac3cadb9-90b9-4f8a-870a-01d77480f1f4",
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
              "id": "5b712ad1-a733-4654-8ed0-da00eccef5c7"
            }
          ]
        },
        {
          "id": "9b84b730-d7ea-4c94-9a79-cb67783cddd8",
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
              "id": "89640b29-6f22-41f8-8634-da0a44a2f669"
            }
          ]
        },
        {
          "id": "2688fde9-1b5f-47e3-b3e3-d5c65a8482f2",
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
              "id": "3753a7c1-ea94-442f-b01c-15ab5f093e5d"
            }
          ]
        },
        {
          "id": "7c62010f-8894-49ac-90a2-a0b6b634fb28",
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
              "id": "0a6c9893-a1c5-4c63-8bbb-6e7b3456a640"
            }
          ]
        },
        {
          "id": "501b323b-09df-4388-b740-d2bc6ef11691",
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
              "id": "426de5c0-ad9e-4564-a4b4-a80e4b2b3401"
            }
          ]
        },
        {
          "id": "c9b04a3e-7567-438f-be30-79ec30503e4d",
          "name": "getUserLikesPage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/likes/:page"
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
            "description": "Checks if the user likes the given page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51a4d7ef-41ec-447a-b42f-4733b06cf0f7"
            }
          ]
        },
        {
          "id": "7c972e7b-c177-4ccc-b0cc-468a49febd88",
          "name": "getUserLinks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/links"
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
            "description": "The user's posted links."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "477e5469-39bc-47b5-9697-b1d8564acf2f"
            }
          ]
        },
        {
          "id": "d8239b09-9437-42ba-bd33-ece48bc19e77",
          "name": "postUserLinks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/links"
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
            "description": "Posts a link on the user's profile page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "754bdaca-b100-4262-bbca-2339c7cb5080"
            }
          ]
        },
        {
          "id": "ab18a1c2-aeb7-4955-b230-e41fd3f4deb8",
          "name": "getUserMovies",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/movies"
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
            "description": "The movies listed on the user's profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cf0319d-00be-42e9-9771-75ad1bdb2c03"
            }
          ]
        },
        {
          "id": "e6b92c99-f15a-4cec-ac67-a64a5f6a4ae2",
          "name": "getUserMusic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/music"
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
            "description": "The music listed on the user's profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e0f2477-3356-4576-9dff-abccda7dd594"
            }
          ]
        },
        {
          "id": "d1b5af77-2526-45fc-a8d4-2784088ed7ed",
          "name": "getUserNotes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/notes"
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
            "description": "The user's notes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ceecdb9b-1387-45a7-8d5d-bd2a7acd2727"
            }
          ]
        },
        {
          "id": "cf1a0591-b187-4f0d-b412-19eadd2bfe4d",
          "name": "postUserNotes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/notes"
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
            "description": "Creates a note on behalf of the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e9c40b5-4dff-4f1c-ba77-6446292a41ef"
            }
          ]
        }
      ]
    }
  ]
}