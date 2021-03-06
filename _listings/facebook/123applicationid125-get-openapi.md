---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get Application
  description: Application
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
  /&#123;application-context-id&#125;:
    get:
      summary: Get Application Context
      description: Application Context
      operationId: getApplicationContext
      x-api-path-slug: 123applicationcontextid125-get
      parameters:
      - in: query
        name: idstring
        description: The token representing the social context
        type: string
      responses:
        200:
          description: OK
      tags:
      - Application
      - Context
  /&#123;analytics-app-events-export-id&#125;:
    get:
      summary: Get Analytics App Events Export
      description: Analytics App Events Export
      operationId: getAnalyticsAppEventsExport
      x-api-path-slug: 123analyticsappeventsexportid125-get
      parameters:
      - in: query
        name: column_namesliststring
        description: Names of columns in the tableDefault
        type: string
      - in: query
        name: end_tsdatetime
        description: End time for the exportDefault
        type: string
      - in: query
        name: error_messagestring
        description: User error messageDefault
        type: string
      - in: query
        name: event_param_nameslistAnalyticsAppEventsExportEventParamNames
        description: Parameters names for each events that map to custom1-25 in data
          tableDefault
        type: string
      - in: query
        name: idnumeric string
        description: ID of the app events export jobDefault
        type: string
      - in: query
        name: recent_download_timestampslistdatetime
        description: Timestamps for recent downloads of the export
        type: string
      - in: query
        name: request_tsdatetime
        description: Time when the export was requested
        type: string
      - in: query
        name: start_tsdatetime
        description: Start time for the exportDefault
        type: string
      - in: query
        name: statusenum
        description: Status of the export jobDefault
        type: string
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - App
      - Events
      - Export
  /&#123;application-id&#125;:
    get:
      summary: Get Application
      description: Application
      operationId: getApplication
      x-api-path-slug: 123applicationid125-get
      parameters:
      - in: query
        name: an_ad_space_limitunsigned int32
        description: The maximum number ofAd Spaces allowed for each Audience Network
          supported platform
        type: string
      - in: query
        name: an_platformslistenum
        description: The platforms associated with the app in the Audience Network
          product
        type: string
      - in: query
        name: app_domainsliststring
        description: Domains and subdomains this app can use
        type: string
      - in: query
        name: app_install_trackedbool
        description: Whether the app install is trackable or not
        type: string
      - in: query
        name: app_namestring
        description: App name
        type: string
      - in: query
        name: app_typeunsigned int32
        description: App type
        type: string
      - in: query
        name: auth_dialog_data_help_urlstring
        description: The URL of a special landing page that helps people who are using
          an app begin publishing Open Graph activity
        type: string
      - in: query
        name: auth_dialog_headlinestring
        description: One line description of an app that appears in the Login Dialog
        type: string
      - in: query
        name: auth_dialog_perms_explanationstring
        description: The text to explain why an app needs additional permissions
        type: string
      - in: query
        name: auth_referral_default_activity_privacystring
        description: The default privacy setting selected for Open Graph activities
          in the Auth Dialog
        type: string
      - in: query
        name: auth_referral_enabledunsigned int32
        description: Indicates whether Authenticated Referrals are enabled
        type: string
      - in: query
        name: auth_referral_extended_permsliststring
        description: Extended permissions that a person can choose to grant when Authenticated
          Referrals are enabled
        type: string
      - in: query
        name: auth_referral_friend_permsliststring
        description: Basic friends permissions that a user must grant when Authenticated
          Referrals are enabled
        type: string
      - in: query
        name: auth_referral_response_typestring
        description: The format that an app receives for the authentication token
          from the Login Dialog
        type: string
      - in: query
        name: auth_referral_user_permsliststring
        description: Basic user permissions that a user must grant when Authenticated
          Referrals are enabled
        type: string
      - in: query
        name: businessBusiness
        description: Business owner of this app
        type: string
      - in: query
        name: canvas_fluid_heightbool
        description: Indicates whether the app uses fluid or settable height values
          for Canvas
        type: string
      - in: query
        name: canvas_fluid_widthunsigned int32
        description: Indicates whether the app uses fluid or fixed width values for
          Canvas
        type: string
      - in: query
        name: canvas_urlstring
        description: The non-secure URL from which Canvas app content is loaded
        type: string
      - in: query
        name: categorystring
        description: The category of the appDefault
        type: string
      - in: query
        name: client_configmap
        description: Config data for the client
        type: string
      - in: query
        name: companystring
        description: The company the app belongs to
        type: string
      - in: query
        name: configured_ios_ssobool
        description: True if the app has configured Single Sign On on iOS
        type: string
      - in: query
        name: contact_emailstring
        description: Email address listed for people using the app to contact developers
        type: string
      - in: query
        name: contextApplicationContext
        description: Social context for the app
        type: string
      - in: query
        name: created_timedatetime
        description: Timestamp that indicates when the app was created
        type: string
      - in: query
        name: creator_uidid
        description: User ID of the creator of this app
        type: string
      - in: query
        name: daily_active_usersnumeric string
        description: The number of daily active users the app has
        type: string
      - in: query
        name: daily_active_users_rankunsigned int32
        description: Ranking of this app vs other apps comparing daily active users
        type: string
      - in: query
        name: deauth_callback_urlstring
        description: URL that is pinged whenever a person removes the app
        type: string
      - in: query
        name: default_share_modestring
        description: The platform that should be used to share content
        type: string
      - in: query
        name: descriptionstring
        description: The description of the app, as provided by the developerCore
        type: string
      - in: query
        name: financial_idstring
        description: The ID for the corresponding audience network financial entity
        type: string
      - in: query
        name: hosting_urlstring
        description: Webspace created with one of our hosting partners for this app
        type: string
      - in: query
        name: icon_urlstring
        description: The URL of this app&#039;s icon
        type: string
      - in: query
        name: idnumeric string
        description: The app IDCore
        type: string
      - in: query
        name: ios_bundle_idliststring
        description: Bundle ID of the associated iOS app
        type: string
      - in: query
        name: ios_supports_native_proxy_auth_flowbool
        description: Whether to support the native proxy login flow
        type: string
      - in: query
        name: ios_supports_system_authbool
        description: Whether to support the iOS integrated Login Dialog
        type: string
      - in: query
        name: ipad_app_store_idstring
        description: ID of the app in the iPad App Store
        type: string
      - in: query
        name: iphone_app_store_idstring
        description: ID of the app in the iPhone App Store
        type: string
      - in: query
        name: is_viewer_adminbool
        description: Test if viewer is one of admins of this app
        type: string
      - in: query
        name: latest_sdk_versionApplicationSDKInfo
        description: App latest sdk version
        type: string
      - in: query
        name: linkstring
        description: A link to the app on FacebookCoreDefault
        type: string
      - in: query
        name: logging_tokenstring
        description: To use for logging purposes
        type: string
      - in: query
        name: logo_urlstring
        description: The URL of the app&#039;s logo
        type: string
      - in: query
        name: migrationsmapstring, bool
        description: Status of migrations for this app
        type: string
      - in: query
        name: mobile_profile_section_urlstring
        description: Mobile URL of the app section on a person&#039;s profile
        type: string
      - in: query
        name: mobile_web_urlstring
        description: URL to which Mobile users will be directed when using the app
        type: string
      - in: query
        name: monthly_active_usersnumeric string
        description: The number of monthly active users the app has
        type: string
      - in: query
        name: monthly_active_users_rankunsigned int32
        description: Ranking of this app vs other apps comparing monthly active users
        type: string
      - in: query
        name: namespacestring
        description: The string appended to apps
        type: string
      - in: query
        name: namestring
        description: The name of the appCoreDefault
        type: string
      - in: query
        name: object_store_urlsApplicationObjectStoreURLs
        description: Mobile store URLs for the app
        type: string
      - in: query
        name: page_tab_default_namestring
        description: The title of the app when used in a Page Tab
        type: string
      - in: query
        name: page_tab_urlstring
        description: The non-secure URL from which Page Tab app content is loaded
        type: string
      - in: query
        name: photo_urlstring
        description: The URL of the app photo
        type: string
      - in: query
        name: privacy_policy_urlstring
        description: The URL that links to a Privacy Policy for the app
        type: string
      - in: query
        name: profile_section_urlstring
        description: URL of the app section on a user&#039;s profile for the desktop
          site
        type: string
      - in: query
        name: restrictionsApplicationRestrictionInfo
        description: Demographic restrictions for the app
        type: string
      - in: query
        name: secure_canvas_urlstring
        description: The secure URL from which Canvas app content is loaded
        type: string
      - in: query
        name: secure_page_tab_urlstring
        description: The secure URL from which Page Tab app content is loaded
        type: string
      - in: query
        name: server_ip_whiteliststring
        description: App requests must originate from this comma-separated list of
          IP addresses
        type: string
      - in: query
        name: social_discoveryunsigned int32
        description: Indicates whether app usage stories show up in the Ticker or
          News Feed
        type: string
      - in: query
        name: subcategorystring
        description: The subcategory the app can be found under
        type: string
      - in: query
        name: supported_platformslistenum &#123;WEB, CANVAS, MOBILE_WEB, IPHONE, IPAD,
          ANDROID, WINDOWS, AMAZON, SUPPLEMENTARY_IMAGES, GAMEROOM, INSTANT_GAME&#125;
        description: All the platform the app supports
        type: string
      - in: query
        name: terms_of_service_urlstring
        description: URL to Terms of Service that appears in the Login Dialog
        type: string
      - in: query
        name: url_scheme_suffixstring
        description: URL scheme suffix
        type: string
      - in: query
        name: user_support_emailstring
        description: Main contact email for this app where people can receive support
        type: string
      - in: query
        name: user_support_urlstring
        description: URL shown in the Canvas footer that people can visit to get support
          for the app
        type: string
      - in: query
        name: website_urlstring
        description: URL of a website that integrates with this app
        type: string
      - in: query
        name: weekly_active_usersnumeric string
        description: The number of weekly active users the app has
        type: string
      responses:
        200:
          description: OK
      tags:
      - Application
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