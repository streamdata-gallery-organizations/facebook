---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Post User Statuses
  description: Posts a status message on the user
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    get:
      summary: Get Search
      description: Search over all public objects in the social graph
      operationId: getSearch
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: q
        description: The search string
      - in: query
        name: type
        description: 'Supports these types of objects: All public posts (post), people
          (user), pages (page), events                                                        (event),
          groups (group), check-ins (checkin)'
      responses:
        200:
          description: OK
      tags:
      - Search
  /{album}:
    get:
      summary: Get Album
      description: A photo album
      operationId: getAlbum
      x-api-path-slug: album-get
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      responses:
        200:
          description: OK
      tags:
      - Album
  /{album}/photos:
    get:
      summary: Get Album Photos
      description: The photos contained in this album
      operationId: getAlbumPhotos
      x-api-path-slug: albumphotos-get
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      responses:
        200:
          description: OK
      tags:
      - Album
      - Photos
    post:
      summary: Post Album Photos
      description: Adds a photo to the album
      operationId: postAlbumPhotos
      x-api-path-slug: albumphotos-post
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      - in: query
        name: message
        description: Photo description
      responses:
        200:
          description: OK
      tags:
      - Album
      - Photos
  /{album}/likes:
    get:
      summary: Get Album Likes
      description: The likes made on this album
      operationId: getAlbumLikes
      x-api-path-slug: albumlikes-get
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      responses:
        200:
          description: OK
      tags:
      - Album
      - Likes
    post:
      summary: Post Album Likes
      description: Likes the album
      operationId: postAlbumLikes
      x-api-path-slug: albumlikes-post
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      responses:
        200:
          description: OK
      tags:
      - Album
      - Likes
    delete:
      summary: Delete Album Likes
      description: Unlikes the album
      operationId: deleteAlbumLikes
      x-api-path-slug: albumlikes-delete
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      responses:
        200:
          description: OK
      tags:
      - Album
      - Likes
  /{album}/comments:
    get:
      summary: Get Album Comments
      description: The comments made on this album
      operationId: getAlbumComments
      x-api-path-slug: albumcomments-get
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      responses:
        200:
          description: OK
      tags:
      - Album
      - Comments
    post:
      summary: Post Album Comments
      description: Posts a comment on the album
      operationId: postAlbumComments
      x-api-path-slug: albumcomments-post
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      - in: query
        name: message
        description: Comment text
      responses:
        200:
          description: OK
      tags:
      - Album
      - Comments
  /{album}/picture:
    get:
      summary: Get Album Picture
      description: The album's cover photo; the first picture uploaded to an album
        becomes the cover photo for the album.
      operationId: getAlbumPicture
      x-api-path-slug: albumpicture-get
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      - in: query
        name: type
        description: One of square (50x50), small (50 pixels wide, variable height),
          and large (about 200 pixels wide,                                                        variable
          height)
      responses:
        200:
          description: OK
      tags:
      - Album
      - Picture
  /{application}:
    get:
      summary: Get Application
      description: An application's profile
      operationId: getApplication
      x-api-path-slug: application-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
  /{application}/accounts:
    get:
      summary: Get Application Accounts
      description: Test User accounts associated with the application.
      operationId: getApplicationAccounts
      x-api-path-slug: applicationaccounts-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Accounts
  /{application}/accounts/test-users:
    post:
      summary: Post Application Accounts Test Users
      description: Creates a test account for the application
      operationId: postApplicationAccountsTestUsers
      x-api-path-slug: applicationaccountstestusers-post
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: installed
        description: Install app for the test user upon creation
      - in: query
        name: name
        description: A name for the test user
      - in: query
        name: permissions
        description: List of extended permissions app granted for the new test user
          if installed is true
      responses:
        200:
          description: OK
      tags:
      - Application
      - Accounts
      - Test
      - Users
  /{application}/albums:
    get:
      summary: Get Application Albums
      description: The photo albums this application has created.
      operationId: getApplicationAlbums
      x-api-path-slug: applicationalbums-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Albums
  /{application}/feed:
    get:
      summary: Get Application Feed
      description: The application's wall.
      operationId: getApplicationFeed
      x-api-path-slug: applicationfeed-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Feed
    post:
      summary: Post Application Feed
      description: Posts a status message on the application's profile page
      operationId: postApplicationFeed
      x-api-path-slug: applicationfeed-post
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: message
        description: Status Message content
      responses:
        200:
          description: OK
      tags:
      - Application
      - Feed
  /{application}/insights:
    get:
      summary: Get Application Insights
      description: Usage metrics for this application
      operationId: getApplicationInsights
      x-api-path-slug: applicationinsights-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Insights
  /{application}/links:
    get:
      summary: Get Application Links
      description: The application's posted links.
      operationId: getApplicationLinks
      x-api-path-slug: applicationlinks-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Links
    post:
      summary: Post Application Links
      description: Posts a link on the application's profile page
      operationId: postApplicationLinks
      x-api-path-slug: applicationlinks-post
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: link
        description: Link URL
      - in: query
        name: message
        description: Link message
      responses:
        200:
          description: OK
      tags:
      - Application
      - Links
  /{application}/picture:
    get:
      summary: Get Application Picture
      description: The application's logo
      operationId: getApplicationPicture
      x-api-path-slug: applicationpicture-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: type
        description: One of square (50x50), small (50 pixels wide, variable height),
          and large (about 200 pixels wide,                                                        variable
          height)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Picture
  /{application}/posts:
    get:
      summary: Get Application Adds
      description: The application's own posts.
      operationId: getApplicationAdds
      x-api-path-slug: applicationposts-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Posts
  /{application}/reviews:
    get:
      summary: Get Application Reviews
      description: Reviews of this application
      operationId: getApplicationReviews
      x-api-path-slug: applicationreviews-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Reviews
  /{application}/staticresources:
    get:
      summary: Get Application Staticresources
      description: Usage stats about the canvas application's static resources, such
        as javascript and CSS, and which ones are being flushed to browsers early.
      operationId: getApplicationStaticresources
      x-api-path-slug: applicationstaticresources-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Staticresources
  /{application}/statuses:
    get:
      summary: Get Application Statuses
      description: The application's status updates
      operationId: getApplicationStatuses
      x-api-path-slug: applicationstatuses-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Statuses
    post:
      summary: Post Application Statuses
      description: Posts a status message on the application's profile page
      operationId: postApplicationStatuses
      x-api-path-slug: applicationstatuses-post
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: message
        description: Status Message content
      responses:
        200:
          description: OK
      tags:
      - Application
      - Statuses
  /{application}/subscriptions:
    get:
      summary: Get Application Subscriptions
      description: All of the subscriptions this application has for real-time notifications.
      operationId: getApplicationSubscriptions
      x-api-path-slug: applicationsubscriptions-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Subscriptions
    post:
      summary: Post Application Subscriptions
      description: Adds a real-time notification subscription for this application.
      operationId: postApplicationSubscriptions
      x-api-path-slug: applicationsubscriptions-post
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: callback_url
        description: A callback URL to which Facebook will post subscription updates
      - in: query
        name: fields
        description: List of properties for the `object` to monitor
      - in: query
        name: object
        description: Object to monitor - `user`, `permissions`, or `page`
      - in: query
        name: verify_token
        description: Token sent in the verification request
      responses:
        200:
          description: OK
      tags:
      - Application
      - Subscriptions
    delete:
      summary: Delete Application Subscriptions
      description: Deletes a real-time notification subscription for this application.
      operationId: deleteApplicationSubscriptions
      x-api-path-slug: applicationsubscriptions-delete
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: object
        description: Object to monitor - `user`, `permissions`, or `page`
      responses:
        200:
          description: OK
      tags:
      - Application
      - Subscriptions
  /{application}/tagged:
    get:
      summary: Get Application Tagged
      description: The photos, videos, and posts in which this application has been
        tagged.
      operationId: getApplicationTagged
      x-api-path-slug: applicationtagged-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Tagged
  /{application}/translations:
    get:
      summary: Get Application Translations
      description: The translated strings for this application.
      operationId: getApplicationTranslations
      x-api-path-slug: applicationtranslations-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Translations
    post:
      summary: Post Application Translations
      description: Uploads translated strings for this application.
      operationId: postApplicationTranslations
      x-api-path-slug: applicationtranslations-post
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: native_strings
        description: A JSON-encoded array of strings to translate
      responses:
        200:
          description: OK
      tags:
      - Application
      - Translations
    delete:
      summary: Delete Application Translations
      description: Deletes a translation string for this application.
      operationId: deleteApplicationTranslations
      x-api-path-slug: applicationtranslations-delete
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: native_hashes
        description: An array of native hashes
      responses:
        200:
          description: OK
      tags:
      - Application
      - Translations
  /{application}/scores:
    get:
      summary: Get Application Scores
      description: Scores for the user and their friends.
      operationId: getApplicationScores
      x-api-path-slug: applicationscores-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Scores
    delete:
      summary: Delete Application Scores
      description: Deletes all the scores for the application.
      operationId: deleteApplicationScores
      x-api-path-slug: applicationscores-delete
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Scores
  /{application}/achievements:
    post:
      summary: Post Application Achievements
      description: Registers an achievement for the application
      operationId: postApplicationAchievements
      x-api-path-slug: applicationachievements-post
      parameters:
      - in: query
        name: achievement
        description: Unique URL to the achievement
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: display_order
        description: Order of this achievement as it shows up in the achievement stories
          UI (low to high)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Achievements
    delete:
      summary: Delete Application Achievements
      description: Unregisters an achievement for the application
      operationId: deleteApplicationAchievements
      x-api-path-slug: applicationachievements-delete
      parameters:
      - in: query
        name: achievement
        description: Unique URL to the achievement
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Achievements
  /{checkin}:
    get:
      summary: Get Checkin
      description: Represents a single visit by a user to a location
      operationId: getCheckin
      x-api-path-slug: checkin-get
      parameters:
      - in: path
        name: checkin
        description: Represents the ID of the checkin object
      responses:
        200:
          description: OK
      tags:
      - Checkin
  /{checkin}/comments:
    get:
      summary: Get Checkin Comments
      description: All of the comments on this checkin.
      operationId: getCheckinComments
      x-api-path-slug: checkincomments-get
      parameters:
      - in: path
        name: checkin
        description: Represents the ID of the checkin object
      responses:
        200:
          description: OK
      tags:
      - Checkin
      - Comments
    post:
      summary: Post Checkin Comments
      description: Posts a comment to this checkin.
      operationId: postCheckinComments
      x-api-path-slug: checkincomments-post
      parameters:
      - in: path
        name: checkin
        description: Represents the ID of the checkin object
      - in: query
        name: message
        description: Comment text
      responses:
        200:
          description: OK
      tags:
      - Checkin
      - Comments
  /{checkin}/likes:
    get:
      summary: Get Checkin Likes
      description: Users who like this checkin.
      operationId: getCheckinLikes
      x-api-path-slug: checkinlikes-get
      parameters:
      - in: path
        name: checkin
        description: Represents the ID of the checkin object
      responses:
        200:
          description: OK
      tags:
      - Checkin
      - Likes
    post:
      summary: Post Checkin Likes
      description: Likes this checkin.
      operationId: postCheckinLikes
      x-api-path-slug: checkinlikes-post
      parameters:
      - in: path
        name: checkin
        description: Represents the ID of the checkin object
      responses:
        200:
          description: OK
      tags:
      - Checkin
      - Likes
    delete:
      summary: Delete Checkin Likes
      description: Unlikes this checkin.
      operationId: deleteCheckinLikes
      x-api-path-slug: checkinlikes-delete
      parameters:
      - in: path
        name: checkin
        description: Represents the ID of the checkin object
      responses:
        200:
          description: OK
      tags:
      - Checkin
      - Likes
  /{comment}:
    get:
      summary: Get Comment
      description: Returns a comment
      operationId: getComment
      x-api-path-slug: comment-get
      parameters:
      - in: path
        name: comment
        description: Represents the ID of the comment object
      responses:
        200:
          description: OK
      tags:
      - Comment
    delete:
      summary: Delete Comment
      description: Deletes a comment
      operationId: deleteComment
      x-api-path-slug: comment-delete
      parameters:
      - in: path
        name: comment
        description: Represents the ID of the comment object
      responses:
        200:
          description: OK
      tags:
      - Comment
  /{comment}/likes:
    get:
      summary: Get Comment Likes
      description: All the likes on this comment
      operationId: getCommentLikes
      x-api-path-slug: commentlikes-get
      parameters:
      - in: path
        name: comment
        description: Represents the ID of the comment object
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Likes
    post:
      summary: Post Comment Likes
      description: Likes the comment
      operationId: postCommentLikes
      x-api-path-slug: commentlikes-post
      parameters:
      - in: path
        name: comment
        description: Represents the ID of the comment object
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Likes
    delete:
      summary: Delete Comment Likes
      description: Unlikes the comment
      operationId: deleteCommentLikes
      x-api-path-slug: commentlikes-delete
      parameters:
      - in: path
        name: comment
        description: Represents the ID of the comment object
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Likes
  /{event}:
    get:
      summary: Get Event
      description: Specifies information about an event, including the location, event
        name, and which invitees plan to attend.
      operationId: getEvent
      x-api-path-slug: event-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
  /{event}/feed:
    get:
      summary: Get Event Feed
      description: This event's wall
      operationId: getEventFeed
      x-api-path-slug: eventfeed-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Feed
    post:
      summary: Post Event Feed
      description: Posts a status message on this event's wall
      operationId: postEventFeed
      x-api-path-slug: eventfeed-post
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      - in: query
        name: message
        description: Status Message content
      responses:
        200:
          description: OK
      tags:
      - Event
      - Feed
  /{event}/noreply:
    get:
      summary: Get Event Noreply
      description: All of the users who have been not yet responded to their invitation
        to this event
      operationId: getEventNoreply
      x-api-path-slug: eventnoreply-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Noreply
  /{event}/maybe:
    get:
      summary: Get Event Maybe
      description: All of the users who have been responded "Maybe" to their invitation
        to this event
      operationId: getEventMaybe
      x-api-path-slug: eventmaybe-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Maybe
    post:
      summary: Post Event Maybe
      description: RSVPs the user as a 'maybe' for the event
      operationId: postEventMaybe
      x-api-path-slug: eventmaybe-post
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Maybe
  /{event}/invited:
    get:
      summary: Get Event Invited
      description: All of the users who have been invited to this event
      operationId: getEventInvited
      x-api-path-slug: eventinvited-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Invited
  /{event}/attending:
    get:
      summary: Get Event Attending
      description: All of the users who are attending this event
      operationId: getEventAttending
      x-api-path-slug: eventattending-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Attending
    post:
      summary: Post Event Attending
      description: RSVPs the user as 'attending' for the event
      operationId: postEventAttending
      x-api-path-slug: eventattending-post
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Attending
  /{event}/declined:
    get:
      summary: Get Event Declined
      description: All of the users who declined their invitation to this event
      operationId: getEventDeclined
      x-api-path-slug: eventdeclined-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Declined
    post:
      summary: Post Event Declined
      description: RSVPs the user as 'declined' for the event
      operationId: postEventDeclined
      x-api-path-slug: eventdeclined-post
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Declined
  /{event}/picture:
    get:
      summary: Get Event Picture
      description: The event's profile picture
      operationId: getEventPicture
      x-api-path-slug: eventpicture-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      - in: query
        name: type
        description: One of square (50x50), small (50 pixels wide, variable height),
          and large (about 200 pixels wide,                                                        variable
          height)
      responses:
        200:
          description: OK
      tags:
      - Event
      - Picture
  /{friendlist}:
    get:
      summary: Get Friendlist
      description: A Facebook friend list. This object represents the list itself
        and not the members of the list.
      operationId: getFriendlist
      x-api-path-slug: friendlist-get
      parameters:
      - in: path
        name: friendlist
        description: Represents the ID of the FriendList object
      responses:
        200:
          description: OK
      tags:
      - Friendlist
    delete:
      summary: Delete Friendlist
      description: Deletes the FriendList.
      operationId: deleteFriendlist
      x-api-path-slug: friendlist-delete
      parameters:
      - in: path
        name: friendlist
        description: Represents the ID of the FriendList object
      responses:
        200:
          description: OK
      tags:
      - Friendlist
  /{friendlist}/members:
    get:
      summary: Get Friendlist Members
      description: All of the users who are members of this list.
      operationId: getFriendlistMembers
      x-api-path-slug: friendlistmembers-get
      parameters:
      - in: path
        name: friendlist
        description: Represents the ID of the FriendList object
      responses:
        200:
          description: OK
      tags:
      - Friendlist
      - Members
  /{friendlist}/members/{user}:
    post:
      summary: Post Friendlist Members User
      description: Adds a user to the friend list
      operationId: postFriendlistMembersUser
      x-api-path-slug: friendlistmembersuser-post
      parameters:
      - in: path
        name: friendlist
        description: Represents the ID of the FriendList object
      - in: path
        name: user
        description: Represents the ID of the User to add to or remove from the friend
          list
      responses:
        200:
          description: OK
      tags:
      - Friendlist
      - Members
      - User
    delete:
      summary: Delete Friendlist Members User
      description: Removes a user from the friend list
      operationId: deleteFriendlistMembersUser
      x-api-path-slug: friendlistmembersuser-delete
      parameters:
      - in: path
        name: friendlist
        description: Represents the ID of the FriendList object
      - in: path
        name: user
        description: Represents the ID of the User to add to or remove from the friend
          list
      responses:
        200:
          description: OK
      tags:
      - Friendlist
      - Members
      - User
  /{group}:
    get:
      summary: Get Group
      description: A Facebook group
      operationId: getGroup
      x-api-path-slug: group-get
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      responses:
        200:
          description: OK
      tags:
      - Group
  /{group}/feed:
    get:
      summary: Get Group Feed
      description: This group's wall
      operationId: getGroupFeed
      x-api-path-slug: groupfeed-get
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      responses:
        200:
          description: OK
      tags:
      - Group
      - Feed
    post:
      summary: Post Group Feed
      description: Posts a status message on this group's wall
      operationId: postGroupFeed
      x-api-path-slug: groupfeed-post
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      - in: query
        name: message
        description: Status Message content
      responses:
        200:
          description: OK
      tags:
      - Group
      - Feed
  /{group}/members:
    get:
      summary: Get Group Members
      description: All of the users who are members of this group
      operationId: getGroupMembers
      x-api-path-slug: groupmembers-get
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      responses:
        200:
          description: OK
      tags:
      - Group
      - Members
  /{group}/picture:
    get:
      summary: Get Group Picture
      description: The profile picture of this group
      operationId: getGroupPicture
      x-api-path-slug: grouppicture-get
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      - in: query
        name: type
        description: One of square (50x50), small (50 pixels wide, variable height),
          and large (about 200 pixels wide,                                                        variable
          height)
      responses:
        200:
          description: OK
      tags:
      - Group
      - Picture
  /{group}/docs:
    get:
      summary: Get Group Docs
      description: The docs in this group
      operationId: getGroupDocs
      x-api-path-slug: groupdocs-get
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      responses:
        200:
          description: OK
      tags:
      - Group
      - Docs
  /{link}:
    get:
      summary: Get Link
      description: A link shared on a user's wall
      operationId: getLink
      x-api-path-slug: link-get
      parameters:
      - in: path
        name: link
        description: Represents the ID of the link object
      responses:
        200:
          description: OK
      tags:
      - Link
  /{link}/comments:
    get:
      summary: Get Link Comments
      description: All of the comments on this link.
      operationId: getLinkComments
      x-api-path-slug: linkcomments-get
      parameters:
      - in: path
        name: link
        description: Represents the ID of the link object
      responses:
        200:
          description: OK
      tags:
      - Link
      - Comments
    post:
      summary: Post Link Comments
      description: Posts a comment to this link.
      operationId: postLinkComments
      x-api-path-slug: linkcomments-post
      parameters:
      - in: path
        name: link
        description: Represents the ID of the link object
      - in: query
        name: message
        description: Comment text
      responses:
        200:
          description: OK
      tags:
      - Link
      - Comments
  /{link}/likes:
    get:
      summary: Get Link Likes
      description: Users who like this link.
      operationId: getLinkLikes
      x-api-path-slug: linklikes-get
      parameters:
      - in: path
        name: link
        description: Represents the ID of the link object
      responses:
        200:
          description: OK
      tags:
      - Link
      - Likes
    post:
      summary: Post Link Likes
      description: Likes this link.
      operationId: postLinkLikes
      x-api-path-slug: linklikes-post
      parameters:
      - in: path
        name: link
        description: Represents the ID of the link object
      responses:
        200:
          description: OK
      tags:
      - Link
      - Likes
    delete:
      summary: Delete Link Likes
      description: Unlikes this link.
      operationId: deleteLinkLikes
      x-api-path-slug: linklikes-delete
      parameters:
      - in: path
        name: link
        description: Represents the ID of the link object
      responses:
        200:
          description: OK
      tags:
      - Link
      - Likes
  /{note}:
    get:
      summary: Get Note
      description: A Facebook note
      operationId: getNote
      x-api-path-slug: note-get
      parameters:
      - in: path
        name: note
        description: Represents the ID of the note object
      responses:
        200:
          description: OK
      tags:
      - Note
  /{note}/comments:
    get:
      summary: Get Note Comments
      description: All of the comments on this note.
      operationId: getNoteComments
      x-api-path-slug: notecomments-get
      parameters:
      - in: path
        name: note
        description: Represents the ID of the note object
      responses:
        200:
          description: OK
      tags:
      - Note
      - Comments
    post:
      summary: Post Note Comments
      description: Posts a comment to this note.
      operationId: postNoteComments
      x-api-path-slug: notecomments-post
      parameters:
      - in: query
        name: message
        description: Comment text
      - in: path
        name: note
        description: Represents the ID of the note object
      responses:
        200:
          description: OK
      tags:
      - Note
      - Comments
  /{note}/likes:
    get:
      summary: Get Note Likes
      description: Users who like this note.
      operationId: getNoteLikes
      x-api-path-slug: notelikes-get
      parameters:
      - in: path
        name: note
        description: Represents the ID of the note object
      responses:
        200:
          description: OK
      tags:
      - Note
      - Likes
    post:
      summary: Post Note Likes
      description: Likes this note.
      operationId: postNoteLikes
      x-api-path-slug: notelikes-post
      parameters:
      - in: path
        name: note
        description: Represents the ID of the note object
      responses:
        200:
          description: OK
      tags:
      - Note
      - Likes
    delete:
      summary: Delete Note Likes
      description: Unlikes this note.
      operationId: deleteNoteLikes
      x-api-path-slug: notelikes-delete
      parameters:
      - in: path
        name: note
        description: Represents the ID of the note object
      responses:
        200:
          description: OK
      tags:
      - Note
      - Likes
  /{page}:
    get:
      summary: Get Page
      description: Returns a Page
      operationId: getPage
      x-api-path-slug: page-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
  /{page}/feed:
    get:
      summary: Get Page Feed
      description: This page's wall
      operationId: getPageFeed
      x-api-path-slug: pagefeed-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Feed
    post:
      summary: Post Page Feed
      description: Posts a status message on this page's wall
      operationId: postPageFeed
      x-api-path-slug: pagefeed-post
      parameters:
      - in: query
        name: message
        description: Status Message content
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Feed
  /{page}/picture:
    get:
      summary: Get Page Picture
      description: The page's profile picture
      operationId: getPagePicture
      x-api-path-slug: pagepicture-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: type
        description: One of square (50x50), small (50 pixels wide, variable height),
          and large (about 200 pixels wide,                                                        variable
          height)
      responses:
        200:
          description: OK
      tags:
      - Page
      - Picture
  /{page}/settings:
    get:
      summary: Get Page Settings
      description: The page's post permission settings
      operationId: getPageSettings
      x-api-path-slug: pagesettings-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Settings
    post:
      summary: Post Page Settings
      description: The page's post permission settings
      operationId: postPageSettings
      x-api-path-slug: pagesettings-post
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: setting
        description: 'Which single setting to update: USERS_CAN_POST, USERS_CAN_POST_PHOTOS,
          USERS_CAN_TAG_PHOTOS, USERS_CAN_POST_VIDEOS'
      - in: query
        name: value
        description: Connect to the social network with the Graph API
      responses:
        200:
          description: OK
      tags:
      - Page
      - Settings
  /{page}/tagged:
    get:
      summary: Get Page Tagged
      description: The photos, videos, and posts in which this page has been tagged
      operationId: getPageTagged
      x-api-path-slug: pagetagged-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Tagged
  /{page}/links:
    get:
      summary: Get Page Links
      description: The page's posted links
      operationId: getPageLinks
      x-api-path-slug: pagelinks-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Links
    post:
      summary: Post Page Links
      description: Posts a link on the page
      operationId: postPageLinks
      x-api-path-slug: pagelinks-post
      parameters:
      - in: query
        name: link
        description: Link URL
      - in: query
        name: message
        description: Link message
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Links
  /{page}/photos:
    get:
      summary: Get Page Photos
      description: The photos contained on this page
      operationId: getPagePhotos
      x-api-path-slug: pagephotos-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Photos
    post:
      summary: Post Page Photos
      description: Adds a photo to the page
      operationId: postPagePhotos
      x-api-path-slug: pagephotos-post
      parameters:
      - in: query
        name: message
        description: Photo description
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Photos
  /{page}/groups:
    get:
      summary: Get Page Groups
      description: The groups this page is a member of
      operationId: getPageGroups
      x-api-path-slug: pagegroups-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Groups
  /{page}/albums:
    get:
      summary: Get Page Albums
      description: The photo albums this Page has uploaded
      operationId: getPageAlbums
      x-api-path-slug: pagealbums-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Albums
  /{page}/statuses:
    get:
      summary: Get Page Statuses
      description: The page's status updates
      operationId: getPageStatuses
      x-api-path-slug: pagestatuses-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Statuses
    post:
      summary: Post Page Statuses
      description: Posts a status message on the page
      operationId: postPageStatuses
      x-api-path-slug: pagestatuses-post
      parameters:
      - in: query
        name: message
        description: Status Message content
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Statuses
  /{page}/videos:
    get:
      summary: Get Page Veos
      description: The videos contained on this page
      operationId: getPageVeos
      x-api-path-slug: pagevideos-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Videos
    post:
      summary: Post Page Veos
      description: Publishes a video to the page
      operationId: postPageVeos
      x-api-path-slug: pagevideos-post
      parameters:
      - in: query
        name: description
        description: Video description
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: title
        description: Video title
      responses:
        200:
          description: OK
      tags:
      - Page
      - Videos
  /{page}/notes:
    get:
      summary: Get Page Notes
      description: The notes contained on this page
      operationId: getPageNotes
      x-api-path-slug: pagenotes-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Notes
    post:
      summary: Post Page Notes
      description: Creates a note on the page
      operationId: postPageNotes
      x-api-path-slug: pagenotes-post
      parameters:
      - in: query
        name: message
        description: Note content
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: subject
        description: The subject of the Note
      responses:
        200:
          description: OK
      tags:
      - Page
      - Notes
  /{page}/posts:
    get:
      summary: Get Page Adds
      description: The page's own posts
      operationId: getPageAdds
      x-api-path-slug: pageposts-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Posts
  /{page}/events:
    get:
      summary: Get Page Events
      description: The events the Page is attending
      operationId: getPageEvents
      x-api-path-slug: pageevents-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Events
    post:
      summary: Post Page Events
      description: Creates an event for the page
      operationId: postPageEvents
      x-api-path-slug: pageevents-post
      parameters:
      - in: query
        name: end_time
        description: Event end time
      - in: query
        name: location
        description: Event location
      - in: query
        name: message
        description: Event description
      - in: query
        name: name
        description: Event name
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: privacy_type
        description: Event privacy setting
      - in: query
        name: start_time
        description: Event start time
      responses:
        200:
          description: OK
      tags:
      - Page
      - Events
  /{page}/checkins:
    get:
      summary: Get Page Checkins
      description: Checkins made to this Place Page by the current user, and friends
        of the current user
      operationId: getPageCheckins
      x-api-path-slug: pagecheckins-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Checkins
  /{page}/tabs:
    get:
      summary: Get Page Tabs
      description: The page's profile tabs
      operationId: getPageTabs
      x-api-path-slug: pagetabs-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Tabs
    post:
      summary: Post Page Tabs
      description: Installs a profile tab at the end of the current list of installed
        tabs for the page
      operationId: postPageTabs
      x-api-path-slug: pagetabs-post
      parameters:
      - in: query
        name: app_id
        description: ID of the application for which to install the tab
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Tabs
  /{page}/tabs/{tab}:
    post:
      summary: Post Page Tabs Tab
      description: Updates an installed profile tab for a page
      operationId: postPageTabsTab
      x-api-path-slug: pagetabstab-post
      parameters:
      - in: query
        name: custom_name
        description: Name to be used for the tab
      - in: query
        name: is_non_connection_landing_tab
        description: Set this tab as the default landing tab for users who have not
          liked and are not admins of the Page
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: position
        description: Order in which the tab will appear on the profile
      - in: path
        name: tab
        description: Represents the ID of the tab
      responses:
        200:
          description: OK
      tags:
      - Page
      - Tabs
      - Tab
    delete:
      summary: Delete Page Tabs Tab
      description: Deletes an installed profile tab (where is_permanent is not true)
        for a page
      operationId: deletePageTabsTab
      x-api-path-slug: pagetabstab-delete
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: path
        name: tab
        description: Represents the ID of the tab
      responses:
        200:
          description: OK
      tags:
      - Page
      - Tabs
      - Tab
  /{page}/admins:
    get:
      summary: Get Page Admins
      description: A list of the Page's admins.
      operationId: getPageAdmins
      x-api-path-slug: pageadmins-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Admins
  /{page}/blocked:
    get:
      summary: Get Page Blocked
      description: A list of the users blocked from the page.
      operationId: getPageBlocked
      x-api-path-slug: pageblocked-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Blocked
    post:
      summary: Post Page Blocked
      description: Blocks a user (or users) from posting content to the page
      operationId: postPageBlocked
      x-api-path-slug: pageblocked-post
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: uids
        description: Comma-separated list of the user IDs you wish to block
      responses:
        200:
          description: OK
      tags:
      - Page
      - Blocked
    delete:
      summary: Delete Page Blocked
      description: Unblocks a user (or users) for the page
      operationId: deletePageBlocked
      x-api-path-slug: pageblocked-delete
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: uids
        description: Comma-separated list of the user IDs you wish to unblock
      responses:
        200:
          description: OK
      tags:
      - Page
      - Blocked
  /{page}/blocked/{user}:
    get:
      summary: Get Page Blocked User
      description: Checks if a user is blocked from the page
      operationId: getPageBlockedUser
      x-api-path-slug: pageblockeduser-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: path
        name: user
        description: Represents the ID of a user
      responses:
        200:
          description: OK
      tags:
      - Page
      - Blocked
      - User
  /{photo}:
    get:
      summary: Get Photo
      description: An individual photo
      operationId: getPhoto
      x-api-path-slug: photo-get
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      responses:
        200:
          description: OK
      tags:
      - Photo
  /{photo}/comments:
    get:
      summary: Get Photo Comments
      description: All of the comments on this photo.
      operationId: getPhotoComments
      x-api-path-slug: photocomments-get
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Comments
    post:
      summary: Post Photo Comments
      description: Posts a comment to this photo.
      operationId: postPhotoComments
      x-api-path-slug: photocomments-post
      parameters:
      - in: query
        name: message
        description: Comment text
      - in: path
        name: photo
        description: Represents the ID of the photo object
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Comments
  /{photo}/likes:
    get:
      summary: Get Photo Likes
      description: Users who like this photo.
      operationId: getPhotoLikes
      x-api-path-slug: photolikes-get
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Likes
    post:
      summary: Post Photo Likes
      description: Likes this photo.
      operationId: postPhotoLikes
      x-api-path-slug: photolikes-post
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Likes
    delete:
      summary: Delete Photo Likes
      description: Unlikes this photo.
      operationId: deletePhotoLikes
      x-api-path-slug: photolikes-delete
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Likes
  /{photo}/picture:
    get:
      summary: Get Photo Picture
      description: The album-sized view of the photo
      operationId: getPhotoPicture
      x-api-path-slug: photopicture-get
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Picture
  /{photo}/tags:
    get:
      summary: Get Photo Tags
      description: Tags for this photo.
      operationId: getPhotoTags
      x-api-path-slug: phototags-get
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Tags
    post:
      summary: Post Photo Tags
      description: Creates a tag on this photo.
      operationId: postPhotoTags
      x-api-path-slug: phototags-post
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      - in: query
        name: to
        description: USER_ID of the User to tag; can also be provided in URL path
      - in: query
        name: x
        description: x coordinate of tag, as a percentage offset from the left edge
          of the picture
      - in: query
        name: "y"
        description: y coordinate of tag, as a percentage offset from the top edge
          of the picture
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Tags
  /{photo}/tags/{user}:
    post:
      summary: Post Photo Tags User
      description: Updates the position of a tag on this photo for the user.
      operationId: postPhotoTagsUser
      x-api-path-slug: phototagsuser-post
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      - in: path
        name: user
        description: Represents the ID of the user
      - in: query
        name: x
        description: x coordinate of tag, as a percentage offset from the left edge
          of the picture
      - in: query
        name: "y"
        description: y coordinate of tag, as a percentage offset from the top edge
          of the picture
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Tags
      - User
  /{post}:
    get:
      summary: Get Add
      description: A Facebook post
      operationId: getAdd
      x-api-path-slug: post-get
      parameters:
      - in: path
        name: post
        description: Represents the ID of the post object
      responses:
        200:
          description: OK
      tags:
      - Post
  /{post}/comments:
    get:
      summary: Get Add Comments
      description: All of the comments on this post.
      operationId: getAddComments
      x-api-path-slug: postcomments-get
      parameters:
      - in: path
        name: post
        description: Represents the ID of the post object
      responses:
        200:
          description: OK
      tags:
      - Post
      - Comments
    post:
      summary: Post Add Comments
      description: Posts a comment to this post.
      operationId: postAddComments
      x-api-path-slug: postcomments-post
      parameters:
      - in: query
        name: message
        description: Comment text
      - in: path
        name: post
        description: Represents the ID of the post object
      responses:
        200:
          description: OK
      tags:
      - Post
      - Comments
  /{post}/likes:
    get:
      summary: Get Add Likes
      description: Users who like this post.
      operationId: getAddLikes
      x-api-path-slug: postlikes-get
      parameters:
      - in: path
        name: post
        description: Represents the ID of the post object
      responses:
        200:
          description: OK
      tags:
      - Post
      - Likes
    post:
      summary: Post Add Likes
      description: Likes this post.
      operationId: postAddLikes
      x-api-path-slug: postlikes-post
      parameters:
      - in: path
        name: post
        description: Represents the ID of the post object
      responses:
        200:
          description: OK
      tags:
      - Post
      - Likes
    delete:
      summary: Delete Add Likes
      description: Unlikes this post.
      operationId: deleteAddLikes
      x-api-path-slug: postlikes-delete
      parameters:
      - in: path
        name: post
        description: Represents the ID of the post object
      responses:
        200:
          description: OK
      tags:
      - Post
      - Likes
  /{status}:
    get:
      summary: Get Status
      description: A Facebook status
      operationId: getStatus
      x-api-path-slug: status-get
      parameters:
      - in: path
        name: status
        description: Represents the ID of the status object
      responses:
        200:
          description: OK
      tags:
      - Status
  /{status}/comments:
    get:
      summary: Get Status Comments
      description: All of the comments on this status.
      operationId: getStatusComments
      x-api-path-slug: statuscomments-get
      parameters:
      - in: path
        name: status
        description: Represents the ID of the status object
      responses:
        200:
          description: OK
      tags:
      - Status
      - Comments
    post:
      summary: Post Status Comments
      description: Posts a comment to this status.
      operationId: postStatusComments
      x-api-path-slug: statuscomments-post
      parameters:
      - in: query
        name: message
        description: Comment text
      - in: path
        name: status
        description: Represents the ID of the status object
      responses:
        200:
          description: OK
      tags:
      - Status
      - Comments
  /{status}/likes:
    get:
      summary: Get Status Likes
      description: Users who like this status.
      operationId: getStatusLikes
      x-api-path-slug: statuslikes-get
      parameters:
      - in: path
        name: status
        description: Represents the ID of the status object
      responses:
        200:
          description: OK
      tags:
      - Status
      - Likes
    post:
      summary: Post Status Likes
      description: Likes this status.
      operationId: postStatusLikes
      x-api-path-slug: statuslikes-post
      parameters:
      - in: path
        name: status
        description: Represents the ID of the status object
      responses:
        200:
          description: OK
      tags:
      - Status
      - Likes
    delete:
      summary: Delete Status Likes
      description: Unlikes this status.
      operationId: deleteStatusLikes
      x-api-path-slug: statuslikes-delete
      parameters:
      - in: path
        name: status
        description: Represents the ID of the status object
      responses:
        200:
          description: OK
      tags:
      - Status
      - Likes
  /{user}:
    get:
      summary: Get User
      description: A user profile.
      operationId: getUser
      x-api-path-slug: user-get
      parameters:
      - in: query
        name: fields
        description: The fields to return
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
  /{user}/accounts:
    get:
      summary: Get User Accounts
      description: The Facebook apps and pages owned by the current user
      operationId: getUserAccounts
      x-api-path-slug: useraccounts-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Accounts
  /{user}/achievements:
    post:
      summary: Post User Achievements
      description: Posts an achievement for the user
      operationId: postUserAchievements
      x-api-path-slug: userachievements-post
      parameters:
      - in: query
        name: achievement
        description: The unique URL of the achievement which the user achieved
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Achievements
    delete:
      summary: Delete User Achievements
      description: Deletes an achievement for the user
      operationId: deleteUserAchievements
      x-api-path-slug: userachievements-delete
      parameters:
      - in: query
        name: achievement
        description: The unique URL of the achievement you wish to delete
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Achievements
  /{user}/activities:
    get:
      summary: Get User Activities
      description: The activities listed on the user's profile
      operationId: getUserActivities
      x-api-path-slug: useractivities-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Activities
  /{user}/albums:
    get:
      summary: Get User Albums
      description: The photo albums this user has created
      operationId: getUserAlbums
      x-api-path-slug: useralbums-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Albums
    post:
      summary: Post User Albums
      description: Creates an album for the user
      operationId: postUserAlbums
      x-api-path-slug: useralbums-post
      parameters:
      - in: query
        name: message
        description: Album description
      - in: query
        name: name
        description: Album name
      - in: query
        name: privacy
        description: Privacy settings for the Album
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Albums
  /{user}/apprequests:
    get:
      summary: Get User Apprequests
      description: The user's outstanding requests from an app.
      operationId: getUserApprequests
      x-api-path-slug: userapprequests-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Apprequests
  /{user}/books:
    get:
      summary: Get User Books
      description: The books listed on the user's profile.
      operationId: getUserBooks
      x-api-path-slug: userbooks-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Books
  /{user}/checkins:
    get:
      summary: Get User Checkins
      description: The places that the user has checked-into
      operationId: getUserCheckins
      x-api-path-slug: usercheckins-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Checkins
    post:
      summary: Post User Checkins
      description: Checks the user into a place
      operationId: postUserCheckins
      x-api-path-slug: usercheckins-post
      parameters:
      - in: query
        name: coordinates
        description: 'The users location, as a string containing latitude and longitude:
          {latitude:'
      - in: query
        name: link
        description: Checkin link
      - in: query
        name: message
        description: Checkin description
      - in: query
        name: picture
        description: Checkin picture
      - in: query
        name: place
        description: Checkin Place ID; for example 110506962309835 for Facebook HQ
      - in: query
        name: tags
        description: Comma-separated list of tagged friends user IDs
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Checkins
  /{user}/events:
    get:
      summary: Get User Events
      description: The events this user is attending.
      operationId: getUserEvents
      x-api-path-slug: userevents-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Events
    post:
      summary: Post User Events
      description: Creates an event for the user
      operationId: postUserEvents
      x-api-path-slug: userevents-post
      parameters:
      - in: query
        name: end_time
        description: Event end time
      - in: query
        name: location
        description: Event location
      - in: query
        name: message
        description: Event description
      - in: query
        name: name
        description: Event name
      - in: query
        name: privacy_type
        description: Event privacy setting
      - in: query
        name: start_time
        description: Event start time
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Events
  /{user}/feed:
    get:
      summary: Get User Feed
      description: This user's wall
      operationId: getUserFeed
      x-api-path-slug: userfeed-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Feed
    post:
      summary: Post User Feed
      description: Posts a status message on this user's wall
      operationId: postUserFeed
      x-api-path-slug: userfeed-post
      parameters:
      - in: query
        name: message
        description: Status Message content
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Feed
  /{user}/friendlists:
    post:
      summary: Post User Friendlists
      description: Creates a FriendList for the user
      operationId: postUserFriendlists
      x-api-path-slug: userfriendlists-post
      parameters:
      - in: query
        name: name
        description: Friend list name
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Friendlists
  /{user}/friends:
    get:
      summary: Get User Friends
      description: The user's friends
      operationId: getUserFriends
      x-api-path-slug: userfriends-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Friends
  /{user}/friends/{friend}:
    get:
      summary: Get User Friends Friend
      description: Checks if the given user is a friend of the current user
      operationId: getUserFriendsFriend
      x-api-path-slug: userfriendsfriend-get
      parameters:
      - in: path
        name: friend
        description: Represents the ID of the users friend
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Friends
      - Friend
  /{user}/games:
    get:
      summary: Get User Games
      description: Games the user has added to the Arts and Entertainment section
        of their profile.
      operationId: getUserGames
      x-api-path-slug: usergames-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Games
  /{user}/groups:
    get:
      summary: Get User Groups
      description: The Groups that the user belongs to.
      operationId: getUserGroups
      x-api-path-slug: usergroups-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Groups
  /{user}/home:
    get:
      summary: Get User Home
      description: The user's news feed
      operationId: getUserHome
      x-api-path-slug: userhome-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Home
  /{user}/inbox:
    get:
      summary: Get User Inbox
      description: The threads in this user's inbox.
      operationId: getUserInbox
      x-api-path-slug: userinbox-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Inbox
  /{user}/interests:
    get:
      summary: Get User Interests
      description: The interests listed on the user's profile
      operationId: getUserInterests
      x-api-path-slug: userinterests-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Interests
  /{user}/likes:
    get:
      summary: Get User Likes
      description: All the pages this user has liked.
      operationId: getUserLikes
      x-api-path-slug: userlikes-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Likes
  /{user}/likes/{page}:
    get:
      summary: Get User Likes Page
      description: Checks if the user likes the given page.
      operationId: getUserLikesPage
      x-api-path-slug: userlikespage-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Likes
      - Page
  /{user}/links:
    get:
      summary: Get User Links
      description: The user's posted links.
      operationId: getUserLinks
      x-api-path-slug: userlinks-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Links
    post:
      summary: Post User Links
      description: Posts a link on the user's profile page
      operationId: postUserLinks
      x-api-path-slug: userlinks-post
      parameters:
      - in: query
        name: link
        description: Link URL
      - in: query
        name: message
        description: Link message
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Links
  /{user}/movies:
    get:
      summary: Get User Movies
      description: The movies listed on the user's profile
      operationId: getUserMovies
      x-api-path-slug: usermovies-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Movies
  /{user}/music:
    get:
      summary: Get User Music
      description: The music listed on the user's profile
      operationId: getUserMusic
      x-api-path-slug: usermusic-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Music
  /{user}/notes:
    get:
      summary: Get User Notes
      description: The user's notes
      operationId: getUserNotes
      x-api-path-slug: usernotes-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Notes
    post:
      summary: Post User Notes
      description: Creates a note on behalf of the user
      operationId: postUserNotes
      x-api-path-slug: usernotes-post
      parameters:
      - in: query
        name: message
        description: Note content
      - in: query
        name: subject
        description: The subject of the Note
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Notes
  /{user}/notifications:
    get:
      summary: Get User Notifications
      description: The user's notifications
      operationId: getUserNotifications
      x-api-path-slug: usernotifications-get
      parameters:
      - in: query
        name: include_read
        description: Enables you to see notifications that the user has already read
          in addition to the ones which are unread
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Notifications
  /{user}/outbox:
    get:
      summary: Get User Outbox
      description: The messages in this user's outbox.
      operationId: getUserOutbox
      x-api-path-slug: useroutbox-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Outbox
  /{user}/payments:
    get:
      summary: Get User Payments
      description: The transactions the user placed with an application.
      operationId: getUserPayments
      x-api-path-slug: userpayments-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Payments
  /{user}/permissions:
    get:
      summary: Get User Permissions
      description: The permissions that user has granted the application.
      operationId: getUserPermissions
      x-api-path-slug: userpermissions-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Permissions
    delete:
      summary: Delete User Permissions
      description: De-authorizes an application or revokes a specific extended permissions
        on behalf of a user
      operationId: deleteUserPermissions
      x-api-path-slug: userpermissions-delete
      parameters:
      - in: query
        name: permission
        description: The permission you wish to revoke
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Permissions
  /{user}/photos:
    get:
      summary: Get User Photos
      description: The photos the user is tagged in
      operationId: getUserPhotos
      x-api-path-slug: userphotos-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Photos
    post:
      summary: Post User Photos
      description: Posts a photo to the user's Wall
      operationId: postUserPhotos
      x-api-path-slug: userphotos-post
      parameters:
      - in: query
        name: message
        description: Photo description
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Photos
  /{user}/picture:
    get:
      summary: Get User Picture
      description: The user's profile picture
      operationId: getUserPicture
      x-api-path-slug: userpicture-get
      parameters:
      - in: query
        name: type
        description: One of square (50x50), small (50 pixels wide, variable height),
          and large (about 200 pixels wide,                                                        variable
          height)
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Picture
  /{user}/pokes:
    get:
      summary: Get User Pokes
      description: The user's pokes
      operationId: getUserPokes
      x-api-path-slug: userpokes-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Pokes
  /{user}/posts:
    get:
      summary: Get User Adds
      description: The user's posts
      operationId: getUserAdds
      x-api-path-slug: userposts-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Posts
    post:
      summary: Post User Adds
      description: Creates a post on behalf of the user
      operationId: postUserAdds
      x-api-path-slug: userposts-post
      parameters:
      - in: query
        name: actions
        description: Post actions
      - in: query
        name: caption
        description: Post caption
      - in: query
        name: description
        description: Post description
      - in: query
        name: link
        description: Post URL
      - in: query
        name: message
        description: Post message
      - in: query
        name: name
        description: Post name
      - in: query
        name: object_attachment
        description: Facebook ID for an existing picture in the Users photo albums
          to use as the thumbnail image
      - in: query
        name: picture
        description: Post thumbnail image
      - in: query
        name: privacy
        description: Post privacy settings
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Posts
  /{user}/scores:
    get:
      summary: Get User Scores
      description: The scores for the user
      operationId: getUserScores
      x-api-path-slug: userscores-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Scores
    post:
      summary: Post User Scores
      description: Posts a score for the user
      operationId: postUserScores
      x-api-path-slug: userscores-post
      parameters:
      - in: query
        name: score
        description: Numeric score with value < 0
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Scores
  /{user}/statuses:
    get:
      summary: Get User Statuses
      description: The user's status updates
      operationId: getUserStatuses
      x-api-path-slug: userstatuses-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Statuses
    post:
      summary: Post User Statuses
      description: Posts a status message on the user
      operationId: postUserStatuses
      x-api-path-slug: userstatuses-post
      parameters:
      - in: query
        name: message
        description: Status Message content
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Statuses
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