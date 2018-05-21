{
  "info": {
    "name": "Facebook Get Canvas Veo",
    "_postman_id": "6066a2dd-4d73-41bb-900c-e1bfe95daca9",
    "description": "Canvas Video",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Canvas",
      "item": [
        {
          "id": "14f10ac1-a0e1-4209-81e5-5113cef40007",
          "name": "getCanvasVeo",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;canvas-video-id&#125;?bottom_paddingnumeric string=bottom_paddingnumeric%20string&element_group_keystring=element_group_keystring&element_typeenum=element_typeenum&idnumeric string=idnumeric%20string&namestring=namestring&styleenum=styleenum&top_paddingnumeric string=top_paddingnumeric%20string&videoVideo=videoVideo",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Canvas Video"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "911415df-06f5-4d05-a625-6d30fe192951"
            }
          ]
        }
      ]
    }
  ]
}