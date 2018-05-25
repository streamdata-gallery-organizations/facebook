---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get Veo Copyright Rule
  description: Video Copyright Rule
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
  /&#123;group-id&#125;/members:
    get:
      summary: Get Group Members
      description: This edge was deprecated on April 4th, 2018, and can no longer
        be used.
      operationId: getGroupMembers
      x-api-path-slug: 123groupid125members-get
      parameters:
      - in: query
        name: administrator
        description: Whether or not the person is a group admin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - Members
  /&#123;group-id&#125;/videos:
    get:
      summary: Get Group Veos
      description: Videos owned by a Facebook Group.
      operationId: getGroupVeos
      x-api-path-slug: 123groupid125videos-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Veos
  /&#123;group-doc-id&#125;:
    get:
      summary: Get Group Doc
      description: Represents a doc within a Facebook group. The /&#123;group-doc-id&#125;
        node returns a single doc.
      operationId: getGroupDoc
      x-api-path-slug: 123groupdocid125-get
      parameters:
      - in: query
        name: can_delete
        description: Whether the session user can delete this doc (on Facebook
        type: string
      - in: query
        name: can_edit
        description: Whether the session user can edit this doc
        type: string
      - in: query
        name: created_time
        description: When the doc was created
        type: string
      - in: query
        name: from
        description: The profile that created this doc
        type: string
      - in: query
        name: icon
        description: The URL for the doc&#039;s icon
        type: string
      - in: query
        name: id
        description: The group doc ID
        type: string
      - in: query
        name: message
        description: The body of the doc
        type: string
      - in: query
        name: revision
        description: An ID representing the current doc revision
        type: string
      - in: query
        name: subject
        description: The title of the doc
        type: string
      - in: query
        name: updated_time
        description: The last time the doc was changed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - Doc
  /&#123;life-event-id&#125;:
    get:
      summary: Get Life Event
      description: Life Event
      operationId: getLifeEvent
      x-api-path-slug: 123lifeeventid125-get
      parameters:
      - in: query
        name: created_timedatetime
        description: The time when this milestone was publishedDefault
        type: string
      - in: query
        name: descriptionstring
        description: Description of the milestoneDefault
        type: string
      - in: query
        name: end_timedatetime
        description: The time when this milestone came to an endDefault
        type: string
      - in: query
        name: fromPage
        description: The information of the Page that ownes the milestoneDefault
        type: string
      - in: query
        name: idnumeric string
        description: The milestone IDDefault
        type: string
      - in: query
        name: is_hiddenbool
        description: Whether the milestone is hidden or notDefault
        type: string
      - in: query
        name: start_timedatetime
        description: The time when this milestone was startedDefault
        type: string
      - in: query
        name: titlestring
        description: The title of the milestoneDefault
        type: string
      - in: query
        name: updated_timedatetime
        description: The time when this milestone was updatedDefault
        type: string
      responses:
        200:
          description: OK
      tags:
      - Life
      - Event
  /&#123;link-id&#125;:
    get:
      summary: Get Link
      description: A link shared on Facebook.
      operationId: getLink
      x-api-path-slug: 123linkid125-get
      parameters:
      - in: query
        name: created_time
        description: The time the message was published
        type: string
      - in: query
        name: description
        description: A description of the link (appears beneath the link caption)
        type: string
      - in: query
        name: from
        description: The user that created the link
        type: string
      - in: query
        name: icon
        description: A URL to the link icon that Facebook displays in the news feed
        type: string
      - in: query
        name: id
        description: The link ID
        type: string
      - in: query
        name: link
        description: The URL that was shared
        type: string
      - in: query
        name: message
        description: The optional message from the user about this link
        type: string
      - in: query
        name: name
        description: The name of the link
        type: string
      - in: query
        name: picture
        description: A URL to the thumbnail image used in the link post
        type: string
      responses:
        200:
          description: OK
      tags:
      - Link
    delete:
      summary: Delete Link
      description: A link shared on Facebook.
      operationId: deleteLink
      x-api-path-slug: 123linkid125-delete
      responses:
        200:
          description: OK
      tags:
      - Link
  /&#123;live-video-id&#125;:
    get:
      summary: Get Live Veo
      description: Live Video
      operationId: getLiveVeo
      x-api-path-slug: 123livevideoid125-get
      parameters:
      - in: query
        name: ad_break_configLiveVideoAdBreakConfig
        description: The ad break configurations for clients implementing triggering
          an ad break ui
        type: string
      - in: query
        name: ad_break_failure_reasonenum
        description: Ad Break failure reason
        type: string
      - in: query
        name: broadcast_start_timedatetime
        description: The time the video was initially published
        type: string
      - in: query
        name: copyrightVideoCopyright
        description: The copyright information for the live video
        type: string
      - in: query
        name: creation_timedatetime
        description: The creation time of the live video
        type: string
      - in: query
        name: dash_preview_urlstring
        description: Preview URL for dash player
        type: string
      - in: query
        name: descriptionstring
        description: The description of the live video
        type: string
      - in: query
        name: embed_htmlstring
        description: The embed html of the live videoDefault
        type: string
      - in: query
        name: idnumeric string
        description: The live video ID
        type: string
      - in: query
        name: is_manual_modebool
        description: Whether schedule live is in manual mode, in which live video
          will start manually instead of on schedled time
        type: string
      - in: query
        name: is_reference_onlybool
        description: Whether the live video is exclusively used for copyright monitoring
        type: string
      - in: query
        name: live_viewsunsigned int32
        description: The instant viewer count of the live video now
        type: string
      - in: query
        name: permalink_urlstring
        description: The permalink URL of this video on Facebook
        type: string
      - in: query
        name: planned_start_timedatetime
        description: Planned start time for a live video
        type: string
      - in: query
        name: seconds_leftint32
        description: Seconds left in the maximum possible duration for this live video
        type: string
      - in: query
        name: secure_stream_urlstring
        description: The secure stream url of the live video
        type: string
      - in: query
        name: statusenum
        description: The status of the live videoDefault
        type: string
      - in: query
        name: stream_urlstring
        description: The stream url of the live videoDefault
        type: string
      - in: query
        name: titlestring
        description: The title of the live videoDefault
        type: string
      - in: query
        name: videoVideo
        description: The inside video of live video - only visible when the live video
          has ended
        type: string
      responses:
        200:
          description: OK
      tags:
      - Live
      - Veo
  /&#123;mailing-address-id&#125;:
    get:
      summary: Get Mailing Address
      description: Mailing Address
      operationId: getMailingAddress
      x-api-path-slug: 123mailingaddressid125-get
      parameters:
      - in: query
        name: citystring
        description: Address city nameDefault
        type: string
      - in: query
        name: city_pagePage
        description: Page representing the address city
        type: string
      - in: query
        name: countrystring
        description: Country of the addressDefault
        type: string
      - in: query
        name: idnumeric string
        description: The mailing address IDDefault
        type: string
      - in: query
        name: postal_codestring
        description: Postal code of the addressDefault
        type: string
      - in: query
        name: regionstring
        description: Region or state of the addressDefault
        type: string
      - in: query
        name: street1string
        description: Street addressDefault
        type: string
      - in: query
        name: street2string
        description: Second part of the street address - apt, suite, etcDefault
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mailing
      - Ress
  /&#123;message-id&#125;:
    get:
      summary: Get Message
      description: An individual message in Facebook Messenger.  This is a Pages-only
        endpoint.
      operationId: getMessage
      x-api-path-slug: 123messageid125-get
      parameters:
      - in: query
        name: created_time
        description: A timestamp of when this message was created
        type: string
      - in: query
        name: from
        description: The sender of this message
        type: string
      - in: query
        name: id
        description: The unique ID for this message
        type: string
      - in: query
        name: message
        description: The text of the message
        type: string
      - in: query
        name: subject
        description: The subject of the message
        type: string
      - in: query
        name: tags
        description: A set of tags indicating the message folder and source of the
          message
        type: string
      - in: query
        name: to
        description: A list of recipients of the message
        type: string
      responses:
        200:
          description: OK
      tags:
      - Message
  /&#123;message-id&#125;/attachments:
    get:
      summary: Get Message Attachments
      description: Files attached to a message. This is a Pages-only endpoint.
      operationId: getMessageAttachments
      x-api-path-slug: 123messageid125attachments-get
      parameters:
      - in: query
        name: id
        description: The attachment ID
        type: string
      - in: query
        name: mime_type
        description: The file MIME type
        type: string
      - in: query
        name: name
        description: The filename of the attachment
        type: string
      - in: query
        name: size
        description: The file size in bytes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Message
      - Attachments
  /&#123;message-id&#125;/shares:
    get:
      summary: Get Message Shares
      description: Shared items in a message. This is a Pages-only endpoint.
      operationId: getMessageShares
      x-api-path-slug: 123messageid125shares-get
      parameters:
      - in: query
        name: description
        description: The description of the shared item
        type: string
      - in: query
        name: id
        description: The shared item ID
        type: string
      - in: query
        name: link
        description: The URL to the shared item
        type: string
      - in: query
        name: name
        description: The title of the shared item
        type: string
      responses:
        200:
          description: OK
      tags:
      - Message
      - Shares
  /&#123;milestone-id&#125;:
    get:
      summary: Get Milestone
      description: This represents a milestone on a Facebook Page. The /&#123;milestone-id&#125;
        node returns a single &#039;milestone&#039;.
      operationId: getMilestone
      x-api-path-slug: 123milestoneid125-get
      parameters:
      - in: query
        name: created_time
        description: The creation time of the milestone
        type: string
      - in: query
        name: description
        description: The description of the milestone
        type: string
      - in: query
        name: end_time
        description: The end time of the milestone
        type: string
      - in: query
        name: from
        description: The Page that posted the milestone
        type: string
      - in: query
        name: id
        description: The ID of a milestone event
        type: string
      - in: query
        name: start_time
        description: The start time of the milestone
        type: string
      - in: query
        name: title
        description: The title of the milestone
        type: string
      - in: query
        name: updated_time
        description: The update time of the milestone
        type: string
      responses:
        200:
          description: OK
      tags:
      - Milestone
  offer:
    native:
      summary: Native Offer
      description: Native Offer
      operationId: nativeOffer
      x-api-path-slug: offer-native
      parameters:
      - in: query
        name: barcode_photostring
        description: Barcode image ID for in-store redemption
        type: string
      - in: query
        name: barcode_photo_uristring
        description: Barcode image URI for in-store redemption
        type: string
      - in: query
        name: barcode_typestring
        description: Barcode type for in-store redemption
        type: string
      - in: query
        name: barcode_valuestring
        description: Barcode value for in-store redemption
        type: string
      - in: query
        name: detailsstring
        description: Additional primary text describing the native offer
        type: string
      - in: query
        name: disable_locationbool
        description: Whether or not the location features, such as the map and nearby
          notification, are disabled
        type: string
      - in: query
        name: discountslistNativeOfferDiscount
        description: A structured representation of each part of the deal
        type: string
      - in: query
        name: expiration_timedatetime
        description: The time when the native offer expires, as a UNIX timestamp
        type: string
      - in: query
        name: idnumeric string
        description: The id of the native offer
        type: string
      - in: query
        name: instore_codestring
        description: The code used to redeem the native offer in-store
        type: string
      - in: query
        name: location_typeenum
        description: Where the offer may be redeemed
        type: string
      - in: query
        name: max_save_countinteger
        description: The maximum number of users who may save the native offer
        type: string
      - in: query
        name: online_codestring
        description: The code used to redeem the native offer online
        type: string
      - in: query
        name: pagePage
        description: The id of the page that owns the native offer
        type: string
      - in: query
        name: page_set_idstring
        description: The ID of Place Page Set which represents the locations where
          this in-store offer is valid for
        type: string
      - in: query
        name: redemption_linkstring
        description: The URL where the native offer may be redeemed
        type: string
      - in: query
        name: save_countinteger
        description: Number of users who have saved the native offer
        type: string
      - in: query
        name: termsstring
        description: Limitations, terms and conditions on the use of the native offer
        type: string
      - in: query
        name: titlestring
        description: The title of the native offerDefault
        type: string
      - in: query
        name: total_unique_codesstring
        description: Number of the unique codes/barcodes uploaded
        type: string
      - in: query
        name: unique_codesstring
        description: The fileId of the unique codes/barcodes file
        type: string
      - in: query
        name: unique_codes_file_code_typestring
        description: Code type of the unique codes/barcodes uploaded
        type: string
      - in: query
        name: unique_codes_file_namestring
        description: Name of the unique codes/barcodes uploaded
        type: string
      - in: query
        name: unique_codes_file_upload_statusstring
        description: The uploaded status of the unique codes/barcodes file
        type: string
      responses:
        200:
          description: OK
      tags:
      - Native
      - Offer
  /&#123;notification-id&#125;:
    get:
      summary: Get Notification
      description: An individual unread Facebook notification.  This is an API that&#039;s
        only available for Pages.
      operationId: getNotification
      x-api-path-slug: 123notificationid125-get
      parameters:
      - in: query
        name: application
        description: The app responsible for generating the notification
        type: string
      - in: query
        name: created_time
        description: When the notification was created
        type: string
      - in: query
        name: from
        description: The entity (user, page, app, etc
        type: string
      - in: query
        name: id
        description: The notification&#039;s id
        type: string
      - in: query
        name: link
        description: The URL that clicking on the notification would take someone
        type: string
      - in: query
        name: object
        description: The object (this can be a post, a photo, a comment, etc
        type: string
      - in: query
        name: title
        description: The message text in the notification
        type: string
      - in: query
        name: to
        description: The entity that received the notification
        type: string
      - in: query
        name: unread
        description: Indicates that the notification is unread
        type: string
      - in: query
        name: updated_time
        description: When the notification was last updated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Notification
  /&#123;open-graph-action-type-id&#125;:
    get:
      summary: Get Open Graph Action Type
      description: Open Graph Action Type
      operationId: getOpenGraphActionType
      x-api-path-slug: 123opengraphactiontypeid125-get
      parameters:
      - in: query
        name: allow_multiple_referencesbool
        description: Whether multiple objects can be referenced by the action
        type: string
      - in: query
        name: app_prepositionstring
        description: The preposition used to address the app
        type: string
      - in: query
        name: button_textstring
        description: Button text
        type: string
      - in: query
        name: descriptionstring
        description: Description
        type: string
      - in: query
        name: idnumeric string
        description: ID
        type: string
      - in: query
        name: is_app_secret_requiredbool
        description: Whether the app secret is required for API calls related to actions
          of this type
        type: string
      - in: query
        name: namestring
        description: NameDefault
        type: string
      - in: query
        name: object_typeslistid
        description: Object types associated with this action type
        type: string
      - in: query
        name: plural_paststring
        description: The plural past form of the action
        type: string
      - in: query
        name: plural_presentstring
        description: The plural present form of the action
        type: string
      - in: query
        name: property_configmapstring, OpenGraphPropertyConfig
        description: Per-property config
        type: string
      - in: query
        name: singular_paststring
        description: The singular past form of the action
        type: string
      - in: query
        name: singular_presentstring
        description: The singular present form of the action
        type: string
      - in: query
        name: tenses_disabledint32
        description: Bitmap of tenses that are disabled (the least significant bit
          relates to past tense, the second least significant relates to present tense
        type: string
      - in: query
        name: typestring
        description: TypeDefault
        type: string
      responses:
        200:
          description: OK
      tags:
      - Open
      - Graph
      - Action
      - Type
  /&#123;open-graph-context-id&#125;:
    get:
      summary: Get Open Graph Context
      description: Open Graph Context
      operationId: getOpenGraphContext
      x-api-path-slug: 123opengraphcontextid125-get
      parameters:
      - in: query
        name: idstring
        description: The token representing the social context
        type: string
      responses:
        200:
          description: OK
      tags:
      - Open
      - Graph
      - Context
  /&#123;open-graph-object-type-id&#125;:
    get:
      summary: Get Open Graph Object Type
      description: Open Graph Object Type
      operationId: getOpenGraphObjectType
      x-api-path-slug: 123opengraphobjecttypeid125-get
      parameters:
      - in: query
        name: articlestring
        description: An article for the type name
        type: string
      - in: query
        name: idnumeric string
        description: ID
        type: string
      - in: query
        name: namestring
        description: A noun representing the typeDefault
        type: string
      - in: query
        name: pluralstring
        description: The plural form of the object
        type: string
      - in: query
        name: property_configmapstring, OpenGraphPropertyConfig
        description: Per-property config
        type: string
      - in: query
        name: singularstring
        description: The singular form of the object
        type: string
      - in: query
        name: typestring
        description: Type nameDefault
        type: string
      responses:
        200:
          description: OK
      tags:
      - Open
      - Graph
      - Object
      - Type
  /&#123;page-admin-note-id&#125;:
    get:
      summary: Get Page Admin Note
      description: Page Admin Note
      operationId: getPageAdminNote
      x-api-path-slug: 123pageadminnoteid125-get
      parameters:
      - in: query
        name: bodystring
        description: Content of this note
        type: string
      - in: query
        name: fromPage
        description: Page that owns the note
        type: string
      - in: query
        name: idnumeric string
        description: ID of the tagDefault
        type: string
      - in: query
        name: userUser
        description: The user that this note is attached to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Page
      - Admin
      - Note
  /&#123;page-call-to-action-id&#125;:
    get:
      summary: Get Page Call To Action
      description: Page Call To Action
      operationId: getPageCallToAction
      x-api-path-slug: 123pagecalltoactionid125-get
      parameters:
      - in: query
        name: android_appApplication
        description: App that stores the destination info on Android
        type: string
      - in: query
        name: android_deeplinkstring
        description: Destination deeplink for the call-to-action on Android
        type: string
      - in: query
        name: android_destination_typeenum
        description: Destination type for the call-to-action on Android
        type: string
      - in: query
        name: android_package_namestring
        description: Destination app for the call-to-action on Android
        type: string
      - in: query
        name: android_urlstring
        description: Destination url for the call-to-action on Android
        type: string
      - in: query
        name: created_timedatetime
        description: Time when the call-to-action was created
        type: string
      - in: query
        name: email_addressstring
        description: Email address that can be contacted by a user
        type: string
      - in: query
        name: fromPage
        description: Page that owns the call-to-action
        type: string
      - in: query
        name: idnumeric string
        description: ID of the call-to-actionDefault
        type: string
      - in: query
        name: intl_number_with_plusstring
        description: International phone number with plus that can be called by a
          phone
        type: string
      - in: query
        name: iphone_appApplication
        description: App that stores the destination info on iPhone
        type: string
      - in: query
        name: iphone_deeplinkstring
        description: Destination deeplink for the call-to-action on iPhone
        type: string
      - in: query
        name: iphone_destination_typeenum
        description: Destination type for the call-to-action on iPhone
        type: string
      - in: query
        name: iphone_urlstring
        description: Destination url for the call-to-action on iPhone
        type: string
      - in: query
        name: statusenum
        description: Current running status of this actionDefault
        type: string
      - in: query
        name: typeenum
        description: The type of actionDefault
        type: string
      - in: query
        name: updated_timedatetime
        description: Time when the call-to-action was last updated
        type: string
      - in: query
        name: web_destination_typeenum
        description: Destination type for the call-to-action on desktop
        type: string
      - in: query
        name: web_urlstring
        description: Destination url for the call-to-action on desktop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Page
      - Call
      - Action
  /&#123;page-label-id&#125;:
    get:
      summary: Get Page Label
      description: Page Label
      operationId: getPageLabel
      x-api-path-slug: 123pagelabelid125-get
      parameters:
      - in: query
        name: creation_timedatetime
        description: Time when the label was created
        type: string
      - in: query
        name: creator_idProfile
        description: Admin who created the label
        type: string
      - in: query
        name: fromPage
        description: Page that owns the label
        type: string
      - in: query
        name: idnumeric string
        description: ID of the labelDefault
        type: string
      - in: query
        name: namestring
        description: Name of the labelDefault
        type: string
      responses:
        200:
          description: OK
      tags:
      - Page
      - Label
  /&#123;pages-platform-component-flow-service-config-id&#125;:
    get:
      summary: Get Pages Platform Component Flow Service Config
      description: Pages Platform Component Flow Service Config
      operationId: getPagesPlatformComponentFlowServiceConfig
      x-api-path-slug: 123pagesplatformcomponentflowserviceconfigid125-get
      parameters:
      - in: query
        name: deeplinkstring
        description: The deeplink to open the flow
        type: string
      - in: query
        name: flow_categoryenum
        description: The category of the flow
        type: string
      - in: query
        name: idnumeric string
        description: Id
        type: string
      - in: query
        name: labelstring
        description: The label of the entry point that enters the flow
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pages
      - Platform
      - Component
      - Flow
      - Service
      - Config
  /&#123;payment-id&#125;:
    get:
      summary: Get Payment
      description: The details of a payment made in an app using Facebook Payments.
      operationId: getPayment
      x-api-path-slug: 123paymentid125-get
      parameters:
      - in: query
        name: actions
        description: The list of different action types that have occurred in this
          payment
        type: string
      - in: query
        name: amount
        description: The amount of money covered by this action
        type: string
      - in: query
        name: application
        description: The app associated with this payment
        type: string
      - in: query
        name: country
        description: Buyer&#039;s ISO Country Code, for tax purposes
        type: string
      - in: query
        name: created_time
        description: The time the payment was originally created
        type: string
      - in: query
        name: currency
        description: The currency of the above amount in this action
        type: string
      - in: query
        name: disputes
        description: Contains the information related to a dispute,  including the
          user_comment and user_email which is provided by the consumer when the dispute
          is initiated
        type: string
      - in: query
        name: id
        description: The payment ID
        type: string
      - in: query
        name: items
        description: The items associated with the payment
        type: string
      - in: query
        name: payout_foreign_exchange_rate
        description: Exchange rate used to calculate payout amount which is remitted
          in USD
        type: string
      - in: query
        name: product
        description: The product URL of this item
        type: string
      - in: query
        name: quantity
        description: The number of this item purchased
        type: string
      - in: query
        name: reason
        description: The reason the developer or Facebook gave to resolve the dispute,
          after it has been resolved
        type: string
      - in: query
        name: request_id
        description: The unique, optional app-created identifier passed into the JS
          function (255 character maximum)
        type: string
      - in: query
        name: status
        description: The status for this particular action
        type: string
      - in: query
        name: tax
        description: The tax parameter specifies if a payment is subject to VAT and,
          if so, how the tax was paid
        type: string
      - in: query
        name: tax_amount
        description: The amount reduced from your payout for any taxes remitted by
          Facebook
        type: string
      - in: query
        name: tax_country
        description: The country determined by Facebook for tax calculation of this
          purchase, given as an ISO 3166-1 alpha-2 country code
        type: string
      - in: query
        name: test
        description: Optional parameter that shows up when a payment is made by a
          payment tester listed in the app&#039;s dashboard
        type: string
      - in: query
        name: time_created
        description: When this action occurred
        type: string
      - in: query
        name: time_updated
        description: When this action was last updated
        type: string
      - in: query
        name: type
        description: The type of this particular action
        type: string
      - in: query
        name: user
        description: The consumer&#039;s first and last name along with their user
          id
        type: string
      - in: query
        name: user_comment
        description: Comment provided by the consumer when the dispute is initiated
        type: string
      - in: query
        name: user_email
        description: Email provided by the consumer when the dispute is initiated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Payment
  /&#123;payment-id&#125;/dispute:
    post:
      summary: Post Payment Dispute
      description: Used to settle any payment disputes.
      operationId: postPaymentDisupdatee
      x-api-path-slug: 123paymentid125dispute-post
      parameters:
      - in: query
        name: reason
        description: The reason you are settling this dispute
        type: string
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Dispute
  /&#123;payment-id&#125;/refunds:
    post:
      summary: Post Payment Refunds
      description: Used to issue any payment refunds.
      operationId: postPaymentRefunds
      x-api-path-slug: 123paymentid125refunds-post
      parameters:
      - in: query
        name: amount
        description: The amount to refund
        type: string
      - in: query
        name: currency
        description: The three-letter ISO code of the currency in which the refund
          amount is specified; it must be the same as the currency in which the original
          purchase was denominated
        type: string
      - in: query
        name: reason
        description: The reason you are refunding this order
        type: string
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Refunds
  /&#123;place-tag-id&#125;:
    get:
      summary: Get Place Tag
      description: Place Tag
      operationId: getPlaceTag
      x-api-path-slug: 123placetagid125-get
      parameters:
      - in: query
        name: created_timedatetime
        description: Time when the place was visitedDefault
        type: string
      - in: query
        name: idnumeric string
        description: IDDefault
        type: string
      - in: query
        name: placePage
        description: The place that was visitedDefault
        type: string
      responses:
        200:
          description: OK
      tags:
      - Place
      - Tag
  /&#123;place-topic-id&#125;:
    get:
      summary: Get Place Topic
      description: Place Topic
      operationId: getPlaceTopic
      x-api-path-slug: 123placetopicid125-get
      parameters:
      - in: query
        name: countunsigned int32
        description: How many Pages have this category
        type: string
      - in: query
        name: has_childrenbool
        description: Whether there are subcategories of this category
        type: string
      - in: query
        name: icon_urlstring
        description: The URL for the icon representing this category
        type: string
      - in: query
        name: idnumeric string
        description: The topic ID
        type: string
      - in: query
        name: namestring
        description: Localized name of the categoryDefault
        type: string
      - in: query
        name: parent_idslistid
        description: IDs of any parent categories that this is a subcategory of
        type: string
      - in: query
        name: plural_namestring
        description: Localized plural name of the category
        type: string
      - in: query
        name: top_subtopic_namesliststring
        description: Names of the subtopics associated with the most pages
        type: string
      responses:
        200:
          description: OK
      tags:
      - Place
      - Topic
  /post-id:
    get:
      summary: Get Post
      description: An individual entry in a profile&#039;s feed. The profile could
        be a user, page, app, or group.
      operationId: getAdd
      x-api-path-slug: postid-get
      parameters:
      - in: query
        name: admin_creator
        description: The admin creator of a Page post
        type: string
      - in: query
        name: age_max
        description: Maximum age
        type: string
      - in: query
        name: age_min
        description: Must be 13 or higher
        type: string
      - in: query
        name: allow
        description: IfvalueisCUSTOM, this is a comma-separated ID list of users and
          friendlists (if any) that can see the post
        type: string
      - in: query
        name: application
        description: Information about the app this post was published by
        type: string
      - in: query
        name: call_to_action
        description: The call to action type used in any Page posts formobile app
          engagement ads
        type: string
      - in: query
        name: can_reply_privately
        description: Whether the Page viewer can send a private reply to this Post
        type: string
      - in: query
        name: caption
        description: Link caption in post that appears below name
        type: string
      - in: query
        name: cities
        description: Values of targeting cities
        type: string
      - in: query
        name: college_years
        description: Array of integers for graduation year from college
        type: string
      - in: query
        name: context
        description: The call to action type used in any Page posts formobile app
          engagement ads
        type: string
      - in: query
        name: countries
        description: Values of targeting countries
        type: string
      - in: query
        name: created_time
        description: The time the post was initially published
        type: string
      - in: query
        name: deny
        description: IfvalueisCUSTOM, this is a comma-separated ID list of users and
          friendlists (if any) that cannot see the post
        type: string
      - in: query
        name: description
        description: A description of a link in the post (appears beneath thecaption)
        type: string
      - in: query
        name: education_statuses
        description: Array of integers for targeting based on education level
        type: string
      - in: query
        name: feed_targeting
        description: Object that controlsnews feed targetingfor this post
        type: string
      - in: query
        name: friends
        description: IfvalueisCUSTOM, this indicates which group of friends can see
          the post
        type: string
      - in: query
        name: from
        description: Information (name and id) about the Profile that created the
          Post
        type: string
      - in: query
        name: full_picture
        description: URL to a full-sized version of the Photo published in the Post
          or scraped from a link in the Post
        type: string
      - in: query
        name: genders
        description: Target specific genders
        type: string
      - in: query
        name: href
        description: Any link associated with the property
        type: string
      - in: query
        name: icon
        description: A link to an icon representing the type of this post
        type: string
      - in: query
        name: id
        description: The post ID
        type: string
      - in: query
        name: instagram_eligibility
        description: Whether the post can be promoted on Instagram
        type: string
      - in: query
        name: interested_in
        description: Indicates targeting based on the &#039;interested in&#039; field
          of the user profile
        type: string
      - in: query
        name: interests
        description: One or more IDs of pages to target fans of pages
        type: string
      - in: query
        name: is_hidden
        description: If this post is marked as hidden (Applies to Pages only)
        type: string
      - in: query
        name: is_instagram_eligible
        description: Whether this post can be promoted in Instagram
        type: string
      - in: query
        name: is_published
        description: Indicates whether a scheduled post was published (applies to
          scheduled Page Post only, for users post and instantly published posts this
          value is alwaystrue)
        type: string
      - in: query
        name: length
        description: The length of the tag text, inunicode code points
        type: string
      - in: query
        name: link
        description: The link attached to this post
        type: string
      - in: query
        name: locales
        description: Targeted locales
        type: string
      - in: query
        name: message
        description: The status message in the post
        type: string
      - in: query
        name: message_tags
        description: An array of profiles tagged in themessagetext
        type: string
      - in: query
        name: name
        description: Name of the person, app or business
        type: string
      - in: query
        name: object_id
        description: The ID of any uploaded photo or video attached to the post
        type: string
      - in: query
        name: offset
        description: The location inunicode code pointsof the first character of the
          tag text in themessage
        type: string
      - in: query
        name: parent_id
        description: The ID of a parent post for this post, if it exists
        type: string
      - in: query
        name: permalink_url
        description: URL to the permalink page of the post
        type: string
      - in: query
        name: picture
        description: URL to a resized version of the Photo published in the Post or
          scraped from a link in the Post
        type: string
      - in: query
        name: place
        description: Any location information attached to the post
        type: string
      - in: query
        name: privacy
        description: The privacy settings of the post
        type: string
      - in: query
        name: promotable_id
        description: ID of post to use for promotion for stories that cannot be promoted
          directly
        type: string
      - in: query
        name: promotion_status
        description: Status of the promotion
        type: string
      - in: query
        name: properties
        description: A list of properties for any attached video, for example, the
          length of the video
        type: string
      - in: query
        name: regions
        description: Values of targeting regions
        type: string
      - in: query
        name: relationship_statuses
        description: Array of integers for targeting based on relationship status
        type: string
      - in: query
        name: shares
        description: The shares count of this post
        type: string
      - in: query
        name: source
        description: A URL to any Flash movie or video file attached to the post
        type: string
      - in: query
        name: status_type
        description: Description of the type of a status update
        type: string
      - in: query
        name: story
        description: Deprecated
        type: string
      - in: query
        name: story_tags
        description: Deprecated field, same asmessage_tags
        type: string
      - in: query
        name: targeting
        description: Object thatlimits the audiencefor this content
        type: string
      - in: query
        name: text
        description: The value of the property
        type: string
      - in: query
        name: to
        description: Profiles mentioned or targeted in this post
        type: string
      - in: query
        name: type
        description: The tagged profile&#039;s type
        type: string
      - in: query
        name: updated_time
        description: 'This field&#039;s behavior depends on the type of object the
          Post is on:'
        type: string
      - in: query
        name: value
        description: The actual privacy setting
        type: string
      - in: query
        name: with_tags
        description: Profiles tagged as being &#039;with&#039; the publisher of the
          post
        type: string
      responses:
        200:
          description: OK
      tags:
      - Posts
    delete:
      summary: Delete Post
      description: An individual entry in a profile&#039;s feed. The profile could
        be a user, page, app, or group.
      operationId: deleteAdd
      x-api-path-slug: postid-delete
      responses:
        200:
          description: OK
      tags:
      - Posts
    post:
      summary: Add Post
      description: An individual entry in a profile&#039;s feed. The profile could
        be a user, page, app, or group.
      operationId: postAdd
      x-api-path-slug: postid-post
      responses:
        200:
          description: OK
      tags:
      - Posts
  /&#123;post-id&#125;/attachments:
    get:
      summary: Get Add Attachments
      description: 'Media content associated with a story or comment. Story attachments
        are accessed from the following endpoints:'
      operationId: getAddAttachments
      x-api-path-slug: 123postid125attachments-get
      parameters:
      - in: query
        name: description
        description: Text accompanying the attachment
        type: string
      - in: query
        name: description_tags
        description: Profiles tagged in the text accompanying the attachment
        type: string
      - in: query
        name: title
        description: Title of the attachment
        type: string
      - in: query
        name: type
        description: Type of the attachment
        type: string
      - in: query
        name: url
        description: URL of the attachment
        type: string
      - in: query
        name: Vector
        description: Vector
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attachments
  /&#123;promotion-info-id&#125;:
    get:
      summary: Get Promotion Info
      description: Promotion Info
      operationId: getPromotionInfo
      x-api-path-slug: 123promotioninfoid125-get
      parameters:
      - in: query
        name: budgetunsigned int32
        description: The budget for the promoted post
        type: string
      - in: query
        name: currencystring
        description: The currency used for the promotion
        type: string
      - in: query
        name: spentunsigned int32
        description: The amount spent promoting this post so far
        type: string
      responses:
        200:
          description: OK
      tags:
      - Promotion
      - Info
  /&#123;rtb-dynamic-post-id&#125;:
    get:
      summary: Get Rtb Dynamic Add
      description: Rtb Dynamic Post
      operationId: getRtbDynamicAdd
      x-api-path-slug: 123rtbdynamicpostid125-get
      parameters:
      - in: query
        name: child_attachmentslistDynamicPostChildAttachment
        description: List of child cards for carousel posts
        type: string
      - in: query
        name: createddatetime
        description: The time this post was made
        type: string
      - in: query
        name: descriptionstring
        description: The link description
        type: string
      - in: query
        name: idnumeric string
        description: The dynamic post IDDefault
        type: string
      - in: query
        name: image_urlstring
        description: The dynamic post image
        type: string
      - in: query
        name: linkstring
        description: The dynamic post link
        type: string
      - in: query
        name: messagestring
        description: The post text
        type: string
      - in: query
        name: owner_idnumeric string
        description: The ID of the owner of this post
        type: string
      - in: query
        name: place_idnumeric string
        description: The place page ID of the dynamic post
        type: string
      - in: query
        name: product_idnumeric string
        description: The product ID
        type: string
      - in: query
        name: titlestring
        description: The title of the dynamic post
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rtb
      - Dynamic
  /&#123;request-id&#125;:
    get:
      summary: Get Request
      description: An individual game request received by someone, sent by an app
        or by another person.
      operationId: getRequest
      x-api-path-slug: 123requestid125-get
      parameters:
      - in: query
        name: application
        description: App associated with the request
        type: string
      - in: query
        name: created_time
        description: Timestamp when the request was created
        type: string
      - in: query
        name: from
        description: The sender associated with the request
        type: string
      - in: query
        name: id
        description: The request object ID
        type: string
      - in: query
        name: message
        description: A string describing the request
        type: string
      - in: query
        name: to
        description: The recipient of the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Request
    delete:
      summary: Delete Request
      description: An individual game request received by someone, sent by an app
        or by another person.
      operationId: deleteRequest
      x-api-path-slug: 123requestid125-delete
      responses:
        200:
          description: OK
      tags:
      - Request
  /&#123;sales-promo-id&#125;:
    get:
      summary: Get Sales Promo
      description: Offer
      operationId: getSalesPromo
      x-api-path-slug: 123salespromoid125-get
      parameters:
      - in: query
        name: availability_locationenum
        description: Where an offer can be redeemed (online/offline/both)
        type: string
      - in: query
        name: descriptionstring
        description: The description of the offer
        type: string
      - in: query
        name: destination_uristring
        description: A link to the offer page on the company website
        type: string
      - in: query
        name: discount_codestring
        description: The offer code providing the discount
        type: string
      - in: query
        name: expiration_timedatetime
        description: The time after which this offer is no longer valid
        type: string
      - in: query
        name: idnumeric string
        description: The ID of the offer
        type: string
      - in: query
        name: pagePage
        description: The page on which the offer is published
        type: string
      - in: query
        name: schedule_timedatetime
        description: The time which the offer is scheduled to be published
        type: string
      - in: query
        name: start_timedatetime
        description: The time which the offer starts
        type: string
      - in: query
        name: terms_and_conditionsstring
        description: The legal terms and conditions of the offer
        type: string
      - in: query
        name: titlestring
        description: The title of the offer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Promo
  /&#123;saved-message-response-id&#125;:
    get:
      summary: Get Saved Message Response
      description: Saved Message Response
      operationId: getSavedMessageResponse
      x-api-path-slug: 123savedmessageresponseid125-get
      parameters:
      - in: query
        name: categorystring
        description: The message category of the saved response,Default
        type: string
      - in: query
        name: idnumeric string
        description: The ID of the saved responseDefault
        type: string
      - in: query
        name: imagestring
        description: The image attached to this save response
        type: string
      - in: query
        name: is_enabledbool
        description: Toggle whether to enable the messageDefault
        type: string
      - in: query
        name: messagestring
        description: The message body of the saved responseDefault
        type: string
      - in: query
        name: titlestring
        description: The title of the saved response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Message
      - Response
  /&#123;status-id&#125;:
    get:
      summary: Get Status
      description: A status message in a profile&#039;s feed.
      operationId: getStatus
      x-api-path-slug: 123statusid125-get
      parameters:
      - in: query
        name: event
        description: Event associated with this status, if any
        type: string
      - in: query
        name: from
        description: The user who posted the message
        type: string
      - in: query
        name: id
        description: The status message ID
        type: string
      - in: query
        name: message
        description: The status message content
        type: string
      - in: query
        name: name
        description: The name of the Profile, e
        type: string
      - in: query
        name: place
        description: Location associated with this status, if any
        type: string
      - in: query
        name: updated_time
        description: The time the message was published
        type: string
      responses:
        200:
          description: OK
      tags:
      - Status
  /&#123;from.id&#125;_&#123;status-id&#125;:
    delete:
      summary: Delete From. Status
      description: A status message in a profile&#039;s feed.
      operationId: deleteFrom.Status
      x-api-path-slug: 123from-id125-123statusid125-delete
      responses:
        200:
          description: OK
      tags:
      - From.
      - Status
    post:
      summary: Post From. Status
      description: A status message in a profile&#039;s feed.
      operationId: postFrom.Status
      x-api-path-slug: 123from-id125-123statusid125-post
      responses:
        200:
          description: OK
      tags:
      - From.
      - Status
  /&#123;test-user-id&#125;:
    post:
      summary: Post Test User
      description: A test user associated with a Facebook app. Test users are created
        and associated using the /&#123;app-id&#125;/accounts/test-users edge or in
        the App Dashboard.
      operationId: postTestUser
      x-api-path-slug: 123testuserid125-post
      parameters:
      - in: query
        name: name
        description: New name for the test user
        type: string
      - in: query
        name: password
        description: A new password for the test user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Test
      - User
    delete:
      summary: Delete Test User
      description: A test user associated with a Facebook app. Test users are created
        and associated using the /&#123;app-id&#125;/accounts/test-users edge or in
        the App Dashboard.
      operationId: deleteTestUser
      x-api-path-slug: 123testuserid125-delete
      responses:
        200:
          description: OK
      tags:
      - Test
      - User
  /&#123;test-user-1&#125;/friends/&#123;test-user-2&#125;:
    post:
      summary: Post Test User 1 Friends Test User 2
      description: The friends of a test user. This is identical to the /&#123;user-id&#125;/friends
        edge aside from the publishing operation explained below.
      operationId: postTestUser1FriendsTestUser2
      x-api-path-slug: 123testuser1125friends123testuser2125-post
      responses:
        200:
          description: OK
      tags:
      - Test
      - User
      - "1"
      - Friends
      - Test
      - User
      - "2"
  /&#123;thread-id&#125;:
    get:
      summary: Get Thread
      description: A Facebook Messages conversation thread. This endpoint is only
        accessible for users that are developers of the app making the request. Pages
        should use the Conversation object.
      operationId: getThread
      x-api-path-slug: 123threadid125-get
      parameters:
      - in: query
        name: comments
        description: The messages in this thread
        type: string
      - in: query
        name: id
        description: The unique ID for this message thread
        type: string
      - in: query
        name: to
        description: Profiles that are subscribed to the thread
        type: string
      - in: query
        name: unread
        description: The amount of messages that are unread by the session profile
        type: string
      - in: query
        name: unseen
        description: The amount of messages that are unseen by the session profile
        type: string
      - in: query
        name: updated_time
        description: When the thread was last updated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Thread
  /&#123;user-id&#125;:
    get:
      summary: Get User
      description: User
      operationId: getUser
      x-api-path-slug: 123userid125-get
      parameters:
      - in: query
        name: aboutstring
        description: Returns no data as of April 4, 2018
        type: string
      - in: query
        name: addressLocation
        description: The person&#039;s address
        type: string
      - in: query
        name: admin_noteslistPageAdminNote
        description: Notes added by viewing page on this person
        type: string
      - in: query
        name: age_rangeAgeRange
        description: The age segment for this person expressed as a minimum and maximum
          age
        type: string
      - in: query
        name: birthdaystring
        description: The person&#039;s birthday
        type: string
      - in: query
        name: contextUserContext
        description: Social context for this person
        type: string
      - in: query
        name: coverUserCoverPhoto
        description: The person&#039;s cover photo
        type: string
      - in: query
        name: currencyCurrency
        description: The person&#039;s local currency information
        type: string
      - in: query
        name: deviceslistUserDevice
        description: The list of devices the person is using
        type: string
      - in: query
        name: educationlistEducationExperience
        description: Returns no data as of April 4, 2018
        type: string
      - in: query
        name: emailstring
        description: The person&#039;s primary email address listed on their profile
        type: string
      - in: query
        name: employee_numberstring
        description: The person&#039;s employee number, as set by the company via
          SCIM API
        type: string
      - in: query
        name: favorite_athleteslistExperience
        description: Athletes the person likes
        type: string
      - in: query
        name: favorite_teamslistExperience
        description: Sports teams the person likes
        type: string
      - in: query
        name: first_namestring
        description: The person&#039;s first nameCore
        type: string
      - in: query
        name: genderstring
        description: The gender selected by this person, male or female
        type: string
      - in: query
        name: hometownPage
        description: The person&#039;s hometown
        type: string
      - in: query
        name: idnumeric string
        description: The id of this person&#039;s user account
        type: string
      - in: query
        name: inspirational_peoplelistExperience
        description: The person&#039;s inspirational people
        type: string
      - in: query
        name: installedbool
        description: Is the app making the request installed?
        type: string
      - in: query
        name: install_typeenum
        description: Install type
        type: string
      - in: query
        name: interested_inliststring
        description: Returns no data as of April 4, 2018
        type: string
      - in: query
        name: is_shared_loginbool
        description: Is this a shared login (e
        type: string
      - in: query
        name: is_verifiedbool
        description: People with large numbers of followers can have the authenticity
          of their identity manually verified by Facebook
        type: string
      - in: query
        name: labelslistPageLabel
        description: Labels applied by viewing page on this person
        type: string
      - in: query
        name: languageslistExperience
        description: Facebook Pages representing the languages this person knows
        type: string
      - in: query
        name: last_namestring
        description: The person&#039;s last nameCore
        type: string
      - in: query
        name: linkstring
        description: A link to the person&#039;s TimelineCore
        type: string
      - in: query
        name: localestring
        description: The person&#039;s localeCore
        type: string
      - in: query
        name: local_news_megaphone_dismiss_statusbool
        description: Display megaphone for local news bookmarkDeprecated
        type: string
      - in: query
        name: local_news_subscription_statusbool
        description: Daily local news notificationDeprecated
        type: string
      - in: query
        name: locationPage
        description: The person&#039;s current location as entered by them on their
          profile
        type: string
      - in: query
        name: meeting_forliststring
        description: What the person is interested in meeting for
        type: string
      - in: query
        name: middle_namestring
        description: The person&#039;s middle nameCore
        type: string
      - in: query
        name: namestring
        description: The person&#039;s full nameCoreDefault
        type: string
      - in: query
        name: name_formatstring
        description: The person&#039;s name formatted to correctly handle Chinese,
          Japanese, or Korean ordering
        type: string
      - in: query
        name: payment_pricepointsPaymentPricepoints
        description: The person&#039;s payment pricepoints
        type: string
      - in: query
        name: politicalstring
        description: Returns no data as of April 4, 2018
        type: string
      - in: query
        name: public_keystring
        description: The person&#039;s PGP public key
        type: string
      - in: query
        name: quotesstring
        description: The person&#039;s favorite quotes
        type: string
      - in: query
        name: relationship_statusstring
        description: Returns no data as of April 4, 2018
        type: string
      - in: query
        name: religionstring
        description: Returns no data as of April 4, 2018
        type: string
      - in: query
        name: security_settingsSecuritySettings
        description: Security settings
        type: string
      - in: query
        name: shared_login_upgrade_required_bydatetime
        description: The time that the shared loginneeds to be upgraded to Business
          Manager by
        type: string
      - in: query
        name: significant_otherUser
        description: The person&#039;s significant other
        type: string
      - in: query
        name: sportslistExperience
        description: Sports played by the person
        type: string
      - in: query
        name: test_groupunsigned int32
        description: Platform test group
        type: string
      - in: query
        name: third_party_idstring
        description: A string containing an anonymous, but unique identifier for the
          person
        type: string
      - in: query
        name: 'timezonefloat (min: -24) (max: 24)'
        description: The person&#039;s current timezone offset from UTCCore
        type: string
      - in: query
        name: token_for_businessstring
        description: A token that is the same across a business&#039;s apps
        type: string
      - in: query
        name: updated_timedatetime
        description: Updated time
        type: string
      - in: query
        name: verifiedbool
        description: Indicates whether the account has been verified
        type: string
      - in: query
        name: video_upload_limitsVideoUploadLimits
        description: Video upload limits
        type: string
      - in: query
        name: viewer_can_send_giftbool
        description: Can the viewer send a gift to this person?
        type: string
      - in: query
        name: websitestring
        description: Returns no data as of April 4, 2018
        type: string
      - in: query
        name: worklistWorkExperience
        description: Returns no data as of April 4, 2018
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
  /&#123;user-context-id&#125;:
    get:
      summary: Get User Context
      description: User Context
      operationId: getUserContext
      x-api-path-slug: 123usercontextid125-get
      parameters:
      - in: query
        name: idstring
        description: The token representing the social context
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Context
  /&#123;video-id&#125;:
    get:
      summary: Get Veo
      description: Video
      operationId: getVeo
      x-api-path-slug: 123videoid125-get
      parameters:
      - in: query
        name: ad_breakslistinteger
        description: Time offsets of ad breaks in milliseconds
        type: string
      - in: query
        name: backdated_timedatetime
        description: The time when the video post was created
        type: string
      - in: query
        name: backdated_time_granularityenum
        description: Accuracy of the backdated time
        type: string
      - in: query
        name: content_categoryenum
        description: The content category of this video
        type: string
      - in: query
        name: content_tagslistnumeric string
        description: Tags that describe the contents of the video
        type: string
      - in: query
        name: created_timedatetime
        description: The time the video was initially published
        type: string
      - in: query
        name: custom_labelsliststring
        description: Labels used to describe the video
        type: string
      - in: query
        name: descriptionstring
        description: The description of the video
        type: string
      - in: query
        name: embeddablebool
        description: Whether the video is embeddable
        type: string
      - in: query
        name: embed_htmlstring
        description: The HTML element that may be embedded in a Web page to play the
          video
        type: string
      - in: query
        name: eventEvent
        description: event
        type: string
      - in: query
        name: formatlistVideoFormat
        description: The different formats of the video
        type: string
      - in: query
        name: fromUser|Page
        description: The profile that created the video
        type: string
      - in: query
        name: iconstring
        description: The icon that Facebook displays when videos are published to
          the feed
        type: string
      - in: query
        name: idnumeric string
        description: The video ID
        type: string
      - in: query
        name: is_crossposting_eligiblebool
        description: Specifies if the video is eligible for crossposting
        type: string
      - in: query
        name: is_crosspost_videobool
        description: Whether the video is crossposted from other page
        type: string
      - in: query
        name: is_instagram_eligiblebool
        description: Whether the video is eligible to be promoted on Instagram
        type: string
      - in: query
        name: lengthfloat
        description: Duration of this video in seconds
        type: string
      - in: query
        name: live_statusenum
        description: The live status of the video
        type: string
      - in: query
        name: permalink_urlstring
        description: URL to the permalink page of the video
        type: string
      - in: query
        name: picturestring
        description: The URL for the thumbnail picture of the video
        type: string
      - in: query
        name: placePlace
        description: Location associated with the video, if any
        type: string
      - in: query
        name: privacyPrivacy
        description: Privacy setting for the video
        type: string
      - in: query
        name: publishedbool
        description: Whether a post about this video is published
        type: string
      - in: query
        name: scheduled_publish_timedatetime
        description: The time that the video is scheduled to publish
        type: string
      - in: query
        name: sourcestring
        description: A URL to the raw, playable video file
        type: string
      - in: query
        name: statusVideoStatus
        description: Object describing the status attributes of a video
        type: string
      - in: query
        name: titlestring
        description: The video title or caption
        type: string
      - in: query
        name: universal_video_idstring
        description: The publishers asset management code for this video
        type: string
      - in: query
        name: updated_timedatetime
        description: The last time the video or its caption was updated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Veo
  /&#123;video-copyright-rule-id&#125;:
    get:
      summary: Get Veo Copyright Rule
      description: Video Copyright Rule
      operationId: getVeoCopyrightRule
      x-api-path-slug: 123videocopyrightruleid125-get
      parameters:
      - in: query
        name: condition_groupslistVideoCopyrightConditionGroup
        description: Groups of conditions on the rules objectDefault
        type: string
      - in: query
        name: copyrightslistnumeric string
        description: Copyrights associated with this copyright rules object
        type: string
      - in: query
        name: created_datedatetime
        description: The date on which the rule was created
        type: string
      - in: query
        name: creatorUser
        description: The person who created the match rule
        type: string
      - in: query
        name: idnumeric string
        description: The id of video copyright rules objectDefault
        type: string
      - in: query
        name: is_in_migrationbool
        description: Whether or not the rule is in migration
        type: string
      - in: query
        name: namestring
        description: Name of the video copyright rules objectDefault
        type: string
      responses:
        200:
          description: OK
      tags:
      - Veo
      - Copyright
      - Rule
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