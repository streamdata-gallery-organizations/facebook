---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Post Object Comments
  description: 'This reference describes the /comments edge that is common to multiple
    Graph API nodes. The structure and operations are the same for each node. The
    following objects has a /comments edge:'
  termsOfService: https://www.facebook.com/policies/
  version: 1.0.0
host: graph.facebook.com
basePath: /v3.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /&#123;object-id&#125;/comments:
    get:
      summary: Get Object Comments
      description: 'This reference describes the /comments edge that is common to
        multiple Graph API nodes. The structure and operations are the same for each
        node. The following objects has a /comments edge:'
      operationId: getObjectComments
      x-api-path-slug: 123objectid125comments-get
      parameters:
      - in: query
        name: order
        description: Order in which comments were returned
        type: string
      - in: query
        name: total_count
        description: The count of comments on this node
        type: string
      responses:
        200:
          description: OK
      tags:
      - Object
      - Comments
    post:
      summary: Post Object Comments
      description: 'This reference describes the /comments edge that is common to
        multiple Graph API nodes. The structure and operations are the same for each
        node. The following objects has a /comments edge:'
      operationId: postObjectComments
      x-api-path-slug: 123objectid125comments-post
      parameters:
      - in: query
        name: attachment_id
        description: An optional ID of a unpublished photo (see no_story field in
          /&#123;user-id&#125;/photos) uploaded to Facebook to include as a photo
          comment
        type: string
      - in: query
        name: attachment_url
        description: The URL of an image to include as a photo comment
        type: string
      - in: query
        name: message
        description: The comment text
        type: string
      - in: query
        name: source
        description: A photo, encoded as form data, to use as a photo comment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Object
      - Comments
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---