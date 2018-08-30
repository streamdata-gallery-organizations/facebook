---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get Group Files
  description: The files uploaded to this group.
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
  /&#123;audience-insights-rule-id&#125;:
    get:
      summary: Get Audience Insights Rule
      description: Audience Insights Rule
      operationId: getAudienceInsightsRule
      x-api-path-slug: 123audienceinsightsruleid125-get
      parameters:
      - in: query
        name: archivedbool
        description: Archive status of the study rule
        type: string
      - in: query
        name: can_be_updatedbool
        description: Tells you if the rule can be updatedDefault
        type: string
      - in: query
        name: created_byUser
        description: The creator of the study rule
        type: string
      - in: query
        name: creation_timedatetime
        description: The creation time of the study rule
        type: string
      - in: query
        name: descriptionstring
        description: Description of the study rule
        type: string
      - in: query
        name: idnumeric string
        description: IDDefault
        type: string
      - in: query
        name: languageenum
        description: The language of the ruleDefault
        type: string
      - in: query
        name: namestring
        description: Name of the study rule
        type: string
      - in: query
        name: rule_componentslistAudienceInsightsRuleComponent
        description: Rule componentsDefault
        type: string
      - in: query
        name: studieslistAudienceStudy
        description: Studies using the study rule
        type: string
      responses:
        200:
          description: OK
      tags:
      - Audience
      - Insights
      - Rule
  /&#123;canvas-id&#125;:
    get:
      summary: Get Canvas
      description: Canvas
      operationId: getCanvas
      x-api-path-slug: 123canvasid125-get
      parameters:
      - in: query
        name: background_colorstring
        description: Background color of the canvas
        type: string
      - in: query
        name: body_elementslistCanvasPhoto|CanvasHeader|CanvasVideo|CanvasText|CanvasCarousel|CanvasButton|CanvasFooter|CanvasStoreLocator|CanvasProductList|CanvasProductSet|CanvasLeadForm
        description: Body element nodes for the canvas
        type: string
      - in: query
        name: canvas_linkstring
        description: The canvas link for the canvas
        type: string
      - in: query
        name: idnumeric string
        description: ID of the canvas
        type: string
      - in: query
        name: is_hiddenbool
        description: The canvas is hidden or not
        type: string
      - in: query
        name: is_publishedbool
        description: Publish status of the canvas
        type: string
      - in: query
        name: last_editorUser
        description: User who last edited this canvas
        type: string
      - in: query
        name: namestring
        description: Name used to label the canvasDefault
        type: string
      - in: query
        name: ownerPage
        description: Page that owns this canvas
        type: string
      - in: query
        name: update_timeint32
        description: Last updated time of the canvas
        type: string
      responses:
        200:
          description: OK
      tags:
      - Canvas
  /&#123;canvas-button-id&#125;:
    get:
      summary: Get Canvas Button
      description: Canvas Button
      operationId: getCanvasButton
      x-api-path-slug: 123canvasbuttonid125-get
      parameters:
      - in: query
        name: actionCanvasOpenURLAction
        description: The action associated with the button
        type: string
      - in: query
        name: background_colorstring
        description: Color of the button background
        type: string
      - in: query
        name: bottom_paddingnumeric string
        description: The padding below the element
        type: string
      - in: query
        name: button_colorstring
        description: Color of the button
        type: string
      - in: query
        name: button_styleenum
        description: The style of the button
        type: string
      - in: query
        name: deep_linkstring
        description: Deep link destination only for mobile apps          (used for
          mobile install or engagement ads, and app link is supported)
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
        name: font_familystring
        description: The font family
        type: string
      - in: query
        name: font_sizenumeric string
        description: The size of the font for the text
        type: string
      - in: query
        name: idnumeric string
        description: The id of the element
        type: string
      - in: query
        name: line_heightnumeric string
        description: The line height of the text
        type: string
      - in: query
        name: namestring
        description: The name of the elementDefault
        type: string
      - in: query
        name: rich_textCanvasRichText
        description: The text inside the button
        type: string
      - in: query
        name: text_alignmentenum
        description: The alignment of the text
        type: string
      - in: query
        name: text_colorstring
        description: The color of the text
        type: string
      - in: query
        name: top_paddingnumeric string
        description: The padding above the element
        type: string
      responses:
        200:
          description: OK
      tags:
      - Canvas
      - Button
  /&#123;canvas-carousel-id&#125;:
    get:
      summary: Get Canvas Carousel
      description: Canvas Carousel
      operationId: getCanvasCarousel
      x-api-path-slug: 123canvascarouselid125-get
      parameters:
      - in: query
        name: bottom_paddingnumeric string
        description: The padding below the element
        type: string
      - in: query
        name: child_elementslistCanvasPhoto
        description: The child elements of the carousel
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
        description: The presentation style of the carousel
        type: string
      - in: query
        name: top_paddingnumeric string
        description: The padding above the element
        type: string
      responses:
        200:
          description: OK
      tags:
      - Canvas
      - Carousel
  /&#123;canvas-footer-id&#125;:
    get:
      summary: Get Canvas Footer
      description: Canvas Footer
      operationId: getCanvasFooter
      x-api-path-slug: 123canvasfooterid125-get
      parameters:
      - in: query
        name: background_colorstring
        description: Background color of the button
        type: string
      - in: query
        name: bottom_paddingnumeric string
        description: The padding below the element
        type: string
      - in: query
        name: child_elementslistCanvasButton
        description: The child elements inside a footer
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
        name: top_paddingnumeric string
        description: The padding above the element
        type: string
      responses:
        200:
          description: OK
      tags:
      - Canvas
      - Footer
  /&#123;canvas-header-id&#125;:
    get:
      summary: Get Canvas Header
      description: Canvas Header
      operationId: getCanvasHeader
      x-api-path-slug: 123canvasheaderid125-get
      parameters:
      - in: query
        name: background_colorstring
        description: The background color of the header
        type: string
      - in: query
        name: bottom_paddingnumeric string
        description: bottom_padding
        type: string
      - in: query
        name: child_elementslistCanvasPhoto
        description: The child elements (typically a photo) inside the header
        type: string
      - in: query
        name: element_group_keystring
        description: element_group_key
        type: string
      - in: query
        name: element_typeenum
        description: element_typeDefault
        type: string
      - in: query
        name: idnumeric string
        description: id
        type: string
      - in: query
        name: namestring
        description: nameDefault
        type: string
      - in: query
        name: top_paddingnumeric string
        description: top_padding
        type: string
      responses:
        200:
          description: OK
      tags:
      - Canvas
      - Header
  /&#123;canvas-photo-id&#125;:
    get:
      summary: Get Canvas Photo
      description: Canvas Photo
      operationId: getCanvasPhoto
      x-api-path-slug: 123canvasphotoid125-get
      parameters:
      - in: query
        name: actionCanvasOpenURLAction
        description: The action associated with the photo
        type: string
      - in: query
        name: bottom_paddingnumeric string
        description: The padding below the element
        type: string
      - in: query
        name: deep_linkstring
        description: Deep link destination only for mobile apps          (used for
          mobile install or engagement ads, and app link is supported)
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
        name: hide_product_pricesbool
        description: Flag to determine whether or not to hide prices for tagged products
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
        name: photoPhoto
        description: The facebook photo node
        type: string
      - in: query
        name: product_tagslistCanvasProductTag
        description: The product tags on the photo
        type: string
      - in: query
        name: styleenum
        description: The presentation style of the photo node
        type: string
      - in: query
        name: top_paddingnumeric string
        description: The padding above the element
        type: string
      responses:
        200:
          description: OK
      tags:
      - Canvas
      - Photo
  /&#123;canvas-product-set-id&#125;:
    get:
      summary: Get Canvas Product Set
      description: Canvas Product Set
      operationId: getCanvasProductSet
      x-api-path-slug: 123canvasproductsetid125-get
      parameters:
      - in: query
        name: bottom_paddingnumeric string
        description: bottom_padding
        type: string
      - in: query
        name: element_group_keystring
        description: element_group_key
        type: string
      - in: query
        name: element_typeenum
        description: element_typeDefault
        type: string
      - in: query
        name: idnumeric string
        description: id
        type: string
      - in: query
        name: image_overlay_specAdCreativeLinkDataImageOverlaySpec
        description: How to render overlays over a product item
        type: string
      - in: query
        name: item_descriptionstring
        description: A token to represent which field from the product to show in
          the product description
        type: string
      - in: query
        name: item_headlinestring
        description: A token to represent which field from the product to show in
          the product headline
        type: string
      - in: query
        name: max_productsunsigned int32
        description: Maximum number of products to show
        type: string
      - in: query
        name: namestring
        description: nameDefault
        type: string
      - in: query
        name: product_set_idnumeric string
        description: The product set id which contains a subset of products within
          a product catalog
        type: string
      - in: query
        name: retailer_item_idsstring
        description: An array of items that should be shown first in the product set
          element
        type: string
      - in: query
        name: show_in_feedbool
        description: A flag that products should be shown in feed unit
        type: string
      - in: query
        name: top_paddingnumeric string
        description: top_padding
        type: string
      responses:
        200:
          description: OK
      tags:
      - Canvas
      - Product
      - Set
  /&#123;canvas-store-locator-id&#125;:
    get:
      summary: Get Canvas Store Locator
      description: Canvas Store Locator
      operationId: getCanvasStoreLocator
      x-api-path-slug: 123canvasstorelocatorid125-get
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
        name: header_background_colorstring
        description: Header background color for the store locator
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
        name: top_paddingnumeric string
        description: The padding above the element
        type: string
      - in: query
        name: typefacestring
        description: Font used to display info about the store
        type: string
      responses:
        200:
          description: OK
      tags:
      - Canvas
      - Store
      - Locator
  /&#123;canvas-text-id&#125;:
    get:
      summary: Get Canvas Text
      description: Canvas Text
      operationId: getCanvasText
      x-api-path-slug: 123canvastextid125-get
      parameters:
      - in: query
        name: background_colorstring
        description: The color of the background for the element
        type: string
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
        name: font_familystring
        description: The font family
        type: string
      - in: query
        name: font_sizenumeric string
        description: The size of the font for the text
        type: string
      - in: query
        name: idnumeric string
        description: The id of the element
        type: string
      - in: query
        name: line_heightnumeric string
        description: The line height of the text
        type: string
      - in: query
        name: namestring
        description: The name of the elementDefault
        type: string
      - in: query
        name: rich_textCanvasRichText
        description: The text content of the element
        type: string
      - in: query
        name: text_alignmentenum
        description: The alignment of the text
        type: string
      - in: query
        name: text_colorstring
        description: The color of the text
        type: string
      - in: query
        name: top_paddingnumeric string
        description: The padding above the element
        type: string
      responses:
        200:
          description: OK
      tags:
      - Canvas
      - Text
  /&#123;comment-id&#125;:
    get:
      summary: Get Comment
      description: A comment can be made on various types of content on Facebook.
        Most Graph API nodes have a /comments edge that lists all the comments on
        that object. The /&#123;comment-id&#125; node returns a single comment.
      operationId: getComment
      x-api-path-slug: 123commentid125-get
      parameters:
      - in: query
        name: attachment
        description: Link, video, sticker, or photo attached to the comment
        type: string
      - in: query
        name: can_comment
        description: Whether the viewer can reply to this comment
        type: string
      - in: query
        name: can_hide
        description: Whether the viewer can hide this comment
        type: string
      - in: query
        name: can_like
        description: Whether the viewer can like this comment
        type: string
      - in: query
        name: can_remove
        description: Whether the viewer can remove this comment
        type: string
      - in: query
        name: can_reply_privately
        description: Whether the viewer can send a private reply to this comment (Page
          viewers only)
        type: string
      - in: query
        name: comment_count
        description: Number of replies to this comment
        type: string
      - in: query
        name: created_time
        description: The time this comment was made
        type: string
      - in: query
        name: from
        description: The person that made this comment
        type: string
      - in: query
        name: id
        description: The comment ID
        type: string
      - in: query
        name: length
        description: How many unicode code points this tag consists of, after the
          offset
        type: string
      - in: query
        name: like_count
        description: Number of times this comment was liked
        type: string
      - in: query
        name: message
        description: The comment text
        type: string
      - in: query
        name: message_tags
        description: An array of Profiles tagged in message
        type: string
      - in: query
        name: name
        description: The text used in the tag
        type: string
      - in: query
        name: object
        description: For comments on a photo or video, this is that object
        type: string
      - in: query
        name: offset
        description: Where the first character of the tagged text is in the message,
          measured in unicode code points
        type: string
      - in: query
        name: parent
        description: For comment replies, this the comment that this is a reply to
        type: string
      - in: query
        name: private_reply_conversation
        description: For comments with private replies, gets conversation between
          the Page and author of the comment (Page viewers only)
        type: string
      - in: query
        name: type
        description: Indicates which type of profile is tagged
        type: string
      - in: query
        name: user_likes
        description: Whether the viewer has liked this comment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comment
    delete:
      summary: Delete Comment
      description: A comment can be made on various types of content on Facebook.
        Most Graph API nodes have a /comments edge that lists all the comments on
        that object. The /&#123;comment-id&#125; node returns a single comment.
      operationId: deleteComment
      x-api-path-slug: 123commentid125-delete
      responses:
        200:
          description: OK
      tags:
      - Comment
    post:
      summary: Post Comment
      description: A comment can be made on various types of content on Facebook.
        Most Graph API nodes have a /comments edge that lists all the comments on
        that object. The /&#123;comment-id&#125; node returns a single comment.
      operationId: postComment
      x-api-path-slug: 123commentid125-post
      parameters:
      - in: query
        name: is_hidden
        description: Whether this comment is hidden or visible
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comment
  /&#123;object-id&#125;/private_replies:
    post:
      summary: Post Object Private Replies
      description: 'This edge allows Pages to reply to Post Comments and Visitor Posts
        with a private Message. It can be used with the following nodes:'
      operationId: postObjectPrivateReplies
      x-api-path-slug: 123objectid125private-replies-post
      parameters:
      - in: query
        name: id
        description: The ID of the Page Comment or Visitor Post that you are replying
          to
        type: string
      - in: query
        name: message
        description: The text of the reply
        type: string
      responses:
        200:
          description: OK
      tags:
      - Object
      - Private
      - Replies
  /&#123;conversation-id&#125;:
    get:
      summary: Get Conversation
      description: A Facebook Messages conversation between a person and a Facebook
        Page.
      operationId: getConversation
      x-api-path-slug: 123conversationid125-get
      parameters:
      - in: query
        name: can_reply
        description: Whether the Page is able to reply
        type: string
      - in: query
        name: id
        description: The ID of a conversation, in a format similar to t_id
        type: string
      - in: query
        name: is_subscribed
        description: Whether the Page is subscribed to the conversation
        type: string
      - in: query
        name: link
        description: The url to the thread
        type: string
      - in: query
        name: message_count
        description: An estimate of the number of messages
        type: string
      - in: query
        name: participants
        description: People and Pages who are on this conversation
        type: string
      - in: query
        name: senders
        description: People who have sent a message
        type: string
      - in: query
        name: snippet
        description: The snippet of the most recent message in a conversation
        type: string
      - in: query
        name: unread_count
        description: An estimate of the number of unread messages
        type: string
      - in: query
        name: updated_time
        description: Last update time
        type: string
      - in: query
        name: Vector
        description: Vector
        type: string
      responses:
        200:
          description: OK
      tags:
      - Conversation
  /&#123;conversation-id&#125;/messages:
    get:
      summary: Get Conversation Messages
      description: The messages in a conversation between a person and a page.
      operationId: getConversationMessages
      x-api-path-slug: 123conversationid125messages-get
      parameters:
      - in: query
        name: Vector
        description: Vector
        type: string
      responses:
        200:
          description: OK
      tags:
      - Conversation
      - Messages
    post:
      summary: Post Conversation Messages
      description: The messages in a conversation between a person and a page.
      operationId: postConversationMessages
      x-api-path-slug: 123conversationid125messages-post
      parameters:
      - in: query
        name: message
        description: The text of reply
        type: string
      responses:
        200:
          description: OK
      tags:
      - Conversation
      - Messages
  /debug_token?input_token=&#123;input-token&#125;:
    get:
      summary: Get Debug Token Input Token Input Token
      description: This endpoint returns metadata about a given access token. This
        includes data such as the user for which the token was issued, whether the
        token is still valid, when it expires, and what permissions the app has for
        the given user.
      operationId: getDebugTokenInupdateTokenInupdateToken
      x-api-path-slug: debug-tokeninput-token123inputtoken125-get
      parameters:
      - in: query
        name: application
        description: Name of the application this access token is for
        type: string
      - in: query
        name: app_id
        description: The ID of the application this access token is for
        type: string
      - in: query
        name: code
        description: The error code for the error
        type: string
      - in: query
        name: data
        description: Data wrapper around the result
        type: string
      - in: query
        name: error
        description: Any error that a request to the graph api would return due to
          the access token
        type: string
      - in: query
        name: expires_at
        description: Timestamp when this access token expires
        type: string
      - in: query
        name: issued_at
        description: Timestamp when this access token was issued
        type: string
      - in: query
        name: is_valid
        description: Whether the access token is still valid or not
        type: string
      - in: query
        name: message
        description: The error message for the error
        type: string
      - in: query
        name: metadata
        description: General metadata associated with the access token
        type: string
      - in: query
        name: profile_id
        description: For impersonated access tokens, the ID of the page this token
          contains
        type: string
      - in: query
        name: scopes
        description: List of permissions that the user has granted for the app in
          this access token
        type: string
      - in: query
        name: subcode
        description: The error subcode for the error
        type: string
      - in: query
        name: user_id
        description: The ID of the user this access token is for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Debug
      - Token
      - Input
      - Token
      - Input
      - Token
  /&#123;doc-id&#125;:
    get:
      summary: Get Doc
      description: Doc
      operationId: getDoc
      x-api-path-slug: 123docid125-get
      parameters:
      - in: query
        name: can_deletebool
        description: Boolean, can document be deleted by viewerDefault
        type: string
      - in: query
        name: can_editbool
        description: Boolean, can document be edited by viewerDefault
        type: string
      - in: query
        name: created_timedatetime
        description: Timestamp of when the document was createdDefault
        type: string
      - in: query
        name: fromUser
        description: Author of the documentDefault
        type: string
      - in: query
        name: iconstring
        description: Image file for document iconDefault
        type: string
      - in: query
        name: idnumeric string
        description: The document ID
        type: string
      - in: query
        name: linkstring
        description: URL for the documentDefault
        type: string
      - in: query
        name: messagestring
        description: Content of the documentDefault
        type: string
      - in: query
        name: revisionid
        description: Current revision IDDefault
        type: string
      - in: query
        name: subjectstring
        description: Title of the documentDefault
        type: string
      - in: query
        name: updated_timedatetime
        description: Last updated timestampDefault
        type: string
      responses:
        200:
          description: OK
      tags:
      - Doc
  /&#123;domain-id&#125;:
    get:
      summary: Get Domain
      description: The Domain Insights dashboard and API is no longer available. This
        change effects all versions of this API. To see referral traffic for your
        website, and demographic details of your visitors, use Facebook Analytics
        instead. For more information, see Referral Insights with Facebook Analytics.
      operationId: getDomain
      x-api-path-slug: 123domainid125-get
      parameters:
      - in: query
        name: id
        description: The ID of the domain
        type: string
      - in: query
        name: name
        description: The name of the domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domain
  /&#123;event-id&#125;:
    get:
      summary: Get Event
      description: Event
      operationId: getEvent
      x-api-path-slug: 123eventid125-get
      parameters:
      - in: query
        name: attending_countint32
        description: Number of people attending the event
        type: string
      - in: query
        name: can_guests_invitebool
        description: Can guests invite friends
        type: string
      - in: query
        name: categorystring
        description: The category of the event
        type: string
      - in: query
        name: coverCoverPhoto
        description: Cover picture
        type: string
      - in: query
        name: declined_countint32
        description: Number of people who declined the event
        type: string
      - in: query
        name: descriptionstring
        description: Long-form descriptionDefault
        type: string
      - in: query
        name: end_timestring
        description: End time, if one has been setDefault
        type: string
      - in: query
        name: event_timeslistChildEvent
        description: Array of times of a multi-instance eventDefault
        type: string
      - in: query
        name: guest_list_enabledbool
        description: Can see guest list
        type: string
      - in: query
        name: idnumeric string
        description: The event ID
        type: string
      - in: query
        name: interested_countint32
        description: Number of people interested in the event
        type: string
      - in: query
        name: is_canceledbool
        description: Whether or not the event has been marked as canceled
        type: string
      - in: query
        name: is_draftbool
        description: Whether the event is in draft mode or published
        type: string
      - in: query
        name: is_page_ownedbool
        description: Whether the event is created by page or not
        type: string
      - in: query
        name: maybe_countint32
        description: Number of people who maybe going to the event
        type: string
      - in: query
        name: namestring
        description: Event nameDefault
        type: string
      - in: query
        name: noreply_countint32
        description: Number of people who did not reply to the event
        type: string
      - in: query
        name: owner
        description: The profile that created the event
        type: string
      - in: query
        name: parent_groupGroup
        description: The group the event belongs to
        type: string
      - in: query
        name: placePlace
        description: Event Place informationDefault
        type: string
      - in: query
        name: scheduled_publish_timestring
        description: Time when event is scheduled to be published
        type: string
      - in: query
        name: start_timestring
        description: Start timeDefault
        type: string
      - in: query
        name: ticketing_privacy_uristring
        description: URI to seller&#039;s privacy policy for ticket purchases
        type: string
      - in: query
        name: ticketing_terms_uristring
        description: URI to seller&#039;s terms of service for ticket purchases
        type: string
      - in: query
        name: ticket_uristring
        description: The link users can visit to buy a ticket to this event
        type: string
      - in: query
        name: ticket_uri_start_sales_timestring
        description: Time when tickets go on sale
        type: string
      - in: query
        name: timezoneenum
        description: Timezone
        type: string
      - in: query
        name: typeenum &#123;private, public, group, community&#125;
        description: The type of the event
        type: string
      - in: query
        name: updated_timedatetime
        description: Last update time (ISO 8601 formatted)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
  /&#123;friend-list-id&#125;:
    get:
      summary: Get Friend List
      description: Friend List
      operationId: getFriendList
      x-api-path-slug: 123friendlistid125-get
      parameters:
      - in: query
        name: idnumeric string
        description: The friend list IDDefault
        type: string
      - in: query
        name: list_typeenum
        description: The type of the friend listDefault
        type: string
      - in: query
        name: namestring
        description: The name of the friend listDefault
        type: string
      - in: query
        name: ownernumeric string
        description: The owner of the friend list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Friend
      - List
  /&#123;group-id&#125;/admins:
    get:
      summary: Get Group Admins
      description: This edge was deprecated on April 4th, 2018, and can no longer
        be used.
      operationId: getGroupAdmins
      x-api-path-slug: 123groupid125admins-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Admins
  /&#123;group-id&#125;/albums:
    get:
      summary: Get Group Albums
      description: The photo albums created for a Group.
      operationId: getGroupAlbums
      x-api-path-slug: 123groupid125albums-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Albums
  /me/albums:
    post:
      summary: Post Me Albums
      description: The photo albums created for a Group.
      operationId: postMeAlbums
      x-api-path-slug: mealbums-post
      parameters:
      - in: query
        name: message
        description: The description of the album, which will show up in news feed
          stories as the status message
        type: string
      - in: query
        name: name
        description: The name given to the album
        type: string
      - in: query
        name: Vector
        description: Vector
        type: string
      responses:
        200:
          description: OK
      tags:
      - Me
      - Albums
  /&#123;group-id&#125;/docs:
    get:
      summary: Get Group Docs
      description: The documents owned by a Group.
      operationId: getGroupDocs
      x-api-path-slug: 123groupid125docs-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Docs
  /&#123;group-id&#125;/events:
    get:
      summary: Get Group Events
      description: All events that belong to a group.
      operationId: getGroupEvents
      x-api-path-slug: 123groupid125events-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Events
  /&#123;group-id&#125;/feed:
    get:
      summary: Get Group Feed
      description: Posts owned by a Group, including status updates and links.
      operationId: getGroupFeed
      x-api-path-slug: 123groupid125feed-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Feed
    post:
      summary: Post Group Feed
      description: Posts owned by a Group, including status updates and links.
      operationId: postGroupFeed
      x-api-path-slug: 123groupid125feed-post
      parameters:
      - in: query
        name: link
        description: The URL of a link to attach to the post
        type: string
      - in: query
        name: message
        description: The main body of the post, otherwise called the status message
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - Feed
  /&#123;group-id&#125;/files:
    get:
      summary: Get Group Files
      description: The files uploaded to this group.
      operationId: getGroupFiles
      x-api-path-slug: 123groupid125files-get
      parameters:
      - in: query
        name: download_link
        description: URL to download the file
        type: string
      - in: query
        name: from
        description: This field was deprecated on April 4th, 2018
        type: string
      - in: query
        name: group
        description: The group the file is uploaded to (the same group as in the request)
        type: string
      - in: query
        name: id
        description: The ID of the file
        type: string
      - in: query
        name: message
        description: The text included with the file post
        type: string
      - in: query
        name: updated_time
        description: The last time the file was changed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - Files
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