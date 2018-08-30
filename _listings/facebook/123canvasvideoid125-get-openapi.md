---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get Canvas Veo
  description: Canvas Video
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
  /&#123;object-id&#125;/likes:
    get:
      summary: Get Object Likes
      description: 'This reference describes the /likes edge that is common to multiple
        Graph API nodes. The structure and operations are the same for each node,
        except that for the following nodes, /likes returns only the profile for the
        current user if read with a user access token:'
      operationId: getObjectLikes
      x-api-path-slug: 123objectid125likes-get
      parameters:
      - in: query
        name: total_count
        description: Total number of User and Page likes on the object
        type: string
      responses:
        200:
          description: OK
      tags:
      - Object
      - Likes
    post:
      summary: Post Object Likes
      description: 'This reference describes the /likes edge that is common to multiple
        Graph API nodes. The structure and operations are the same for each node,
        except that for the following nodes, /likes returns only the profile for the
        current user if read with a user access token:'
      operationId: postObjectLikes
      x-api-path-slug: 123objectid125likes-post
      responses:
        200:
          description: OK
      tags:
      - Object
      - Likes
    delete:
      summary: Delete Object Likes
      description: 'This reference describes the /likes edge that is common to multiple
        Graph API nodes. The structure and operations are the same for each node,
        except that for the following nodes, /likes returns only the profile for the
        current user if read with a user access token:'
      operationId: deleteObjectLikes
      x-api-path-slug: 123objectid125likes-delete
      responses:
        200:
          description: OK
      tags:
      - Object
      - Likes
  /&#123;achievement-type-id&#125;:
    get:
      summary: Get Achievement Type
      description: A games achievement type created by a Facebook App. Not to be confused
        with an instance of an achievement.
      operationId: getAchievementType
      x-api-path-slug: 123achievementtypeid125-get
      parameters:
      - in: query
        name: application
        description: The app that created the achievement
        type: string
      - in: query
        name: context
        description: Context of the achievement for the associated app
        type: string
      - in: query
        name: created_time
        description: Time when the achievement was created
        type: string
      - in: query
        name: data
        description: An object containing the points this achievement is worth
        type: string
      - in: query
        name: description
        description: Description of the achievement
        type: string
      - in: query
        name: height
        description: Pixel height of the image
        type: string
      - in: query
        name: id
        description: ID of the achievement type
        type: string
      - in: query
        name: image
        description: Image for the achievement
        type: string
      - in: query
        name: is_scraped
        description: Whether the URL containing the achievement metadata has been
          scraped by Facebook servers
        type: string
      - in: query
        name: points
        description: Number of points that this achievement is worth
        type: string
      - in: query
        name: title
        description: Title of achievement
        type: string
      - in: query
        name: type
        description: The value will be games
        type: string
      - in: query
        name: updated_time
        description: Time when the achievement was last updated
        type: string
      - in: query
        name: url
        description: Unique URL of the achievement
        type: string
      - in: query
        name: width
        description: Pixel width of the image
        type: string
      responses:
        200:
          description: OK
      tags:
      - Achievement
      - Type
  /&#123;album-id&#125;:
    get:
      summary: Get Album
      description: Represents a photo album. The /&#123;album-id&#125; node returns
        a single album.
      operationId: getAlbum
      x-api-path-slug: 123albumid125-get
      parameters:
      - in: query
        name: can_upload
        description: Whether the viewer can upload photos to this album
        type: string
      - in: query
        name: count
        description: The approximate number of photos in the album
        type: string
      - in: query
        name: cover_photo
        description: The ID of the album&#039;s cover photo
        type: string
      - in: query
        name: created_time
        description: The time the album was initially created
        type: string
      - in: query
        name: description
        description: The description of the album
        type: string
      - in: query
        name: event
        description: The event associated with this album
        type: string
      - in: query
        name: from
        description: The current user, if the current user created the album
        type: string
      - in: query
        name: id
        description: The album ID
        type: string
      - in: query
        name: link
        description: A link to this album on Facebook
        type: string
      - in: query
        name: location
        description: The textual location of the album
        type: string
      - in: query
        name: name
        description: The title of the album
        type: string
      - in: query
        name: place
        description: The place associated with this album
        type: string
      - in: query
        name: privacy
        description: The privacy settings for the album
        type: string
      - in: query
        name: type
        description: The type of the album
        type: string
      - in: query
        name: updated_time
        description: The last time the album was updated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Album
  /&#123;album-id&#125;/picture:
    get:
      summary: Get Album Picture
      description: The cover photo of a photo album.
      operationId: getAlbumPicture
      x-api-path-slug: 123albumid125picture-get
      responses:
        200:
          description: OK
      tags:
      - Album
      - Picture
  /&#123;album-id&#125;/photos:
    get:
      summary: Get Album Photos
      description: The photos in an album on Facebook.
      operationId: getAlbumPhotos
      x-api-path-slug: 123albumid125photos-get
      responses:
        200:
          description: OK
      tags:
      - Album
      - Photos
  /&#123;object-id&#125;/sharedposts:
    get:
      summary: Get Object Sharedadds
      description: The /sharedposts edge that is common to multiple Graph API nodes.
        The structure and operations are the same for each node.
      operationId: getObjectSharedadds
      x-api-path-slug: 123objectid125sharedposts-get
      responses:
        200:
          description: OK
      tags:
      - Object
      - Sharedadds
  /&#123;canvas-video-id&#125;:
    get:
      summary: Get Canvas Veo
      description: Canvas Video
      operationId: getCanvasVeo
      x-api-path-slug: 123canvasvideoid125-get
      parameters:
      - in: query
        name: bottom_paddingnumeric string
        description: The padding below the element
        type: string
      - in: query
        name: element_group_keystring
        description: The element group key to bundle multiple elements in editing
        type: string
      - in: query
        name: element_typeenum
        description: The type of the elementDefault
        type: string
      - in: query
        name: idnumeric string
        description: The id of the element
        type: string
      - in: query
        name: namestring
        description: The name of the elementDefault
        type: string
      - in: query
        name: styleenum
        description: The presentation style of the video
        type: string
      - in: query
        name: top_paddingnumeric string
        description: The padding above the element
        type: string
      - in: query
        name: videoVideo
        description: The facebook video node
        type: string
      responses:
        200:
          description: OK
      tags:
      - Canvas
      - Veo
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