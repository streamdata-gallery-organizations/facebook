{
  "info": {
    "name": "Facebook Get User Books",
    "_postman_id": "3b695740-456f-45ff-a272-380afe59ec90",
    "description": "The books listed on the user's profile.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "abc4791f-aae2-460f-9e55-38b6a8bf462a",
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
              "id": "f89e5ef9-2b67-496d-be4e-f814d06bec8c"
            }
          ]
        }
      ]
    },
    {
      "name": "Album",
      "item": [
        {
          "id": "990798fb-9b4e-40f6-980f-3ab624401f6c",
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
              "id": "fcb279fc-44b8-4b8b-8c22-cefcadd71cde"
            }
          ]
        },
        {
          "id": "90a1cab9-7cc5-4899-abda-6df9bdd9de93",
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
              "id": "57709823-3af7-47d3-ace6-ed5992f15834"
            }
          ]
        },
        {
          "id": "7b91d3b9-8783-46da-a70d-4935854dd1a7",
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
              "id": "c7305e50-1199-4ae3-9061-1333e8792cd1"
            }
          ]
        },
        {
          "id": "b94ea71c-e665-4a5d-9a5f-8a0511b9ad67",
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
              "id": "4af9866f-8f6a-4bc2-82ab-4332b32b52df"
            }
          ]
        },
        {
          "id": "ba4b5143-668d-4c94-9012-20cdd5ee9a84",
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
              "id": "0007c1ab-a1a7-40a9-891e-cdbc77777a49"
            }
          ]
        },
        {
          "id": "f5aed3a4-9a39-4c7b-aa36-82ea95d9221e",
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
              "id": "41016109-f860-477d-a9ab-60bfdb15186f"
            }
          ]
        },
        {
          "id": "27316eea-7be2-4ab6-9e2b-8a05e4e88946",
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
              "id": "194bdda0-8355-4102-bafb-d2eddd05fdb5"
            }
          ]
        },
        {
          "id": "20bd1174-12ee-4866-bbe1-879335c2e7b9",
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
              "id": "636870f3-7051-4613-851a-bb99e98d5a25"
            }
          ]
        },
        {
          "id": "7bb4a25a-863f-4edc-a074-a7c6b8079f28",
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
              "id": "fa320858-0520-49f0-9676-4e1474faf836"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "df50121f-0af2-45fc-bece-b87b29833520",
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
              "id": "f60af5de-c23d-437e-8431-2009542e7c99"
            }
          ]
        },
        {
          "id": "20ce5adb-0c11-483c-9911-080a530b8886",
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
              "id": "54ce82a2-b84b-4762-b5e4-318bd134a6f2"
            }
          ]
        },
        {
          "id": "27defebd-7ce4-47d6-9824-2fd2b139aa0a",
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
              "id": "a44caf1d-7881-46a4-82b5-1906d77e29ee"
            }
          ]
        },
        {
          "id": "a2a7196c-2571-4629-b77b-08b61ac446ac",
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
              "id": "8e7d368c-c918-4ced-88bd-7879231a8164"
            }
          ]
        },
        {
          "id": "dab26707-e954-4424-9e03-ad61e83e5e2e",
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
              "id": "7880d32c-2b00-4b0f-ad1c-966fd26fb293"
            }
          ]
        },
        {
          "id": "9bd2806e-0624-4bc6-aa69-edbe09dac090",
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
              "id": "02773263-0c36-4390-84ea-06bc840ec63e"
            }
          ]
        },
        {
          "id": "bae23a66-e345-42e1-abee-98b0515c2ea9",
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
              "id": "d5c726a3-0fb2-416e-afa4-03490e23a1fb"
            }
          ]
        },
        {
          "id": "9e8f22c1-8839-4a6b-8e4c-c94a31df95d3",
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
              "id": "0fa09bbf-9539-4881-9540-57d7b9d3ebe2"
            }
          ]
        },
        {
          "id": "6fc4deef-313a-4f33-acc2-99a5eadce6ee",
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
              "id": "757209c9-8447-44bd-91c1-47a2b13ebab7"
            }
          ]
        },
        {
          "id": "f92f61bd-edf0-4d87-a452-8b6b58972f69",
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
              "id": "c1d690c9-dc69-425d-8898-d404629b4416"
            }
          ]
        },
        {
          "id": "d3ad562e-6548-468e-b1c1-56848e32b7f4",
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
              "id": "3a6827b9-0dda-401f-8d4c-0bfa3581fa5e"
            }
          ]
        },
        {
          "id": "122de225-f2e0-4904-8a02-fb0b5e122988",
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
              "id": "8009861b-127c-470a-a9f8-a799c441ddd6"
            }
          ]
        },
        {
          "id": "931627c3-b626-488f-97c8-2c3388e114f2",
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
              "id": "8f6d4091-06ec-417d-bdc9-648be97182df"
            }
          ]
        },
        {
          "id": "790d210b-e7bf-4796-b691-09550022b97a",
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
              "id": "aadbbdba-428b-4c77-a345-4776e1169c3a"
            }
          ]
        },
        {
          "id": "13d4b1bd-86ee-4566-989f-27e54b4901b7",
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
              "id": "f56992f4-7bf2-491c-a23c-95aa23c4c111"
            }
          ]
        },
        {
          "id": "b5154dd2-7a2e-48ff-9fb1-15fe428043c9",
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
              "id": "c7fdcf6b-df8b-4f90-9b3b-1ce2c66c38d1"
            }
          ]
        },
        {
          "id": "83ce0502-521c-4dca-8eb1-c9b7d5424488",
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
              "id": "e6b4b1bc-2718-489b-9bf1-39a204ae8342"
            }
          ]
        },
        {
          "id": "3df8c4ae-a375-4962-a837-4d9588fa79d9",
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
              "id": "60488132-8105-461a-a8e4-a9d3cf2365e5"
            }
          ]
        },
        {
          "id": "4683385e-af1c-48ad-bc7b-a9c8a169905d",
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
              "id": "ce5333df-c019-4776-992e-e961cd12f7b9"
            }
          ]
        },
        {
          "id": "d3c92a9d-171c-47d3-b175-021ab80ed621",
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
              "id": "81c52b57-363e-4db4-b2b3-5d4affdafbe9"
            }
          ]
        },
        {
          "id": "38292e43-bacb-4290-8798-39ed25eb7192",
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
              "id": "bc9742b5-bd17-4fab-9931-3495a0e71ee9"
            }
          ]
        },
        {
          "id": "0ffc2069-05e0-450a-b795-a5324447f600",
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
              "id": "3a423ed1-c42a-496d-985c-871ad49c042a"
            }
          ]
        },
        {
          "id": "7fc5fb75-572a-462b-8cde-a824dcae620c",
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
              "id": "759938eb-600f-438f-b92c-7da2d479c2ab"
            }
          ]
        },
        {
          "id": "69ac0685-b459-4601-a757-a4bdb183b981",
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
              "id": "f19cd1e4-1481-42b4-a605-c76eff3bbb11"
            }
          ]
        },
        {
          "id": "31ddb9b2-f6d5-4d3d-892a-584ad1b8972a",
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
              "id": "4a7565c1-6dbc-43c6-9621-5bdd19ca3376"
            }
          ]
        },
        {
          "id": "b5ec2775-0253-467a-9ee1-89270e90c420",
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
              "id": "a00a0904-c17b-4f49-853e-12a87ad39700"
            }
          ]
        }
      ]
    },
    {
      "name": "Checkin",
      "item": [
        {
          "id": "9c2eab84-8e10-44a0-b175-8aa11cee57cc",
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
              "id": "5d71f63c-4da2-45a9-8e1c-53cc658716f7"
            }
          ]
        },
        {
          "id": "720f2dfe-b7ed-4548-ab2d-c79af285526b",
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
              "id": "98eef2bc-00f0-4ec5-809e-d2aef2f7acf0"
            }
          ]
        },
        {
          "id": "07204145-348f-4c78-81b1-b7a64f99a803",
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
              "id": "204e7d7e-f436-4fa2-88ed-91f18a795828"
            }
          ]
        },
        {
          "id": "1b5ddfe3-119b-45dc-89eb-d1447c6873ab",
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
              "id": "f1d2fb28-9492-4e39-a355-2206a8c70f1d"
            }
          ]
        },
        {
          "id": "bd77a03e-53e8-4259-ad04-813159e49259",
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
              "id": "b10453d1-2665-4905-9e35-da5c29b03d1b"
            }
          ]
        },
        {
          "id": "023a778b-091f-444f-ae0c-7035e692d193",
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
              "id": "21b80421-0342-463d-bf1f-12e6ebafc326"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "ed414d9f-0644-4e68-91a4-f9a9d449bfc5",
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
              "id": "040f0fd4-152c-4cd6-b8f6-0cbd1637cbfe"
            }
          ]
        },
        {
          "id": "6596d50d-f0a4-499b-bb9c-ffcb2357e9f5",
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
              "id": "3d39c9d9-21d2-47e8-a2e6-2e6cb4590013"
            }
          ]
        },
        {
          "id": "ba668d64-f7af-4f7b-ace5-2f1a253eac2a",
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
              "id": "f3e65b26-06a7-4ab3-9d1a-2087921825f7"
            }
          ]
        },
        {
          "id": "8bb47b9e-29fe-4e3b-94b2-8270b5f5cddd",
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
              "id": "2f6d2a7a-bad2-4f98-9a13-42741d6e7971"
            }
          ]
        },
        {
          "id": "c5820e09-919c-43c8-aa67-853945701d34",
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
              "id": "0a6ee8cf-590c-48b1-aabb-2013003d50e0"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "8d83fb03-d2d5-45c0-a559-73d5ae99ee3a",
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
              "id": "758f0f6b-8134-4025-a845-e58415347b80"
            }
          ]
        },
        {
          "id": "f6593228-4193-4d79-95e8-726ce7a8e772",
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
              "id": "39db42e7-12d7-4075-b857-73406fb1de7f"
            }
          ]
        },
        {
          "id": "b80f4db4-414d-4ae1-b5e2-4c695e85148b",
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
              "id": "0f258b26-6f82-42b9-82c8-38f166941e3f"
            }
          ]
        },
        {
          "id": "e19ff99f-eb18-4672-84d8-80e9ec2e19da",
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
              "id": "21033f7e-33c7-4497-a87b-c69d5315da7d"
            }
          ]
        },
        {
          "id": "9759fd07-0ae0-4f73-8e69-ea198220cc44",
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
              "id": "a60313ea-98d6-42a0-9e4e-b48353bcb75c"
            }
          ]
        },
        {
          "id": "c70a8d52-3e46-473f-ba27-56878da7e5b6",
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
              "id": "9ea9edd2-4ccc-41c3-8acc-2d6123aa7b9a"
            }
          ]
        },
        {
          "id": "b35bb308-b599-419a-b7de-5d1a241abbfa",
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
              "id": "cd84b3ff-bf55-42c1-a4ae-703b4edb37ae"
            }
          ]
        },
        {
          "id": "964a9112-0fa2-4a16-bd85-f546e35c0da9",
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
              "id": "60c6d234-ab3f-4f92-a672-d929dcb35da7"
            }
          ]
        },
        {
          "id": "1e72f95b-9ef5-402e-8dc7-47d92a5f71c3",
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
              "id": "80e0cc63-a594-4df6-bac7-75e2643347b3"
            }
          ]
        },
        {
          "id": "ac3b664b-fa3d-4e9b-9e50-a0ae68c9345d",
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
              "id": "9c0cd975-8506-4762-b83c-e700d9c3b408"
            }
          ]
        },
        {
          "id": "0de14248-a82c-41b3-9456-3e4c2b33768b",
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
              "id": "c7f4f599-c967-4fec-ac8f-7d8e59bb613c"
            }
          ]
        },
        {
          "id": "7ccf99c0-f7fb-400c-9e8c-c2ceb9c74e47",
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
              "id": "30a98c44-1d4f-41db-9818-4b9bca8435a8"
            }
          ]
        }
      ]
    },
    {
      "name": "Friendlist",
      "item": [
        {
          "id": "2de0859b-7014-4b3e-bea3-f5e49691f81d",
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
              "id": "eba86576-9844-45f1-a14a-d5ac420ce337"
            }
          ]
        },
        {
          "id": "3795de66-40f0-44b0-86bb-facadb84ea54",
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
              "id": "838cd55f-f433-4c8d-b8ea-becd84496198"
            }
          ]
        },
        {
          "id": "b98976fe-e637-4639-b306-2f9697c736db",
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
              "id": "0498c942-6d16-4735-a199-cd34a2eef811"
            }
          ]
        },
        {
          "id": "58a55495-7122-42e5-beae-5a49360573e2",
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
              "id": "7d5600e3-2b9a-44f0-8ee6-40b13c26a920"
            }
          ]
        },
        {
          "id": "138bc9e0-72db-44d3-b23a-3147948a4381",
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
              "id": "7263fbd5-b436-4c0a-8769-23764fd316df"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "d86697be-b6fe-4734-9698-064c42d7fbb1",
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
              "id": "ce7bed87-426a-47f9-b54a-afe44f68e546"
            }
          ]
        },
        {
          "id": "fbd6603a-64eb-4dc6-a5cd-84913d7cfcb3",
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
              "id": "52381cf5-140c-4521-98a6-c2e4c27170cc"
            }
          ]
        },
        {
          "id": "36fea2c1-3855-4daf-8c24-cc6c93cb98e9",
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
              "id": "0a89978f-0d34-486c-9ee8-b4ff04d7d8ea"
            }
          ]
        },
        {
          "id": "43b55106-bc27-4488-b1e1-de89c14811d1",
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
              "id": "9ac2c0a7-24a2-4a31-a2e0-33f286c03a29"
            }
          ]
        },
        {
          "id": "ef4ff3c3-8fd4-44a0-933c-c81a420b912d",
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
              "id": "86cf4768-0501-42a0-bb81-6fc0c66c7f5a"
            }
          ]
        },
        {
          "id": "e0e8e652-773f-4a2a-97c0-1e1eaadcc256",
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
              "id": "22da3330-2b85-43ec-927e-d0edbe8fe362"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "6d31b723-3b3b-4a02-be07-520c5b76d72d",
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
              "id": "2ee5ae36-2754-4435-a6a8-9f4ba335460a"
            }
          ]
        },
        {
          "id": "616e1aea-770d-4c13-86d3-80a62673c549",
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
              "id": "332806ff-feb4-4f43-a97c-d9c91f22af5e"
            }
          ]
        },
        {
          "id": "27e5b653-02d8-4a0f-af30-7607bd2479c4",
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
              "id": "2e1d5462-c97c-47a3-a35e-34f34ce10fd5"
            }
          ]
        },
        {
          "id": "b90efe47-6d71-4fef-abba-5140249d7a11",
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
              "id": "4336e5e4-af16-4ee6-9791-aa1e2451882b"
            }
          ]
        },
        {
          "id": "d94180df-d4e4-4e54-8e95-777dcbe5dbb7",
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
              "id": "0703ccb0-59f1-4ef3-9c7f-81af910df85e"
            }
          ]
        },
        {
          "id": "48ba7dfa-227e-4a44-bf19-45df014c4418",
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
              "id": "6ead429c-5dc7-4368-9237-ab51472b773e"
            }
          ]
        }
      ]
    },
    {
      "name": "Note",
      "item": [
        {
          "id": "95e5e8f0-8dd2-4ab5-9140-87955fd23135",
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
              "id": "7ab7677e-12b2-42a7-aa1e-b2b6735d6be0"
            }
          ]
        },
        {
          "id": "f221a0d9-50c2-4614-bbc0-628d9f99e45a",
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
              "id": "0b2307c4-9f32-4e93-9c85-01c0166d7625"
            }
          ]
        },
        {
          "id": "a33f943d-8fe8-41d3-a0e6-aad4a41d9175",
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
              "id": "c479735f-95f1-4cbf-bf9e-b027d521c60d"
            }
          ]
        },
        {
          "id": "3687cf2f-e3e1-4810-8489-8f8e14284d3c",
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
              "id": "d0086393-0a18-4f5d-b42a-217df1541f97"
            }
          ]
        },
        {
          "id": "a4c0f220-2900-4b06-beab-49821519767c",
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
              "id": "13bff1dd-931f-487c-af60-0b432d96006c"
            }
          ]
        },
        {
          "id": "573ddcc6-3dee-49fc-be5c-a8f44dae040d",
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
              "id": "4e50098e-67cf-4ee3-9c96-0b621d915c8d"
            }
          ]
        }
      ]
    },
    {
      "name": "Page",
      "item": [
        {
          "id": "4b60cbb9-160c-442b-a45e-a96d694412bb",
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
              "id": "b5faeb63-d709-41af-b031-f81dbfc3a6f5"
            }
          ]
        },
        {
          "id": "555b95e4-eb32-4f26-bcb4-c951771b2f13",
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
              "id": "5a7f68c3-e29a-47e0-8f51-e61a69cb82ea"
            }
          ]
        },
        {
          "id": "1b7b2a86-7ec4-4d4c-8db9-f9a41c1b1eed",
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
              "id": "d57da5a6-06c6-476e-908b-e78d647d310b"
            }
          ]
        },
        {
          "id": "35f1df17-468a-4336-a397-ae53385448cc",
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
              "id": "4e481bee-b31f-4b9b-a8fa-cf457022273f"
            }
          ]
        },
        {
          "id": "e92dd461-604e-4146-9102-19e3c7e60863",
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
              "id": "73de5c1c-2af0-40a6-aaae-d7475d9862a4"
            }
          ]
        },
        {
          "id": "da48c2b5-97c6-4914-9956-2b84aff0cfb5",
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
              "id": "afa09154-52ff-483e-9a68-2d13967dd244"
            }
          ]
        },
        {
          "id": "1370d130-ef97-4ee6-8b27-4900ce0b92cf",
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
              "id": "edb2095f-6699-4e41-8ed3-2e4232079522"
            }
          ]
        },
        {
          "id": "c85c4158-ac0a-49ea-a081-bc1f320ad03c",
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
              "id": "cddb8b5d-8ff0-49ea-8cb2-2860ccd48a93"
            }
          ]
        },
        {
          "id": "17bec4b6-9f0c-47f2-a239-b5e2f8e7e660",
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
              "id": "6bbc44c5-6288-47cd-883e-9121202be92d"
            }
          ]
        },
        {
          "id": "65177813-9f33-45df-aa19-7bf19857d327",
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
              "id": "7908acab-7655-48c1-9902-e51c0dcff0c8"
            }
          ]
        },
        {
          "id": "ae6dc52d-fbd4-415f-8efd-680ed9beb042",
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
              "id": "27004a99-2bc2-40c4-9d0f-9959353a9205"
            }
          ]
        },
        {
          "id": "a7da079f-f714-4469-b8c4-3ceb74cbb1ce",
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
              "id": "91cf173c-cea1-4e3e-857e-72f7b2fb6e22"
            }
          ]
        },
        {
          "id": "c1f46418-4a13-42c7-bad6-7dbf43335fc9",
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
              "id": "307e7ff8-85d6-45b3-a74e-4277e6b55550"
            }
          ]
        },
        {
          "id": "4afa11d0-61e4-492d-a737-d22cf5db3584",
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
              "id": "366907e7-10e0-4fae-a6b1-be0056069f6e"
            }
          ]
        },
        {
          "id": "f6e362ed-8890-4808-9660-27fda9ab235b",
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
              "id": "8f1281bb-545c-4694-a6fc-87c29937da29"
            }
          ]
        },
        {
          "id": "eae9b5da-3f22-40e5-9316-55e968e69630",
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
              "id": "ad7b13c7-95ae-4247-8f2b-a977708cbaf5"
            }
          ]
        },
        {
          "id": "82f85d12-4560-4486-bba2-674dc63e3b4e",
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
              "id": "9563136b-bd00-490c-9888-89efbea443bd"
            }
          ]
        },
        {
          "id": "35449781-9ec8-488e-922e-c2a01773ed1f",
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
              "id": "9a99a5e2-a88e-4ccb-802b-3887daf6da62"
            }
          ]
        },
        {
          "id": "f8303aa5-2331-4770-ad00-f33719a49da8",
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
              "id": "e48551f9-f8b7-4e7b-af74-a892ac7e17df"
            }
          ]
        },
        {
          "id": "a8ccfb6b-5f87-42a4-972b-c9f38fd14e11",
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
              "id": "c65ba09f-7cf9-4ac9-b9ab-99cf1a0f06eb"
            }
          ]
        },
        {
          "id": "2b7c05bc-a790-4113-bd11-7de76127e43d",
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
              "id": "ef84aec3-62dd-49c6-9602-596f802b082e"
            }
          ]
        },
        {
          "id": "73eca4d6-0024-47fa-af8e-9f84b412fccb",
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
              "id": "625eed8c-2f24-4e4e-a47c-034d767313da"
            }
          ]
        },
        {
          "id": "5cafffc8-f00e-4f49-9a8a-17d224ad7e01",
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
              "id": "8cf80229-c366-40f6-9236-f72d77f3cbf2"
            }
          ]
        },
        {
          "id": "80c3590a-2f2e-450c-a306-9b189fef0385",
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
              "id": "b03ea7ef-4b58-46a8-a9f8-02a6eb6ea7e8"
            }
          ]
        },
        {
          "id": "0c0fb0d2-e226-4ca3-b89e-3a372833bdd9",
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
              "id": "36ea359d-a9a1-46f7-9517-16d53b56f285"
            }
          ]
        },
        {
          "id": "350a5d6a-52b6-4474-a7de-8e8e1764d9b7",
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
              "id": "e0953f20-a0db-49fa-be1b-a4883cc7dec7"
            }
          ]
        },
        {
          "id": "a6e6b4b5-d006-4e88-9327-72b1cda3f943",
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
              "id": "1659e90b-fce7-4409-b4f8-12499c0f3407"
            }
          ]
        },
        {
          "id": "e3fc91e0-4073-4e83-be66-001a9260b902",
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
              "id": "763f14b5-fb98-4891-9b5a-65f69b35cb4f"
            }
          ]
        },
        {
          "id": "1647c330-dbca-4c21-b3f6-45fe47111e68",
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
              "id": "84ae06f4-fcd5-4b44-bbbf-61c3436ddbea"
            }
          ]
        },
        {
          "id": "629a3e9e-0bbb-4e0f-8849-5195e46abd24",
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
              "id": "0cd1b1f4-dae4-49b1-ab96-c0cc3f70eb2f"
            }
          ]
        },
        {
          "id": "e9fee752-5d6f-49db-8a71-8f29cf45e672",
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
              "id": "0181a047-517b-4c26-ad4c-d3dccadaafd4"
            }
          ]
        },
        {
          "id": "20e35e4b-8c32-4a49-b91a-9a9421d804d8",
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
              "id": "ed18a7e6-a653-43fc-9d03-92b96ef0a8b7"
            }
          ]
        }
      ]
    },
    {
      "name": "Photo",
      "item": [
        {
          "id": "4a430ebd-f276-4896-8bef-3d6834f3d763",
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
              "id": "f762bcb0-7ff5-4452-a0e0-0eb9901b8ca9"
            }
          ]
        },
        {
          "id": "a11ec8c9-2a9c-4e07-886a-c75547766ad9",
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
              "id": "7e6e563f-491a-488c-bf0e-c49e99f93fc4"
            }
          ]
        },
        {
          "id": "d5281153-bb5c-4363-88ed-3c2dfcb7074f",
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
              "id": "f7c20c2a-3d4a-46c8-8768-a35d2b416f95"
            }
          ]
        },
        {
          "id": "f45da988-bc2a-4893-87a0-d17608eae9af",
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
              "id": "2fa1b1c6-6e16-47ad-81b9-a4a6c1d6b339"
            }
          ]
        },
        {
          "id": "aabe03c4-0bfe-42c0-8e1e-3e5b0d9826f7",
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
              "id": "106a965d-5d3b-4081-b260-08eb6c33a762"
            }
          ]
        },
        {
          "id": "9c005ba5-5af2-4af0-8edf-a4f04863bf7a",
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
              "id": "1724de54-e856-4673-af34-4533ae67c399"
            }
          ]
        },
        {
          "id": "a35d2838-5c93-4987-9a48-dcf0823c8bc6",
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
              "id": "1c22c91f-239f-4ee0-8736-8c8396dcdd40"
            }
          ]
        },
        {
          "id": "8cd0d944-ed68-4f1e-b7de-904141baae15",
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
              "id": "f20192ed-f75b-44d1-9f82-e2348e056edd"
            }
          ]
        },
        {
          "id": "a2ee8178-67b7-4cfe-bb87-5a6c5f7024a0",
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
              "id": "c86ec3c9-72d2-4b68-a5d6-2ad2638cb546"
            }
          ]
        },
        {
          "id": "b9c0ad10-444a-4791-b9e6-0c211c3a9cb2",
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
              "id": "3f56f5bf-1bae-4170-b6aa-a150cd7ed6a2"
            }
          ]
        }
      ]
    },
    {
      "name": "Post",
      "item": [
        {
          "id": "5cf7dc38-4d42-437b-ba19-e00c73cf28b6",
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
              "id": "0d114332-3adf-4c2a-9ba8-a398e3cf1f75"
            }
          ]
        },
        {
          "id": "77bb009a-2225-4887-81e6-deca3be10290",
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
              "id": "71588d5e-68e1-40bc-b651-bfef1fd3008a"
            }
          ]
        },
        {
          "id": "da90a29b-85a3-4538-8ce7-bfa1ee36a348",
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
              "id": "ec86f96c-541d-4753-b3d3-8f778ea1e7df"
            }
          ]
        },
        {
          "id": "f573f374-bb72-4a52-80d3-7a5affce3f72",
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
              "id": "eb8b3000-b70a-4f5e-b452-75d3aa322836"
            }
          ]
        },
        {
          "id": "40b758c2-011b-4d49-ad53-f934972fb63b",
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
              "id": "44f5ad3d-344b-41ea-af08-9ab84a2b3c33"
            }
          ]
        },
        {
          "id": "6ef98eb0-67e9-4c36-b4c3-b320d5a3410d",
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
              "id": "1bdb42b6-8a4b-424c-aeec-074024f39f02"
            }
          ]
        }
      ]
    },
    {
      "name": "Status",
      "item": [
        {
          "id": "14e8e4bd-c787-4dec-a037-4407326a0831",
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
              "id": "1ccd6597-6e76-4e3b-b0ff-65b39d4be408"
            }
          ]
        },
        {
          "id": "98faea80-5d70-4a1b-a277-2fe4200fa574",
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
              "id": "74762544-b09c-440f-9720-ae2112145a11"
            }
          ]
        },
        {
          "id": "c34f1f96-47d0-41c3-a756-7d8d01555570",
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
              "id": "39c02522-a57f-4161-b480-e71dde4f6317"
            }
          ]
        },
        {
          "id": "576c7dd2-1d4f-4d30-a275-393c94b975fa",
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
              "id": "e0907364-366a-4888-bcca-07e79f9f8d14"
            }
          ]
        },
        {
          "id": "f9989787-4511-4437-98d3-ac82a710cf17",
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
              "id": "2d9f215d-237e-4ca6-9490-88ba19032053"
            }
          ]
        },
        {
          "id": "571b9211-e3d1-436e-b44f-faa0db77c5b6",
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
              "id": "46064841-6dec-45e3-96af-d515b395b6a3"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "0884feaa-0591-403a-bdb0-ece2c7eec7e8",
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
              "id": "d8454f0e-cc2b-4771-9a74-4eae664325e6"
            }
          ]
        },
        {
          "id": "39c9f6ff-f62c-4b28-a169-a4fed17fc215",
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
              "id": "75bc32c5-748a-472d-8aab-da13db08db98"
            }
          ]
        },
        {
          "id": "b4de055c-ac0a-41df-9510-7e81af496c47",
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
              "id": "24dfa31b-7e8e-4329-bd54-1428ab41f74b"
            }
          ]
        },
        {
          "id": "ddfcec8a-4dee-4b76-ada5-abf9c91babd7",
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
              "id": "a1d02e4a-e874-4afd-b558-d95d7ad979b8"
            }
          ]
        },
        {
          "id": "71375ad2-20f3-41e2-9cc7-c37e8e79ccb5",
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
              "id": "321de931-5603-4a6f-b58e-961df1213fe9"
            }
          ]
        },
        {
          "id": "5140934a-14fb-4300-b114-d0a275824be6",
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
              "id": "b68772c9-1a90-44f7-bf99-a74487b7de94"
            }
          ]
        },
        {
          "id": "2ac48b13-b8f5-46cf-bc9d-1c7bbfc2a40b",
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
              "id": "087adc26-c10a-4aa5-9404-bfa0bf2cc46f"
            }
          ]
        },
        {
          "id": "75074940-d7e0-431d-8be1-c8c69d193590",
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
              "id": "01a87734-ddf4-49ce-8a89-50c35ff5c735"
            }
          ]
        },
        {
          "id": "ffb6d4ef-2a68-4546-96f4-fc44c9631016",
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
              "id": "ee70403a-fc5e-4371-bba3-f8192c18df53"
            }
          ]
        }
      ]
    }
  ]
}