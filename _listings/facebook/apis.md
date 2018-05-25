---
name: Facebook
x-slug: facebook
description: Create an account or log into Facebook. Connect with friends, family
  and other people you know. Share photos and videos, send messages and get updates.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
x-kinRank: "9"
x-alexaRank: "3"
tags: Facebook
created: "2018-05-25"
modified: "2018-05-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/apis.md
specificationVersion: "0.14"
apis:
- name: Facebook Get Object Comments
  x-api-slug: facebook
  description: 'This reference describes the /comments edge that is common to multiple
    Graph API nodes. The structure and operations are the same for each node. The
    following objects has a /comments edge:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;object-id&#125;/comments
  tags: Object,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123objectid125comments-get-openapi.md
- name: Facebook Post Object Comments
  x-api-slug: facebook
  description: 'This reference describes the /comments edge that is common to multiple
    Graph API nodes. The structure and operations are the same for each node. The
    following objects has a /comments edge:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;object-id&#125;/comments
  tags: Object,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123objectid125comments-post-openapi.md
- name: Facebook Get Object Likes
  x-api-slug: facebook
  description: 'This reference describes the /likes edge that is common to multiple
    Graph API nodes. The structure and operations are the same for each node, except
    that for the following nodes, /likes returns only the profile for the current
    user if read with a user access token:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;object-id&#125;/likes
  tags: Object,Likes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123objectid125likes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123objectid125likes-get-openapi.md
- name: Facebook Post Object Likes
  x-api-slug: facebook
  description: 'This reference describes the /likes edge that is common to multiple
    Graph API nodes. The structure and operations are the same for each node, except
    that for the following nodes, /likes returns only the profile for the current
    user if read with a user access token:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;object-id&#125;/likes
  tags: Object,Likes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123objectid125likes-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123objectid125likes-post-openapi.md
- name: Facebook Delete Object Likes
  x-api-slug: facebook
  description: 'This reference describes the /likes edge that is common to multiple
    Graph API nodes. The structure and operations are the same for each node, except
    that for the following nodes, /likes returns only the profile for the current
    user if read with a user access token:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;object-id&#125;/likes
  tags: Object,Likes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123objectid125likes-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123objectid125likes-delete-openapi.md
- name: Facebook Get Achievement Type
  x-api-slug: facebook
  description: A games achievement type created by a Facebook App. Not to be confused
    with an instance of an achievement.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;achievement-type-id&#125;
  tags: Achievement,Type
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123achievementtypeid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123achievementtypeid125-get-openapi.md
- name: Facebook Get Album
  x-api-slug: facebook
  description: Represents a photo album. The /&#123;album-id&#125; node returns a
    single album.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;album-id&#125;
  tags: Album
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123albumid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123albumid125-get-openapi.md
- name: Facebook Get Album Picture
  x-api-slug: facebook
  description: The cover photo of a photo album.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;album-id&#125;/picture
  tags: Album,Picture
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123albumid125picture-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123albumid125picture-get-openapi.md
- name: Facebook Get Album Photos
  x-api-slug: facebook
  description: The photos in an album on Facebook.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;album-id&#125;/photos
  tags: Album,Photos
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123albumid125photos-get-openapi.md
- name: Facebook Get Object Sharedadds
  x-api-slug: facebook
  description: The /sharedposts edge that is common to multiple Graph API nodes. The
    structure and operations are the same for each node.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;object-id&#125;/sharedposts
  tags: Object,Sharedadds
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123objectid125sharedposts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123objectid125sharedposts-get-openapi.md
- name: Facebook Get Canvas Veo
  x-api-slug: facebook
  description: Canvas Video
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;canvas-video-id&#125;
  tags: Canvas,Veo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasvideoid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasvideoid125-get-openapi.md
- name: Facebook Get Application Context
  x-api-slug: facebook
  description: Application Context
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;application-context-id&#125;
  tags: Application,Context
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123applicationcontextid125-get-openapi.md
- name: Facebook Get Analytics App Events Export
  x-api-slug: facebook
  description: Analytics App Events Export
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;analytics-app-events-export-id&#125;
  tags: Analytics,App,Events,Export
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123analyticsappeventsexportid125-get-openapi.md
- name: Facebook Get Application
  x-api-slug: facebook
  description: Application
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;application-id&#125;
  tags: Application
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123applicationid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123applicationid125-get-openapi.md
- name: Facebook Get Audience Insights Rule
  x-api-slug: facebook
  description: Audience Insights Rule
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;audience-insights-rule-id&#125;
  tags: Audience,Insights,Rule
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123audienceinsightsruleid125-get-openapi.md
- name: Facebook Get Canvas
  x-api-slug: facebook
  description: Canvas
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;canvas-id&#125;
  tags: Canvas
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasid125-get-openapi.md
- name: Facebook Get Canvas Button
  x-api-slug: facebook
  description: Canvas Button
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;canvas-button-id&#125;
  tags: Canvas,Button
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasbuttonid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasbuttonid125-get-openapi.md
- name: Facebook Get Canvas Carousel
  x-api-slug: facebook
  description: Canvas Carousel
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;canvas-carousel-id&#125;
  tags: Canvas,Carousel
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvascarouselid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvascarouselid125-get-openapi.md
- name: Facebook Get Canvas Footer
  x-api-slug: facebook
  description: Canvas Footer
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;canvas-footer-id&#125;
  tags: Canvas,Footer
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasfooterid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasfooterid125-get-openapi.md
- name: Facebook Get Canvas Header
  x-api-slug: facebook
  description: Canvas Header
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;canvas-header-id&#125;
  tags: Canvas,Header
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasheaderid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasheaderid125-get-openapi.md
- name: Facebook Get Canvas Photo
  x-api-slug: facebook
  description: Canvas Photo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;canvas-photo-id&#125;
  tags: Canvas,Photo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasphotoid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasphotoid125-get-openapi.md
- name: Facebook Get Canvas Product Set
  x-api-slug: facebook
  description: Canvas Product Set
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;canvas-product-set-id&#125;
  tags: Canvas,Product,Set
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasproductsetid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasproductsetid125-get-openapi.md
- name: Facebook Get Canvas Store Locator
  x-api-slug: facebook
  description: Canvas Store Locator
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;canvas-store-locator-id&#125;
  tags: Canvas,Store,Locator
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasstorelocatorid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvasstorelocatorid125-get-openapi.md
- name: Facebook Get Canvas Text
  x-api-slug: facebook
  description: Canvas Text
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;canvas-text-id&#125;
  tags: Canvas,Text
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvastextid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123canvastextid125-get-openapi.md
- name: Facebook Get Comment
  x-api-slug: facebook
  description: A comment can be made on various types of content on Facebook. Most
    Graph API nodes have a /comments edge that lists all the comments on that object.
    The /&#123;comment-id&#125; node returns a single comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;comment-id&#125;
  tags: Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123commentid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123commentid125-get-openapi.md
- name: Facebook Delete Comment
  x-api-slug: facebook
  description: A comment can be made on various types of content on Facebook. Most
    Graph API nodes have a /comments edge that lists all the comments on that object.
    The /&#123;comment-id&#125; node returns a single comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;comment-id&#125;
  tags: Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123commentid125-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123commentid125-delete-openapi.md
- name: Facebook Post Comment
  x-api-slug: facebook
  description: A comment can be made on various types of content on Facebook. Most
    Graph API nodes have a /comments edge that lists all the comments on that object.
    The /&#123;comment-id&#125; node returns a single comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;comment-id&#125;
  tags: Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123commentid125-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123commentid125-post-openapi.md
- name: Facebook Post Object Private Replies
  x-api-slug: facebook
  description: 'This edge allows Pages to reply to Post Comments and Visitor Posts
    with a private Message. It can be used with the following nodes:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;object-id&#125;/private_replies
  tags: Object,Private,Replies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123objectid125private-replies-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123objectid125private-replies-post-openapi.md
- name: Facebook Get Conversation
  x-api-slug: facebook
  description: A Facebook Messages conversation between a person and a Facebook Page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;conversation-id&#125;
  tags: Conversation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123conversationid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123conversationid125-get-openapi.md
- name: Facebook Get Conversation Messages
  x-api-slug: facebook
  description: The messages in a conversation between a person and a page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;conversation-id&#125;/messages
  tags: Conversation,Messages
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123conversationid125messages-get-openapi.md
- name: Facebook Post Conversation Messages
  x-api-slug: facebook
  description: The messages in a conversation between a person and a page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;conversation-id&#125;/messages
  tags: Conversation,Messages
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123conversationid125messages-post-openapi.md
- name: Facebook Get Debug Token Input Token Input Token
  x-api-slug: facebook
  description: This endpoint returns metadata about a given access token. This includes
    data such as the user for which the token was issued, whether the token is still
    valid, when it expires, and what permissions the app has for the given user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//debug_token?input_token=&#123;input-token&#125;
  tags: Debug,Token,Input,Token,Input,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/debug-tokeninput-token123inputtoken125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/debug-tokeninput-token123inputtoken125-get-openapi.md
- name: Facebook Get Doc
  x-api-slug: facebook
  description: Doc
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;doc-id&#125;
  tags: Doc
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123docid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123docid125-get-openapi.md
- name: Facebook Get Domain
  x-api-slug: facebook
  description: The Domain Insights dashboard and API is no longer available. This
    change effects all versions of this API. To see referral traffic for your website,
    and demographic details of your visitors, use Facebook Analytics instead. For
    more information, see Referral Insights with Facebook Analytics.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;domain-id&#125;
  tags: Domain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123domainid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123domainid125-get-openapi.md
- name: Facebook Get Event
  x-api-slug: facebook
  description: Event
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;event-id&#125;
  tags: Event
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123eventid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123eventid125-get-openapi.md
- name: Facebook Get Friend List
  x-api-slug: facebook
  description: Friend List
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;friend-list-id&#125;
  tags: Friend,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123friendlistid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123friendlistid125-get-openapi.md
- name: Facebook Get Group Admins
  x-api-slug: facebook
  description: This edge was deprecated on April 4th, 2018, and can no longer be used.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;group-id&#125;/admins
  tags: Group,Admins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupid125admins-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupid125admins-get-openapi.md
- name: Facebook Get Group Albums
  x-api-slug: facebook
  description: The photo albums created for a Group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;group-id&#125;/albums
  tags: Group,Albums
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupid125albums-get-openapi.md
- name: Facebook Post Me Albums
  x-api-slug: facebook
  description: The photo albums created for a Group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//me/albums
  tags: Me,Albums
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mealbums-post-openapi.md
- name: Facebook Get Group Docs
  x-api-slug: facebook
  description: The documents owned by a Group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;group-id&#125;/docs
  tags: Group,Docs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupid125docs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupid125docs-get-openapi.md
- name: Facebook Get Group Events
  x-api-slug: facebook
  description: All events that belong to a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;group-id&#125;/events
  tags: Group,Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupid125events-get-openapi.md
- name: Facebook Get Group Feed
  x-api-slug: facebook
  description: Posts owned by a Group, including status updates and links.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;group-id&#125;/feed
  tags: Group,Feed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupid125feed-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupid125feed-get-openapi.md
- name: Facebook Post Group Feed
  x-api-slug: facebook
  description: Posts owned by a Group, including status updates and links.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;group-id&#125;/feed
  tags: Group,Feed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupid125feed-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupid125feed-post-openapi.md
- name: Facebook Get Group Files
  x-api-slug: facebook
  description: The files uploaded to this group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;group-id&#125;/files
  tags: Group,Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupid125files-get-openapi.md
- name: Facebook Get Group Members
  x-api-slug: facebook
  description: This edge was deprecated on April 4th, 2018, and can no longer be used.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;group-id&#125;/members
  tags: Group,Members
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupid125members-get-openapi.md
- name: Facebook Get Group Veos
  x-api-slug: facebook
  description: Videos owned by a Facebook Group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;group-id&#125;/videos
  tags: Group,Veos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupid125videos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupid125videos-get-openapi.md
- name: Facebook Get Group Doc
  x-api-slug: facebook
  description: Represents a doc within a Facebook group. The /&#123;group-doc-id&#125;
    node returns a single doc.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;group-doc-id&#125;
  tags: Group,Doc
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupdocid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123groupdocid125-get-openapi.md
- name: Facebook Get Life Event
  x-api-slug: facebook
  description: Life Event
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;life-event-id&#125;
  tags: Life,Event
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123lifeeventid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123lifeeventid125-get-openapi.md
- name: Facebook Get Link
  x-api-slug: facebook
  description: A link shared on Facebook.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;link-id&#125;
  tags: Link
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123linkid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123linkid125-get-openapi.md
- name: Facebook Delete Link
  x-api-slug: facebook
  description: A link shared on Facebook.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;link-id&#125;
  tags: Link
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123linkid125-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123linkid125-delete-openapi.md
- name: Facebook Get Live Veo
  x-api-slug: facebook
  description: Live Video
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;live-video-id&#125;
  tags: Live,Veo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123livevideoid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123livevideoid125-get-openapi.md
- name: Facebook Get Mailing Address
  x-api-slug: facebook
  description: Mailing Address
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;mailing-address-id&#125;
  tags: Mailing,Ress
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123mailingaddressid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123mailingaddressid125-get-openapi.md
- name: Facebook Get Message
  x-api-slug: facebook
  description: An individual message in Facebook Messenger.  This is a Pages-only
    endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;message-id&#125;
  tags: Message
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123messageid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123messageid125-get-openapi.md
- name: Facebook Get Message Attachments
  x-api-slug: facebook
  description: Files attached to a message. This is a Pages-only endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;message-id&#125;/attachments
  tags: Message,Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123messageid125attachments-get-openapi.md
- name: Facebook Get Message Shares
  x-api-slug: facebook
  description: Shared items in a message. This is a Pages-only endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;message-id&#125;/shares
  tags: Message,Shares
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123messageid125shares-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123messageid125shares-get-openapi.md
- name: Facebook Get Milestone
  x-api-slug: facebook
  description: This represents a milestone on a Facebook Page. The /&#123;milestone-id&#125;
    node returns a single &#039;milestone&#039;.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;milestone-id&#125;
  tags: Milestone
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123milestoneid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123milestoneid125-get-openapi.md
- name: Facebook Native Offer
  x-api-slug: facebook
  description: Native Offer
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0/offer
  tags: Native,Offer
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/offer-native-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/offer-native-openapi.md
- name: Facebook Get Notification
  x-api-slug: facebook
  description: An individual unread Facebook notification.  This is an API that&#039;s
    only available for Pages.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;notification-id&#125;
  tags: Notification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123notificationid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123notificationid125-get-openapi.md
- name: Facebook Get Open Graph Action Type
  x-api-slug: facebook
  description: Open Graph Action Type
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;open-graph-action-type-id&#125;
  tags: Open,Graph,Action,Type
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123opengraphactiontypeid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123opengraphactiontypeid125-get-openapi.md
- name: Facebook Get Open Graph Context
  x-api-slug: facebook
  description: Open Graph Context
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;open-graph-context-id&#125;
  tags: Open,Graph,Context
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123opengraphcontextid125-get-openapi.md
- name: Facebook Get Open Graph Object Type
  x-api-slug: facebook
  description: Open Graph Object Type
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;open-graph-object-type-id&#125;
  tags: Open,Graph,Object,Type
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123opengraphobjecttypeid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123opengraphobjecttypeid125-get-openapi.md
- name: Facebook Get Page Admin Note
  x-api-slug: facebook
  description: Page Admin Note
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;page-admin-note-id&#125;
  tags: Page,Admin,Note
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123pageadminnoteid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123pageadminnoteid125-get-openapi.md
- name: Facebook Get Page Call To Action
  x-api-slug: facebook
  description: Page Call To Action
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;page-call-to-action-id&#125;
  tags: Page,Call,Action
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123pagecalltoactionid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123pagecalltoactionid125-get-openapi.md
- name: Facebook Get Page Label
  x-api-slug: facebook
  description: Page Label
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;page-label-id&#125;
  tags: Page,Label
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123pagelabelid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123pagelabelid125-get-openapi.md
- name: Facebook Get Pages Platform Component Flow Service Config
  x-api-slug: facebook
  description: Pages Platform Component Flow Service Config
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;pages-platform-component-flow-service-config-id&#125;
  tags: Pages,Platform,Component,Flow,Service,Config
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123pagesplatformcomponentflowserviceconfigid125-get-openapi.md
- name: Facebook Get Payment
  x-api-slug: facebook
  description: The details of a payment made in an app using Facebook Payments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;payment-id&#125;
  tags: Payment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123paymentid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123paymentid125-get-openapi.md
- name: Facebook Post Payment Dispute
  x-api-slug: facebook
  description: Used to settle any payment disputes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;payment-id&#125;/dispute
  tags: Payment,Dispute
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123paymentid125dispute-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123paymentid125dispute-post-openapi.md
- name: Facebook Post Payment Refunds
  x-api-slug: facebook
  description: Used to issue any payment refunds.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;payment-id&#125;/refunds
  tags: Payment,Refunds
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123paymentid125refunds-post-openapi.md
- name: Facebook Get Place Tag
  x-api-slug: facebook
  description: Place Tag
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;place-tag-id&#125;
  tags: Place,Tag
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123placetagid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123placetagid125-get-openapi.md
- name: Facebook Get Place Topic
  x-api-slug: facebook
  description: Place Topic
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;place-topic-id&#125;
  tags: Place,Topic
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123placetopicid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123placetopicid125-get-openapi.md
- name: Facebook Get Post
  x-api-slug: facebook
  description: An individual entry in a profile&#039;s feed. The profile could be
    a user, page, app, or group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//post-id
  tags: Posts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/postid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/postid-get-openapi.md
- name: Facebook Delete Post
  x-api-slug: facebook
  description: An individual entry in a profile&#039;s feed. The profile could be
    a user, page, app, or group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//post-id
  tags: Posts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/postid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/postid-delete-openapi.md
- name: Facebook Add Post
  x-api-slug: facebook
  description: An individual entry in a profile&#039;s feed. The profile could be
    a user, page, app, or group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//post-id
  tags: Posts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/postid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/postid-post-openapi.md
- name: Facebook Get Add Attachments
  x-api-slug: facebook
  description: 'Media content associated with a story or comment. Story attachments
    are accessed from the following endpoints:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;post-id&#125;/attachments
  tags: Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123postid125attachments-get-openapi.md
- name: Facebook Get Promotion Info
  x-api-slug: facebook
  description: Promotion Info
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;promotion-info-id&#125;
  tags: Promotion,Info
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123promotioninfoid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123promotioninfoid125-get-openapi.md
- name: Facebook Get Rtb Dynamic Add
  x-api-slug: facebook
  description: Rtb Dynamic Post
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;rtb-dynamic-post-id&#125;
  tags: Rtb,Dynamic
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123rtbdynamicpostid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123rtbdynamicpostid125-get-openapi.md
- name: Facebook Get Request
  x-api-slug: facebook
  description: An individual game request received by someone, sent by an app or by
    another person.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;request-id&#125;
  tags: Request
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123requestid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123requestid125-get-openapi.md
- name: Facebook Delete Request
  x-api-slug: facebook
  description: An individual game request received by someone, sent by an app or by
    another person.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;request-id&#125;
  tags: Request
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123requestid125-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123requestid125-delete-openapi.md
- name: Facebook Get Sales Promo
  x-api-slug: facebook
  description: Offer
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;sales-promo-id&#125;
  tags: Sales,Promo
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123salespromoid125-get-openapi.md
- name: Facebook Get Saved Message Response
  x-api-slug: facebook
  description: Saved Message Response
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;saved-message-response-id&#125;
  tags: Saved,Message,Response
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123savedmessageresponseid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123savedmessageresponseid125-get-openapi.md
- name: Facebook Get Status
  x-api-slug: facebook
  description: A status message in a profile&#039;s feed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;status-id&#125;
  tags: Status
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123statusid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123statusid125-get-openapi.md
- name: Facebook Delete From. Status
  x-api-slug: facebook
  description: A status message in a profile&#039;s feed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;from.id&#125;_&#123;status-id&#125;
  tags: From.,Status
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123from-id125-123statusid125-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123from-id125-123statusid125-delete-openapi.md
- name: Facebook Post From. Status
  x-api-slug: facebook
  description: A status message in a profile&#039;s feed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;from.id&#125;_&#123;status-id&#125;
  tags: From.,Status
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123from-id125-123statusid125-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123from-id125-123statusid125-post-openapi.md
- name: Facebook Post Test User
  x-api-slug: facebook
  description: A test user associated with a Facebook app. Test users are created
    and associated using the /&#123;app-id&#125;/accounts/test-users edge or in the
    App Dashboard.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;test-user-id&#125;
  tags: Test,User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123testuserid125-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123testuserid125-post-openapi.md
- name: Facebook Delete Test User
  x-api-slug: facebook
  description: A test user associated with a Facebook app. Test users are created
    and associated using the /&#123;app-id&#125;/accounts/test-users edge or in the
    App Dashboard.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;test-user-id&#125;
  tags: Test,User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123testuserid125-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123testuserid125-delete-openapi.md
- name: Facebook Post Test User 1 Friends Test User 2
  x-api-slug: facebook
  description: The friends of a test user. This is identical to the /&#123;user-id&#125;/friends
    edge aside from the publishing operation explained below.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;test-user-1&#125;/friends/&#123;test-user-2&#125;
  tags: Test,User,1,Friends,Test,User,2
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123testuser1125friends123testuser2125-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123testuser1125friends123testuser2125-post-openapi.md
- name: Facebook Get Thread
  x-api-slug: facebook
  description: A Facebook Messages conversation thread. This endpoint is only accessible
    for users that are developers of the app making the request. Pages should use
    the Conversation object.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;thread-id&#125;
  tags: Thread
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123threadid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123threadid125-get-openapi.md
- name: Facebook Get User
  x-api-slug: facebook
  description: User
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;
  tags: User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125-get-openapi.md
- name: Facebook Get User Context
  x-api-slug: facebook
  description: User Context
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-context-id&#125;
  tags: User,Context
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123usercontextid125-get-openapi.md
- name: Facebook Get Veo
  x-api-slug: facebook
  description: Video
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;video-id&#125;
  tags: Veo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123videoid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123videoid125-get-openapi.md
- name: Facebook Get Veo Copyright Rule
  x-api-slug: facebook
  description: Video Copyright Rule
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;video-copyright-rule-id&#125;
  tags: Veo,Copyright,Rule
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123videocopyrightruleid125-get-openapi.md
- name: Facebook Get Veo List
  x-api-slug: facebook
  description: Video List
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;video-list-id&#125;
  tags: Veo,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123videolistid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123videolistid125-get-openapi.md
- name: Facebook Get With Asset3d
  x-api-slug: facebook
  description: With Asset3d
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;with-asset3d-id&#125;
  tags: Asset3d
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123withasset3did125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123withasset3did125-get-openapi.md
- name: Facebook Get Work Experience
  x-api-slug: facebook
  description: Work Experience
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;work-experience-id&#125;
  tags: Work,Experience
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123workexperienceid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123workexperienceid125-get-openapi.md
- name: Facebook Get App Request
  x-api-slug: facebook
  description: App Request
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;app-request-id&#125;
  tags: App,Request
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123apprequestid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123apprequestid125-get-openapi.md
- name: Facebook Get Async Session
  x-api-slug: facebook
  description: Async Session
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;async-session-id&#125;
  tags: Async,Session
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123asyncsessionid125-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123asyncsessionid125-get-openapi.md
- name: Facebook Get User Achievements
  x-api-slug: facebook
  description: User Achievements
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/achievements
  tags: User,Achievements
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125achievements-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125achievements-get-openapi.md
- name: Facebook Get User Ad Studies
  x-api-slug: facebook
  description: User Ad Studies
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/ad_studies
  tags: User,Ad,Studies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125ad-studies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125ad-studies-get-openapi.md
- name: Facebook Get User Adaccounts
  x-api-slug: facebook
  description: User Adaccounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/adaccounts
  tags: User,Adaccounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125adaccounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125adaccounts-get-openapi.md
- name: Facebook Get User Adcontracts
  x-api-slug: facebook
  description: User Adcontracts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/adcontracts
  tags: User,Adcontracts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125adcontracts-get-openapi.md
- name: Facebook Get User Adnetworkanalytics
  x-api-slug: facebook
  description: User Adnetworkanalytics
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/adnetworkanalytics
  tags: User,Adnetworkanalytics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125adnetworkanalytics-get-openapi.md
- name: Facebook Get User Albums
  x-api-slug: facebook
  description: User Albums
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/albums
  tags: User,Albums
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125albums-get-openapi.md
- name: Facebook Get User Apprequestformerrecipients
  x-api-slug: facebook
  description: User Apprequestformerrecipients
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/apprequestformerrecipients
  tags: User,Apprequestformerrecipients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125apprequestformerrecipients-get-openapi.md
- name: Facebook Get User Apprequests
  x-api-slug: facebook
  description: User Apprequests
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/apprequests
  tags: User,Apprequests
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125apprequests-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125apprequests-get-openapi.md
- name: Facebook Get User Asset3ds
  x-api-slug: facebook
  description: User Asset3ds
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/asset3ds
  tags: User,Asset3ds
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125asset3ds-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125asset3ds-get-openapi.md
- name: Facebook Get User Assigned Ad Accounts
  x-api-slug: facebook
  description: User Assigned Ad Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/assigned_ad_accounts
  tags: User,Assigned,Ad,Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125assigned-ad-accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125assigned-ad-accounts-get-openapi.md
- name: Facebook Get User Assigned Monetization Properties
  x-api-slug: facebook
  description: User Assigned Monetization Properties
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/assigned_monetization_properties
  tags: User,Assigned,Monetization,Properties
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125assigned-monetization-properties-get-openapi.md
- name: Facebook Get User Assigned Pages
  x-api-slug: facebook
  description: User Assigned Pages
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/assigned_pages
  tags: User,Assigned,Pages
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125assigned-pages-get-openapi.md
- name: Facebook Get User Assigned Product Catalogs
  x-api-slug: facebook
  description: User Assigned Product Catalogs
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/assigned_product_catalogs
  tags: User,Assigned,Product,Catalogs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125assigned-product-catalogs-get-openapi.md
- name: Facebook Get User Books
  x-api-slug: facebook
  description: User Books
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/books
  tags: User,Books
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125books-get-openapi.md
- name: Facebook Get User Business Activities
  x-api-slug: facebook
  description: User Business Activities
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/business_activities
  tags: User,Business,Activities
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125business-activities-get-openapi.md
- name: Facebook Get User Businesses
  x-api-slug: facebook
  description: User Businesses
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/businesses
  tags: User,Businesses
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125businesses-get-openapi.md
- name: Facebook Get User Conversations
  x-api-slug: facebook
  description: User Conversations
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/conversations
  tags: User,Conversations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125conversations-get-openapi.md
- name: Facebook Get User Custom Labels
  x-api-slug: facebook
  description: User Custom Labels
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/custom_labels
  tags: User,Custom,Labels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125custom-labels-get-openapi.md
- name: Facebook Get User Domains
  x-api-slug: facebook
  description: User Domains
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/domains
  tags: User,Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125domains-get-openapi.md
- name: Facebook Get User Events
  x-api-slug: facebook
  description: User Events
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/events
  tags: User,Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125events-get-openapi.md
- name: Facebook Get User Family
  x-api-slug: facebook
  description: User Family
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/family
  tags: User,Family
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125family-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125family-get-openapi.md
- name: Facebook Get User Favorite Requests
  x-api-slug: facebook
  description: User Favorite Requests
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/favorite_requests
  tags: User,Favorite,Requests
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125favorite-requests-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125favorite-requests-get-openapi.md
- name: Facebook Get Me Feed
  x-api-slug: facebook
  description: 'The feed of posts (including status updates) and links published by
    this person, or by others on this person&#039;s profile. There are other edges
    which provide filtered versions of this edge:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//me/feed
  tags: Me,Feed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mefeed-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mefeed-get-openapi.md
- name: Facebook Post Me Feed
  x-api-slug: facebook
  description: 'The feed of posts (including status updates) and links published by
    this person, or by others on this person&#039;s profile. There are other edges
    which provide filtered versions of this edge:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//me/feed
  tags: Me,Feed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mefeed-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mefeed-post-openapi.md
- name: Facebook Get User Friendlists
  x-api-slug: facebook
  description: User Friendlists
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/friendlists
  tags: User,Friendlists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125friendlists-get-openapi.md
- name: Facebook Get Me Friendrequests
  x-api-slug: facebook
  description: A person&#039;s pending friend requests.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//me/friendrequests
  tags: Me,Friendrequests
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mefriendrequests-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mefriendrequests-get-openapi.md
- name: Facebook Get User Games
  x-api-slug: facebook
  description: User Games
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/games
  tags: User,Games
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125games-get-openapi.md
- name: Facebook Get User Groups
  x-api-slug: facebook
  description: User Groups
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/groups
  tags: User,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125groups-get-openapi.md
- name: Facebook Get Me Home
  x-api-slug: facebook
  description: As of October 6th, 2015, this endpoint is no longer available.  Please
    consider using the /user-id/feed edge instead.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//me/home
  tags: Me,Home
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mehome-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mehome-get-openapi.md
- name: Facebook Get User S For Apps
  x-api-slug: facebook
  description: User Ids For Apps
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/ids_for_apps
  tags: User,S,Apps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125ids-for-apps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125ids-for-apps-get-openapi.md
- name: Facebook Get User S For Business
  x-api-slug: facebook
  description: User IDs for Business
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/ids_for_business
  tags: User,S,Business
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125ids-for-business-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125ids-for-business-get-openapi.md
- name: Facebook Get User S For Pages
  x-api-slug: facebook
  description: User Ids For Pages
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/ids_for_pages
  tags: User,S,Pages
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125ids-for-pages-get-openapi.md
- name: Facebook Get Me Inbox
  x-api-slug: facebook
  description: A person&#039;s Facebook Messages inbox.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//me/inbox
  tags: Me,Inbox
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/meinbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/meinbox-get-openapi.md
- name: Facebook Get User Invitable Friends
  x-api-slug: facebook
  description: User Invitable Friends
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/invitable_friends
  tags: User,Invitable,Friends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125invitable-friends-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125invitable-friends-get-openapi.md
- name: Facebook Get User Leadgen Forms
  x-api-slug: facebook
  description: User Leadgen Forms
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/leadgen_forms
  tags: User,Leadgen,Forms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125leadgen-forms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125leadgen-forms-get-openapi.md
- name: Facebook Get User Live Veos
  x-api-slug: facebook
  description: User Live Videos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/live_videos
  tags: User,Live,Veos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125live-videos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125live-videos-get-openapi.md
- name: Facebook Get Me Locations
  x-api-slug: facebook
  description: A feed of posts and photos that include location information and in
    which this person has been tagged. This is useful for constructing a chronology
    of places that the person has visited.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//me/locations
  tags: Me,Locations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/melocations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/melocations-get-openapi.md
- name: Facebook Get User Movies
  x-api-slug: facebook
  description: User Movies
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/movies
  tags: User,Movies
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125movies-get-openapi.md
- name: Facebook Get User Music
  x-api-slug: facebook
  description: User Music
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/music
  tags: User,Music
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125music-get-openapi.md
- name: Facebook Get Me Outbox
  x-api-slug: facebook
  description: Items in a person&#039;s Facebook Messages outbox.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//me/outbox
  tags: Me,Outbox
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/meoutbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/meoutbox-get-openapi.md
- name: Facebook Get User Permissions
  x-api-slug: facebook
  description: User Permissions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/permissions
  tags: User,Permissions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125permissions-get-openapi.md
- name: Facebook Get User Personal Ad Accounts
  x-api-slug: facebook
  description: User Personal Ad Accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/personal_ad_accounts
  tags: User,Personal,Ad,Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125personal-ad-accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125personal-ad-accounts-get-openapi.md
- name: Facebook Get User Photos
  x-api-slug: facebook
  description: User Photos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/photos
  tags: User,Photos
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125photos-get-openapi.md
- name: Facebook Get User Picture
  x-api-slug: facebook
  description: User Picture
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/picture
  tags: User,Picture
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125picture-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125picture-get-openapi.md
- name: Facebook Get User Promotable Domains
  x-api-slug: facebook
  description: User Promotable Domains
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/promotable_domains
  tags: User,Promotable,Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125promotable-domains-get-openapi.md
- name: Facebook Get User Promotable Events
  x-api-slug: facebook
  description: User Promotable Events
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/promotable_events
  tags: User,Promotable,Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125promotable-events-get-openapi.md
- name: Facebook Get User Request History
  x-api-slug: facebook
  description: User Request History
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/request_history
  tags: User,Request,History
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125request-history-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125request-history-get-openapi.md
- name: Facebook Get User Rich Media Documents
  x-api-slug: facebook
  description: User Rich Media Documents
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/rich_media_documents
  tags: User,Rich,Media,Documents
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125rich-media-documents-get-openapi.md
- name: Facebook Get Me Scores
  x-api-slug: facebook
  description: As of April 4, 2018, this endpoint only returns an empty data set.
    Please see the changelog for more information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//me/scores
  tags: Me,Scores
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mescores-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mescores-get-openapi.md
- name: Facebook Post Me Scores
  x-api-slug: facebook
  description: As of April 4, 2018, this endpoint only returns an empty data set.
    Please see the changelog for more information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//me/scores
  tags: Me,Scores
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mescores-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mescores-post-openapi.md
- name: Facebook Delete Me Scores
  x-api-slug: facebook
  description: As of April 4, 2018, this endpoint only returns an empty data set.
    Please see the changelog for more information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//me/scores
  tags: Me,Scores
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mescores-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/mescores-delete-openapi.md
- name: Facebook Get User Session Keys
  x-api-slug: facebook
  description: User Session Keys
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/session_keys
  tags: User,Session,Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125session-keys-get-openapi.md
- name: Facebook Get User Stream Filters
  x-api-slug: facebook
  description: User Stream Filters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/stream_filters
  tags: User,Stream,Filters
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125stream-filters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125stream-filters-get-openapi.md
- name: Facebook Get User Taggable Friends
  x-api-slug: facebook
  description: User Taggable Friends
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/taggable_friends
  tags: User,Taggable,Friends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125taggable-friends-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125taggable-friends-get-openapi.md
- name: Facebook Get User Tagged Places
  x-api-slug: facebook
  description: User Tagged Places
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/tagged_places
  tags: User,Tagged,Places
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125tagged-places-get-openapi.md
- name: Facebook Get User Television
  x-api-slug: facebook
  description: User Television
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/television
  tags: User,Television
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125television-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125television-get-openapi.md
- name: Facebook Get User Threads
  x-api-slug: facebook
  description: User Threads
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/threads
  tags: User,Threads
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125threads-get-openapi.md
- name: Facebook Get User Veo Broadcasts
  x-api-slug: facebook
  description: User Video Broadcasts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0//&#123;user-id&#125;/video_broadcasts
  tags: User,Veo,Broadcasts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/123userid125video-broadcasts-get-openapi.md
- name: Facebook
  x-api-slug: facebook
  description: Create an account or log into Facebook. Connect with friends, family
    and other people you know. Share photos and videos, send messages and get updates.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: https://facebook.com
  baseURL: https://graph.facebook.com//v3.0
  tags: Facebook
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/facebook/master/_listings/facebook/openapi.md
x-common:
- type: x-android-sdk
  url: https://developers.facebook.com/docs/android/share
- type: x-apigee-console
  url: https://api.apigee.com/v1/consoles/facebook/apidescription?format=internal&ver=1386216190000
- type: x-application-gallery
  url: https://developers.facebook.com/docs/showcase/
- type: x-base
  url: https://graph.facebook.com
- type: x-best-practices
  url: https://developers.facebook.com/docs/sharing/best-practices
- type: x-blog
  url: http://blog.facebook.com
- type: x-blog-rss
  url: https://www.facebook.com/business/news/rss/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/facebook
- type: x-crunchbase
  url: https://crunchbase.com/organization/facebook
- type: x-developer
  url: https://developers.facebook.com/
- type: x-forum
  url: https://www.facebook.com/groups/fbdevelopers
- type: x-github
  url: https://github.com/facebook
- type: x-ios-sdk
  url: https://developers.facebook.com/docs/ios/share
- type: x-issues
  url: https://developers.facebook.com/status/issues/
- type: x-javascript-library
  url: https://developers.facebook.com/docs/reference/javascript/
- type: x-partners
  url: https://facebookmarketingpartners.com/
- type: x-php-sdk
  url: https://developers.facebook.com/docs/reference/php/
- type: x-plugins
  url: https://developers.facebook.com/docs/plugins/
- type: x-privacy
  url: https://www.facebook.com/settings?tab=privacy
- type: x-road-map
  url: https://developers.facebook.com/docs/apps/migrations
- type: x-status
  url: https://developers.facebook.com/status/
- type: x-terms-of-service
  url: https://www.facebook.com/terms
- type: x-terms-of-service
  url: https://developers.facebook.com/policy
- type: x-transparency-report
  url: https://www.facebook.com/about/government_requests
- type: x-twitter
  url: https://twitter.com/facebook
- type: x-website
  url: https://facebook.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---