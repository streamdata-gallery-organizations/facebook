---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get Object Comments
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
x-streamrank:
  polling_total_time_average: ~
  polling_size_download_average: ~
  streaming_total_time_average: ~
  streaming_size_download_average: ~
  change_yes: ~
  change_no: ~
  time_percentage: ~
  size_percentage: ~
  change_percentage: "200"
  last_run: ~
  days_run: ~
  minute_run: ~
---