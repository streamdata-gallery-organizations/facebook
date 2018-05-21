{
  "info": {
    "name": "Facebook Delete Me Scores",
    "_postman_id": "bbb363bf-87e6-44b6-b22f-887407182310",
    "description": "As of April 4, 2018, this endpoint only returns an empty data set. Please see the changelog for more information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Object",
      "item": [
        {
          "id": "455c4b0c-ba3f-42b3-be94-176356a52e19",
          "name": "getObjectComments",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;object-id&#125;/comments?order=order&total_count=total_count",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This reference describes the /comments edge that is common to multiple Graph API nodes. The structure and operations are the same for each node. The following objects has a /comments edge:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53225e63-28e2-45ba-a7c6-c052cc7acca1"
            }
          ]
        },
        {
          "id": "00b46fcc-68d2-4488-97d2-1ea5573b7352",
          "name": "postObjectComments",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;object-id&#125;/comments?attachment_id=attachment_id&attachment_url=attachment_url&message=message&source=source",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "This reference describes the /comments edge that is common to multiple Graph API nodes. The structure and operations are the same for each node. The following objects has a /comments edge:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67f94532-3f54-4c1f-9974-8c5516ddd485"
            }
          ]
        },
        {
          "id": "077d9881-8447-4731-bbc0-943e25374c50",
          "name": "getObjectLikes",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;object-id&#125;/likes?total_count=total_count",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This reference describes the /likes edge that is common to multiple Graph API nodes. The structure and operations are the same for each node, except that for the following nodes, /likes returns only the profile for the current user if read with a user access token:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b1c0b7e-cb04-412a-a40e-117f7af39278"
            }
          ]
        },
        {
          "id": "2e9c3135-0ad3-4cea-9bc7-8dc6f34bc36c",
          "name": "postObjectLikes",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;object-id&#125;/likes",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "This reference describes the /likes edge that is common to multiple Graph API nodes. The structure and operations are the same for each node, except that for the following nodes, /likes returns only the profile for the current user if read with a user access token:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aab5040f-6bf5-414f-a19b-1dfa5411bf23"
            }
          ]
        },
        {
          "id": "df472ece-ad39-4eee-9b75-71dbd7882a53",
          "name": "deleteObjectLikes",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;object-id&#125;/likes",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "This reference describes the /likes edge that is common to multiple Graph API nodes. The structure and operations are the same for each node, except that for the following nodes, /likes returns only the profile for the current user if read with a user access token:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79dce395-3c65-481e-a1a8-0aaed1796935"
            }
          ]
        },
        {
          "id": "fe7298a9-a9b1-44b6-a06e-8799d32e3a95",
          "name": "getObjectSharedadds",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;object-id&#125;/sharedposts",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The /sharedposts edge that is common to multiple Graph API nodes. The structure and operations are the same for each node."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b652324b-c473-4a02-bb18-ae8cea63554a"
            }
          ]
        },
        {
          "id": "14a00fd9-9af1-44d6-826b-3db977c77862",
          "name": "postObjectPrivateReplies",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;object-id&#125;/private_replies?id=id&message=message",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "This edge allows Pages to reply to Post Comments and Visitor Posts with a private Message. It can be used with the following nodes:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4db165be-c410-4121-8119-f18742cc99f6"
            }
          ]
        }
      ]
    },
    {
      "name": "Achievement",
      "item": [
        {
          "id": "811031f2-6e73-42e9-aabf-cd57adeaeee1",
          "name": "getAchievementType",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;achievement-type-id&#125;?application=application&context=context&created_time=created_time&data=data&description=description&height=height&id=id&image=image&is_scraped=is_scraped&points=points&title=title&type=type&updated_time=updated_time&url=url&width=width",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A games achievement type created by a Facebook App. Not to be confused with an instance of an achievement."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "836fd734-aef9-462c-8c8a-3b044a60e507"
            }
          ]
        }
      ]
    },
    {
      "name": "Album",
      "item": [
        {
          "id": "61b79dbf-4c86-4711-973e-64fdc3517dd9",
          "name": "getAlbum",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;album-id&#125;?can_upload=can_upload&count=count&cover_photo=cover_photo&created_time=created_time&description=description&event=event&from=from&id=id&link=link&location=location&name=name&place=place&privacy=privacy&type=type&updated_time=updated_time",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents a photo album. The /&#123;album-id&#125; node returns a single album."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c5690e6-de76-4a11-bf3d-2c96d7b23686"
            }
          ]
        },
        {
          "id": "2d5eea4f-9622-474a-b96d-776929a68de3",
          "name": "getAlbumPicture",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;album-id&#125;/picture",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The cover photo of a photo album."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21f483f1-07f0-45e6-af62-96bbb0d5322a"
            }
          ]
        },
        {
          "id": "bf6a9c69-fcde-4182-8af7-05f622134f64",
          "name": "getAlbumPhotos",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;album-id&#125;/photos",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The photos in an album on Facebook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64d5e82c-9546-4d08-a09f-b025a609981e"
            }
          ]
        }
      ]
    },
    {
      "name": "Canvas",
      "item": [
        {
          "id": "7a4b4a3d-5d2b-4ce0-bdc7-fa7d4ad036e0",
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
              "id": "afbf9a57-9890-4574-af70-40329195f6aa"
            }
          ]
        },
        {
          "id": "bd7ffe98-d39d-421a-8480-aa09427c3433",
          "name": "getCanvas",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;canvas-id&#125;?background_colorstring=background_colorstring&body_elementslistCanvasPhoto|CanvasHeader|CanvasVideo|CanvasText|CanvasCarousel|CanvasButton|CanvasFooter|CanvasStoreLocator|CanvasProductList|CanvasProductSet|CanvasLeadForm=body_elementslistCanvasPhoto%7CCanvasHeader%7CCanvasVideo%7CCanvasText%7CCanvasCarousel%7CCanvasButton%7CCanvasFooter%7CCanvasStoreLocator%7CCanvasProductList%7CCanvasProductSet%7CCanvasLeadForm&canvas_linkstring=canvas_linkstring&idnumeric string=idnumeric%20string&is_hiddenbool=is_hiddenbool&is_publishedbool=is_publishedbool&last_editorUser=last_editorUser&namestring=namestring&ownerPage=ownerPage&update_timeint32=update_timeint32",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Canvas"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7b20212-b43a-476c-bc5a-751016044282"
            }
          ]
        },
        {
          "id": "333ececa-13d2-4ff9-8af9-50893a0638eb",
          "name": "getCanvasButton",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;canvas-button-id&#125;?actionCanvasOpenURLAction=actionCanvasOpenURLAction&background_colorstring=background_colorstring&bottom_paddingnumeric string=bottom_paddingnumeric%20string&button_colorstring=button_colorstring&button_styleenum=button_styleenum&deep_linkstring=deep_linkstring&element_group_keystring=element_group_keystring&element_typeenum=element_typeenum&font_familystring=font_familystring&font_sizenumeric string=font_sizenumeric%20string&idnumeric string=idnumeric%20string&line_heightnumeric string=line_heightnumeric%20string&namestring=namestring&rich_textCanvasRichText=rich_textCanvasRichText&text_alignmentenum=text_alignmentenum&text_colorstring=text_colorstring&top_paddingnumeric string=top_paddingnumeric%20string",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Canvas Button"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77a58cde-0961-4d9c-9121-92ef1a508eca"
            }
          ]
        },
        {
          "id": "e573ef4b-f234-4aea-99c1-70eb814d5535",
          "name": "getCanvasCarousel",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;canvas-carousel-id&#125;?bottom_paddingnumeric string=bottom_paddingnumeric%20string&child_elementslistCanvasPhoto=child_elementslistCanvasPhoto&element_group_keystring=element_group_keystring&element_typeenum=element_typeenum&idnumeric string=idnumeric%20string&namestring=namestring&styleenum=styleenum&top_paddingnumeric string=top_paddingnumeric%20string",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Canvas Carousel"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3965c50-7b92-438e-9d8a-bf3e9f89f1b4"
            }
          ]
        },
        {
          "id": "6ee495b2-9f05-403e-9282-4e9bbd327427",
          "name": "getCanvasFooter",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;canvas-footer-id&#125;?background_colorstring=background_colorstring&bottom_paddingnumeric string=bottom_paddingnumeric%20string&child_elementslistCanvasButton=child_elementslistCanvasButton&element_group_keystring=element_group_keystring&element_typeenum=element_typeenum&idnumeric string=idnumeric%20string&namestring=namestring&top_paddingnumeric string=top_paddingnumeric%20string",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Canvas Footer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cbeb4fd-deb7-4f3c-a95d-5e7d06820ceb"
            }
          ]
        },
        {
          "id": "9e62a195-3fed-4456-92b2-0cd3a7a16b6e",
          "name": "getCanvasHeader",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;canvas-header-id&#125;?background_colorstring=background_colorstring&bottom_paddingnumeric string=bottom_paddingnumeric%20string&child_elementslistCanvasPhoto=child_elementslistCanvasPhoto&element_group_keystring=element_group_keystring&element_typeenum=element_typeenum&idnumeric string=idnumeric%20string&namestring=namestring&top_paddingnumeric string=top_paddingnumeric%20string",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Canvas Header"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db90f915-bd48-4b93-a3f2-0f350a787535"
            }
          ]
        },
        {
          "id": "b7c59ee9-fc72-4846-a331-4186db25fb74",
          "name": "getCanvasPhoto",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;canvas-photo-id&#125;?actionCanvasOpenURLAction=actionCanvasOpenURLAction&bottom_paddingnumeric string=bottom_paddingnumeric%20string&deep_linkstring=deep_linkstring&element_group_keystring=element_group_keystring&element_typeenum=element_typeenum&hide_product_pricesbool=hide_product_pricesbool&idnumeric string=idnumeric%20string&namestring=namestring&photoPhoto=photoPhoto&product_tagslistCanvasProductTag=product_tagslistCanvasProductTag&styleenum=styleenum&top_paddingnumeric string=top_paddingnumeric%20string",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Canvas Photo"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79a66504-6eb4-48b1-aeeb-ddb03c55d8fe"
            }
          ]
        },
        {
          "id": "bb74bb24-89f6-4570-b7ba-6d477269d5f7",
          "name": "getCanvasProductSet",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;canvas-product-set-id&#125;?bottom_paddingnumeric string=bottom_paddingnumeric%20string&element_group_keystring=element_group_keystring&element_typeenum=element_typeenum&idnumeric string=idnumeric%20string&image_overlay_specAdCreativeLinkDataImageOverlaySpec=image_overlay_specAdCreativeLinkDataImageOverlaySpec&item_descriptionstring=item_descriptionstring&item_headlinestring=item_headlinestring&max_productsunsigned int32=max_productsunsigned%20int32&namestring=namestring&product_set_idnumeric string=product_set_idnumeric%20string&retailer_item_idsstring=retailer_item_idsstring&show_in_feedbool=show_in_feedbool&top_paddingnumeric string=top_paddingnumeric%20string",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Canvas Product Set"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d689622b-c2a5-4576-ba0b-3f8198e5913d"
            }
          ]
        },
        {
          "id": "a4d09d59-642b-42ae-a460-c21e43036bc2",
          "name": "getCanvasStoreLocator",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;canvas-store-locator-id&#125;?bottom_paddingnumeric string=bottom_paddingnumeric%20string&element_group_keystring=element_group_keystring&element_typeenum=element_typeenum&header_background_colorstring=header_background_colorstring&idnumeric string=idnumeric%20string&namestring=namestring&top_paddingnumeric string=top_paddingnumeric%20string&typefacestring=typefacestring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Canvas Store Locator"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "287cbe3c-9dee-4d56-a47a-2ca750b66ad5"
            }
          ]
        },
        {
          "id": "18a3fbcd-9153-4e14-a85b-4f78d9eeb127",
          "name": "getCanvasText",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;canvas-text-id&#125;?background_colorstring=background_colorstring&bottom_paddingnumeric string=bottom_paddingnumeric%20string&element_group_keystring=element_group_keystring&element_typeenum=element_typeenum&font_familystring=font_familystring&font_sizenumeric string=font_sizenumeric%20string&idnumeric string=idnumeric%20string&line_heightnumeric string=line_heightnumeric%20string&namestring=namestring&rich_textCanvasRichText=rich_textCanvasRichText&text_alignmentenum=text_alignmentenum&text_colorstring=text_colorstring&top_paddingnumeric string=top_paddingnumeric%20string",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Canvas Text"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f544f6a4-8fd2-4b10-924b-15736d426c86"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "7ada3590-117b-409e-999d-c6be7a7b910a",
          "name": "getApplicationContext",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;application-context-id&#125;?idstring=idstring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application Context"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "945a8f26-abed-469d-b354-af1ea3b646c6"
            }
          ]
        },
        {
          "id": "5d0faa5e-00c1-418a-8ecb-55a83db8a190",
          "name": "getApplication",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;application-id&#125;?an_ad_space_limitunsigned int32=an_ad_space_limitunsigned%20int32&an_platformslistenum=an_platformslistenum&app_domainsliststring=app_domainsliststring&app_install_trackedbool=app_install_trackedbool&app_namestring=app_namestring&app_typeunsigned int32=app_typeunsigned%20int32&auth_dialog_data_help_urlstring=auth_dialog_data_help_urlstring&auth_dialog_headlinestring=auth_dialog_headlinestring&auth_dialog_perms_explanationstring=auth_dialog_perms_explanationstring&auth_referral_default_activity_privacystring=auth_referral_default_activity_privacystring&auth_referral_enabledunsigned int32=auth_referral_enabledunsigned%20int32&auth_referral_extended_permsliststring=auth_referral_extended_permsliststring&auth_referral_friend_permsliststring=auth_referral_friend_permsliststring&auth_referral_response_typestring=auth_referral_response_typestring&auth_referral_user_permsliststring=auth_referral_user_permsliststring&businessBusiness=businessBusiness&canvas_fluid_heightbool=canvas_fluid_heightbool&canvas_fluid_widthunsigned int32=canvas_fluid_widthunsigned%20int32&canvas_urlstring=canvas_urlstring&categorystring=categorystring&client_configmap=client_configmap&companystring=companystring&configured_ios_ssobool=configured_ios_ssobool&contact_emailstring=contact_emailstring&contextApplicationContext=contextApplicationContext&created_timedatetime=created_timedatetime&creator_uidid=creator_uidid&daily_active_usersnumeric string=daily_active_usersnumeric%20string&daily_active_users_rankunsigned int32=daily_active_users_rankunsigned%20int32&deauth_callback_urlstring=deauth_callback_urlstring&default_share_modestring=default_share_modestring&descriptionstring=descriptionstring&financial_idstring=financial_idstring&hosting_urlstring=hosting_urlstring&icon_urlstring=icon_urlstring&idnumeric string=idnumeric%20string&ios_bundle_idliststring=ios_bundle_idliststring&ios_supports_native_proxy_auth_flowbool=ios_supports_native_proxy_auth_flowbool&ios_supports_system_authbool=ios_supports_system_authbool&ipad_app_store_idstring=ipad_app_store_idstring&iphone_app_store_idstring=iphone_app_store_idstring&is_viewer_adminbool=is_viewer_adminbool&latest_sdk_versionApplicationSDKInfo=latest_sdk_versionApplicationSDKInfo&linkstring=linkstring&logging_tokenstring=logging_tokenstring&logo_urlstring=logo_urlstring&migrationsmapstring, bool=migrationsmapstring%2C%20bool&mobile_profile_section_urlstring=mobile_profile_section_urlstring&mobile_web_urlstring=mobile_web_urlstring&monthly_active_usersnumeric string=monthly_active_usersnumeric%20string&monthly_active_users_rankunsigned int32=monthly_active_users_rankunsigned%20int32&namespacestring=namespacestring&namestring=namestring&object_store_urlsApplicationObjectStoreURLs=object_store_urlsApplicationObjectStoreURLs&page_tab_default_namestring=page_tab_default_namestring&page_tab_urlstring=page_tab_urlstring&photo_urlstring=photo_urlstring&privacy_policy_urlstring=privacy_policy_urlstring&profile_section_urlstring=profile_section_urlstring&restrictionsApplicationRestrictionInfo=restrictionsApplicationRestrictionInfo&secure_canvas_urlstring=secure_canvas_urlstring&secure_page_tab_urlstring=secure_page_tab_urlstring&server_ip_whiteliststring=server_ip_whiteliststring&social_discoveryunsigned int32=social_discoveryunsigned%20int32&subcategorystring=subcategorystring&supported_platformslistenum &#123;WEB, CANVAS, MOBILE_WEB, IPHONE, IPAD, ANDROID, WINDOWS, AMAZON, SUPPLEMENTARY_IMAGES, GAMEROOM, INSTANT_GAME&#125;=supported_platformslistenum%20%26%23123%3BWEB%2C%20CANVAS%2C%20MOBILE_WEB%2C%20IPHONE%2C%20IPAD%2C%20ANDROID%2C%20WINDOWS%2C%20AMAZON%2C%20SUPPLEMENTARY_IMAGES%2C%20GAMEROOM%2C%20INSTANT_GAME%26%23125%3B&terms_of_service_urlstring=terms_of_service_urlstring&url_scheme_suffixstring=url_scheme_suffixstring&user_support_emailstring=user_support_emailstring&user_support_urlstring=user_support_urlstring&website_urlstring=website_urlstring&weekly_active_usersnumeric string=weekly_active_usersnumeric%20string",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "246eba39-0fd8-4fbd-8376-dce57dcdbee4"
            }
          ]
        }
      ]
    },
    {
      "name": "Analytics",
      "item": [
        {
          "id": "615f96e7-745a-4b53-9130-188531c84564",
          "name": "getAnalyticsAppEventsExport",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;analytics-app-events-export-id&#125;?column_namesliststring=column_namesliststring&end_tsdatetime=end_tsdatetime&error_messagestring=error_messagestring&event_param_nameslistAnalyticsAppEventsExportEventParamNames=event_param_nameslistAnalyticsAppEventsExportEventParamNames&idnumeric string=idnumeric%20string&recent_download_timestampslistdatetime=recent_download_timestampslistdatetime&request_tsdatetime=request_tsdatetime&start_tsdatetime=start_tsdatetime&statusenum=statusenum",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Analytics App Events Export"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e1b3413-db81-41e5-902f-2ca44a8ce719"
            }
          ]
        }
      ]
    },
    {
      "name": "Audience",
      "item": [
        {
          "id": "937f8cdf-aff5-4772-bbfd-1e863c3bb342",
          "name": "getAudienceInsightsRule",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;audience-insights-rule-id&#125;?archivedbool=archivedbool&can_be_updatedbool=can_be_updatedbool&created_byUser=created_byUser&creation_timedatetime=creation_timedatetime&descriptionstring=descriptionstring&idnumeric string=idnumeric%20string&languageenum=languageenum&namestring=namestring&rule_componentslistAudienceInsightsRuleComponent=rule_componentslistAudienceInsightsRuleComponent&studieslistAudienceStudy=studieslistAudienceStudy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Audience Insights Rule"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dcca8d41-aba3-4458-bfea-265a981dab06"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "e8ff70b4-eefe-4298-a91f-c9133df67459",
          "name": "getComment",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;comment-id&#125;?attachment=attachment&can_comment=can_comment&can_hide=can_hide&can_like=can_like&can_remove=can_remove&can_reply_privately=can_reply_privately&comment_count=comment_count&created_time=created_time&from=from&id=id&length=length&like_count=like_count&message=message&message_tags=message_tags&name=name&object=object&offset=offset&parent=parent&private_reply_conversation=private_reply_conversation&type=type&user_likes=user_likes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A comment can be made on various types of content on Facebook. Most Graph API nodes have a /comments edge that lists all the comments on that object. The /&#123;comment-id&#125; node returns a single comment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b5884e1-2c59-4805-bd56-557ac7750c1e"
            }
          ]
        },
        {
          "id": "944a721a-1b2f-4e8e-9829-451bd641dc9c",
          "name": "postComment",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;comment-id&#125;?is_hidden=is_hidden",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "A comment can be made on various types of content on Facebook. Most Graph API nodes have a /comments edge that lists all the comments on that object. The /&#123;comment-id&#125; node returns a single comment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b64773e-a047-4144-a283-3fe6012388c1"
            }
          ]
        },
        {
          "id": "0d833d7e-b594-4797-8b08-4960102f135b",
          "name": "deleteComment",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;comment-id&#125;",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "A comment can be made on various types of content on Facebook. Most Graph API nodes have a /comments edge that lists all the comments on that object. The /&#123;comment-id&#125; node returns a single comment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8265a19-304a-4a94-91d8-bcbda1bb37d1"
            }
          ]
        }
      ]
    },
    {
      "name": "Conversation",
      "item": [
        {
          "id": "189dd6e6-1141-4849-9c2f-cbd0f1bf6896",
          "name": "getConversation",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;conversation-id&#125;?can_reply=can_reply&id=id&is_subscribed=is_subscribed&link=link&message_count=message_count&participants=participants&senders=senders&snippet=snippet&unread_count=unread_count&updated_time=updated_time&Vector=Vector",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A Facebook Messages conversation between a person and a Facebook Page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96f808e3-fc5c-4378-80e5-d5dc16c321dc"
            }
          ]
        },
        {
          "id": "48938d74-be6f-4879-9523-4a93ecd7cadc",
          "name": "getConversationMessages",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;conversation-id&#125;/messages?Vector=Vector",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The messages in a conversation between a person and a page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8288f9be-534c-4d43-9385-582f9420703d"
            }
          ]
        },
        {
          "id": "5190e05e-74f3-4b50-b8b4-5112426663e5",
          "name": "postConversationMessages",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;conversation-id&#125;/messages?message=message",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The messages in a conversation between a person and a page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e106303a-7f1f-42bf-93f8-6e3a65806527"
            }
          ]
        }
      ]
    },
    {
      "name": "Debug",
      "item": [
        {
          "id": "eedc48d9-42de-4c3c-9aeb-f5e4d48356f5",
          "name": "getDebugTokenInupdateTokenInupdateToken",
          "request": {
            "url": "http://graph.facebook.com/v3.0/debug_token?input_token=&#123;input-token&#125;?application=application&app_id=app_id&code=code&data=data&error=error&expires_at=expires_at&issued_at=issued_at&is_valid=is_valid&message=message&metadata=metadata&profile_id=profile_id&scopes=scopes&subcode=subcode&user_id=user_id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint returns metadata about a given access token. This includes data such as the user for which the token was issued, whether the token is still valid, when it expires, and what permissions the app has for the given user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40b66664-c01d-4b05-a8e0-72e3862f16e9"
            }
          ]
        }
      ]
    },
    {
      "name": "Doc",
      "item": [
        {
          "id": "d98ccfe9-c4fc-4898-a2f8-fcdb91b1537e",
          "name": "getDoc",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;doc-id&#125;?can_deletebool=can_deletebool&can_editbool=can_editbool&created_timedatetime=created_timedatetime&fromUser=fromUser&iconstring=iconstring&idnumeric string=idnumeric%20string&linkstring=linkstring&messagestring=messagestring&revisionid=revisionid&subjectstring=subjectstring&updated_timedatetime=updated_timedatetime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Doc"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b6077e0-d2a8-4f35-b45e-4ae959b13860"
            }
          ]
        }
      ]
    },
    {
      "name": "Domain",
      "item": [
        {
          "id": "d872f69b-04cc-4ce8-a776-e0309bf35cd9",
          "name": "getDomain",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;domain-id&#125;?id=id&name=name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Domain Insights dashboard and API is no longer available. This change effects all versions of this API. To see referral traffic for your website, and demographic details of your visitors, use Facebook Analytics instead. For more information, see Referral Insights with Facebook Analytics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dcb73a3d-72d8-4f13-8aed-3a25fbdcfd49"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "4ac53664-503e-4fbb-8a37-e00188cb2db9",
          "name": "getEvent",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;event-id&#125;?attending_countint32=attending_countint32&can_guests_invitebool=can_guests_invitebool&categorystring=categorystring&coverCoverPhoto=coverCoverPhoto&declined_countint32=declined_countint32&descriptionstring=descriptionstring&end_timestring=end_timestring&event_timeslistChildEvent=event_timeslistChildEvent&guest_list_enabledbool=guest_list_enabledbool&idnumeric string=idnumeric%20string&interested_countint32=interested_countint32&is_canceledbool=is_canceledbool&is_draftbool=is_draftbool&is_page_ownedbool=is_page_ownedbool&maybe_countint32=maybe_countint32&namestring=namestring&noreply_countint32=noreply_countint32&owner=owner&parent_groupGroup=parent_groupGroup&placePlace=placePlace&scheduled_publish_timestring=scheduled_publish_timestring&start_timestring=start_timestring&ticketing_privacy_uristring=ticketing_privacy_uristring&ticketing_terms_uristring=ticketing_terms_uristring&ticket_uristring=ticket_uristring&ticket_uri_start_sales_timestring=ticket_uri_start_sales_timestring&timezoneenum=timezoneenum&typeenum &#123;private, public, group, community&#125;=typeenum%20%26%23123%3Bprivate%2C%20public%2C%20group%2C%20community%26%23125%3B&updated_timedatetime=updated_timedatetime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f70f97a9-374d-4497-adec-df14a042f0c7"
            }
          ]
        }
      ]
    },
    {
      "name": "Friend",
      "item": [
        {
          "id": "3396f290-da4c-481e-836a-9ee3dc927353",
          "name": "getFriendList",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;friend-list-id&#125;?idnumeric string=idnumeric%20string&list_typeenum=list_typeenum&namestring=namestring&ownernumeric string=ownernumeric%20string",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Friend List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e4bb867-2bad-4c7a-a57e-682223f15c05"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "63dbbc98-9461-43cd-936d-778ee79faf9c",
          "name": "getGroupAdmins",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;group-id&#125;/admins",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This edge was deprecated on April 4th, 2018, and can no longer be used."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2583e313-76e3-493b-906e-bdf3eacf6a5f"
            }
          ]
        },
        {
          "id": "431e2be0-fb78-4adc-8324-9a6dbb2489ac",
          "name": "getGroupAlbums",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;group-id&#125;/albums",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The photo albums created for a Group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87593d48-d94d-46a5-9041-5c4515b0c7d7"
            }
          ]
        },
        {
          "id": "576222b8-4ca4-40b1-90fe-b293e12193bc",
          "name": "getGroupDocs",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;group-id&#125;/docs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The documents owned by a Group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "424dc1f6-9f10-41e0-bd6d-f442f87f9fe5"
            }
          ]
        },
        {
          "id": "2a7906f4-9753-4ff0-b42b-832c45322520",
          "name": "getGroupEvents",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;group-id&#125;/events",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All events that belong to a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e25dd6d-22d4-440d-836d-edd624cf32f2"
            }
          ]
        },
        {
          "id": "c01988d4-9ff0-4690-903a-c5efd749c08f",
          "name": "getGroupFeed",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;group-id&#125;/feed",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Posts owned by a Group, including status updates and links."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a37ec4a-2dae-45a3-aac5-0b1c5b31168b"
            }
          ]
        },
        {
          "id": "328876a3-9811-403c-8e63-757a3163fa5e",
          "name": "postGroupFeed",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;group-id&#125;/feed?link=link&message=message",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts owned by a Group, including status updates and links."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b271ce6-0ad1-4dc4-a742-3f606e23eb8f"
            }
          ]
        },
        {
          "id": "43511aeb-2334-489e-a1d6-d33031768d3f",
          "name": "getGroupFiles",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;group-id&#125;/files?download_link=download_link&from=from&group=group&id=id&message=message&updated_time=updated_time",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The files uploaded to this group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cfd24d0-c869-48e8-9b81-c66a43356a48"
            }
          ]
        },
        {
          "id": "edd61f58-7d37-4448-a69d-d6911fee7805",
          "name": "getGroupMembers",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;group-id&#125;/members?administrator=administrator",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This edge was deprecated on April 4th, 2018, and can no longer be used."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc6b0369-1514-493d-b41c-e04d1794a54a"
            }
          ]
        },
        {
          "id": "4a26f696-9422-4886-920e-e9e3fa35be90",
          "name": "getGroupVeos",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;group-id&#125;/videos",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Videos owned by a Facebook Group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31d4767f-f4c2-49a9-936a-0e98672c1ead"
            }
          ]
        },
        {
          "id": "f1b681ea-c169-49bd-a4b8-b10582adf6c6",
          "name": "getGroupDoc",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;group-doc-id&#125;?can_delete=can_delete&can_edit=can_edit&created_time=created_time&from=from&icon=icon&id=id&message=message&revision=revision&subject=subject&updated_time=updated_time",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents a doc within a Facebook group. The /&#123;group-doc-id&#125; node returns a single doc."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89837452-72f0-42b4-9b3b-0e1a51e293c2"
            }
          ]
        }
      ]
    },
    {
      "name": "Me",
      "item": [
        {
          "id": "5913a9d0-678a-4e90-adc3-da65c57dc442",
          "name": "postMeAlbums",
          "request": {
            "url": "http://graph.facebook.com/v3.0/me/albums?message=message&name=name&Vector=Vector",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The photo albums created for a Group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "454991f1-ac2b-4f65-83e3-f7b6b9b17791"
            }
          ]
        },
        {
          "id": "0a1054d6-cfe6-46a3-b8f7-b1a269c900bf",
          "name": "getMeFeed",
          "request": {
            "url": "http://graph.facebook.com/v3.0/me/feed",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The feed of posts (including status updates) and links published by this person, or by others on this person&#039;s profile. There are other edges which provide filtered versions of this edge:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba18aaa3-dcf2-4347-ab8f-1c8dadcb5001"
            }
          ]
        },
        {
          "id": "78acd664-c2a9-44ce-aaf4-4c4937cb193a",
          "name": "postMeFeed",
          "request": {
            "url": "http://graph.facebook.com/v3.0/me/feed?allow=allow&attached_media=attached_media&deny=deny&link=link&media_fbid=media_fbid&message=message&object_attachment=object_attachment&place=place&privacy=privacy&tags=tags&value=value",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The feed of posts (including status updates) and links published by this person, or by others on this person&#039;s profile. There are other edges which provide filtered versions of this edge:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c9fdb50-2220-42f8-bc6a-7dc9d1be5cea"
            }
          ]
        },
        {
          "id": "e84ef5df-8a95-4bfd-a649-5be585f3f0b6",
          "name": "getMeFriendrequests",
          "request": {
            "url": "http://graph.facebook.com/v3.0/me/friendrequests?created_time=created_time&from=from&message=message&to=to&unread=unread",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A person&#039;s pending friend requests."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00595157-60f3-42f4-a139-648a7fe7c36d"
            }
          ]
        },
        {
          "id": "7f1ff539-41a2-4808-a85d-3abe3349cb7e",
          "name": "getMeHome",
          "request": {
            "url": "http://graph.facebook.com/v3.0/me/home",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "As of October 6th, 2015, this endpoint is no longer available.  Please consider using the /user-id/feed edge instead."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb6b4037-ebf7-40c9-b6ec-4266b63a5297"
            }
          ]
        },
        {
          "id": "a38ac2d4-ad51-4c77-bd9b-f247887fc680",
          "name": "getMeInbox",
          "request": {
            "url": "http://graph.facebook.com/v3.0/me/inbox",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A person&#039;s Facebook Messages inbox."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4400aea9-9d4b-4250-a2df-d3610d958513"
            }
          ]
        },
        {
          "id": "8757ffc6-1409-4a4b-8ed7-b0febf6fd12f",
          "name": "getMeLocations",
          "request": {
            "url": "http://graph.facebook.com/v3.0/me/locations?type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A feed of posts and photos that include location information and in which this person has been tagged. This is useful for constructing a chronology of places that the person has visited."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8958eeb-362e-46b9-a094-b0b2092b51ee"
            }
          ]
        },
        {
          "id": "d507ebc7-9ec0-4547-a7fc-8d0ed9230a6a",
          "name": "getMeOutbox",
          "request": {
            "url": "http://graph.facebook.com/v3.0/me/outbox",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Items in a person&#039;s Facebook Messages outbox."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7dc615f-8b5c-4397-9adf-1005d131073d"
            }
          ]
        },
        {
          "id": "5517a509-8121-4eaf-a126-60cb12b2644c",
          "name": "getMeScores",
          "request": {
            "url": "http://graph.facebook.com/v3.0/me/scores?application=application&score=score&user=user",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "As of April 4, 2018, this endpoint only returns an empty data set. Please see the changelog for more information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88afcb17-c74e-4e3e-ae27-47dda9fcbcea"
            }
          ]
        },
        {
          "id": "4272d130-b65d-41c7-918c-f4a991569345",
          "name": "postMeScores",
          "request": {
            "url": "http://graph.facebook.com/v3.0/me/scores?score=score",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "As of April 4, 2018, this endpoint only returns an empty data set. Please see the changelog for more information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24266107-f20f-46bc-a6d4-796c690f6a05"
            }
          ]
        },
        {
          "id": "71466261-9aa0-4d88-bb09-8aab630ed3f9",
          "name": "deleteMeScores",
          "request": {
            "url": "http://graph.facebook.com/v3.0/me/scores",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "As of April 4, 2018, this endpoint only returns an empty data set. Please see the changelog for more information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6119f4c9-7be9-4c32-9d13-c557fac6f3f1"
            }
          ]
        }
      ]
    },
    {
      "name": "Life",
      "item": [
        {
          "id": "8a8a3f5f-d2d9-4d76-8b8f-3b7a6a1f3fd5",
          "name": "getLifeEvent",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;life-event-id&#125;?created_timedatetime=created_timedatetime&descriptionstring=descriptionstring&end_timedatetime=end_timedatetime&fromPage=fromPage&idnumeric string=idnumeric%20string&is_hiddenbool=is_hiddenbool&start_timedatetime=start_timedatetime&titlestring=titlestring&updated_timedatetime=updated_timedatetime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Life Event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82db75ae-665d-427a-86b7-2e605cc8f54c"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "c0e76291-fd14-4207-af1d-118c8cb1f067",
          "name": "getLink",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;link-id&#125;?created_time=created_time&description=description&from=from&icon=icon&id=id&link=link&message=message&name=name&picture=picture",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A link shared on Facebook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63b0ccd3-55b8-41b8-87b2-77c159864570"
            }
          ]
        },
        {
          "id": "3088bd8f-0b14-4bac-8b24-1f96abf47bf4",
          "name": "deleteLink",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;link-id&#125;",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "A link shared on Facebook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac158a2a-668d-4660-ba12-e81494e1d1c2"
            }
          ]
        }
      ]
    },
    {
      "name": "Live",
      "item": [
        {
          "id": "2e98ab05-16c8-4a8e-b0ba-a8590970d361",
          "name": "getLiveVeo",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;live-video-id&#125;?ad_break_configLiveVideoAdBreakConfig=ad_break_configLiveVideoAdBreakConfig&ad_break_failure_reasonenum=ad_break_failure_reasonenum&broadcast_start_timedatetime=broadcast_start_timedatetime&copyrightVideoCopyright=copyrightVideoCopyright&creation_timedatetime=creation_timedatetime&dash_preview_urlstring=dash_preview_urlstring&descriptionstring=descriptionstring&embed_htmlstring=embed_htmlstring&idnumeric string=idnumeric%20string&is_manual_modebool=is_manual_modebool&is_reference_onlybool=is_reference_onlybool&live_viewsunsigned int32=live_viewsunsigned%20int32&permalink_urlstring=permalink_urlstring&planned_start_timedatetime=planned_start_timedatetime&seconds_leftint32=seconds_leftint32&secure_stream_urlstring=secure_stream_urlstring&statusenum=statusenum&stream_urlstring=stream_urlstring&titlestring=titlestring&videoVideo=videoVideo",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Live Video"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed8813e7-6243-415e-aec2-faa069161ac3"
            }
          ]
        }
      ]
    },
    {
      "name": "Mailing",
      "item": [
        {
          "id": "ffca4041-5d81-4df6-ab91-a60386409bff",
          "name": "getMailingAddress",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;mailing-address-id&#125;?citystring=citystring&city_pagePage=city_pagePage&countrystring=countrystring&idnumeric string=idnumeric%20string&postal_codestring=postal_codestring&regionstring=regionstring&street1string=street1string&street2string=street2string",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Mailing Address"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e91082c8-0be9-4a57-acc6-fa0f093c51b6"
            }
          ]
        }
      ]
    },
    {
      "name": "Message",
      "item": [
        {
          "id": "8f1d03c0-3acc-4806-8e37-7142fc420684",
          "name": "getMessage",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;message-id&#125;?created_time=created_time&from=from&id=id&message=message&subject=subject&tags=tags&to=to",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "An individual message in Facebook Messenger.  This is a Pages-only endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c091c2fd-0c63-426b-8cc7-bd4c8c6fddea"
            }
          ]
        },
        {
          "id": "a70b2bd8-73ca-4cd2-85b9-fe5c80b1d9c3",
          "name": "getMessageAttachments",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;message-id&#125;/attachments?id=id&mime_type=mime_type&name=name&size=size",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Files attached to a message. This is a Pages-only endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7f11548-ca16-4179-824e-9c4f47373e84"
            }
          ]
        },
        {
          "id": "99b037d6-880a-4c3f-93f4-330a2f28aa5f",
          "name": "getMessageShares",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;message-id&#125;/shares?description=description&id=id&link=link&name=name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Shared items in a message. This is a Pages-only endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9bfb3207-66a7-4910-bfcc-82de6e43f125"
            }
          ]
        }
      ]
    },
    {
      "name": "Milestone",
      "item": [
        {
          "id": "326ea67c-3cfb-4819-8043-3b67865a3fbc",
          "name": "getMilestone",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;milestone-id&#125;?created_time=created_time&description=description&end_time=end_time&from=from&id=id&start_time=start_time&title=title&updated_time=updated_time",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This represents a milestone on a Facebook Page. The /&#123;milestone-id&#125; node returns a single &#039;milestone&#039;."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ae1a635-6f59-42ff-a829-1507024683db"
            }
          ]
        }
      ]
    },
    {
      "name": "Notification",
      "item": [
        {
          "id": "f827edd5-32f7-43db-a90d-b951f3800053",
          "name": "getNotification",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;notification-id&#125;?application=application&created_time=created_time&from=from&id=id&link=link&object=object&title=title&to=to&unread=unread&updated_time=updated_time",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "An individual unread Facebook notification.  This is an API that&#039;s only available for Pages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3bd7d92-a60e-42f2-9670-08fcca01f3be"
            }
          ]
        }
      ]
    },
    {
      "name": "Open",
      "item": [
        {
          "id": "3bf24a7f-6231-457c-844a-6fb72a04535b",
          "name": "getOpenGraphActionType",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;open-graph-action-type-id&#125;?allow_multiple_referencesbool=allow_multiple_referencesbool&app_prepositionstring=app_prepositionstring&button_textstring=button_textstring&descriptionstring=descriptionstring&idnumeric string=idnumeric%20string&is_app_secret_requiredbool=is_app_secret_requiredbool&namestring=namestring&object_typeslistid=object_typeslistid&plural_paststring=plural_paststring&plural_presentstring=plural_presentstring&property_configmapstring, OpenGraphPropertyConfig=property_configmapstring%2C%20OpenGraphPropertyConfig&singular_paststring=singular_paststring&singular_presentstring=singular_presentstring&tenses_disabledint32=tenses_disabledint32&typestring=typestring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Open Graph Action Type"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d238fb7c-df6a-42f1-aab9-40e50944dc87"
            }
          ]
        },
        {
          "id": "642c2144-d636-4534-8115-9782732e214e",
          "name": "getOpenGraphContext",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;open-graph-context-id&#125;?idstring=idstring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Open Graph Context"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e5213bd-223b-4c6a-9103-feff0ef7bb02"
            }
          ]
        },
        {
          "id": "5436055e-ac23-48b9-809a-19f38622e17f",
          "name": "getOpenGraphObjectType",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;open-graph-object-type-id&#125;?articlestring=articlestring&idnumeric string=idnumeric%20string&namestring=namestring&pluralstring=pluralstring&property_configmapstring, OpenGraphPropertyConfig=property_configmapstring%2C%20OpenGraphPropertyConfig&singularstring=singularstring&typestring=typestring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Open Graph Object Type"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c3154dc-57cd-4fdc-b8ba-231998c49cc1"
            }
          ]
        }
      ]
    },
    {
      "name": "Page",
      "item": [
        {
          "id": "93a12d44-c9f9-4e58-a5a3-83f3437a154e",
          "name": "getPageAdminNote",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;page-admin-note-id&#125;?bodystring=bodystring&fromPage=fromPage&idnumeric string=idnumeric%20string&userUser=userUser",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Page Admin Note"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8429b25d-2204-4b54-bcc3-af1769d4f070"
            }
          ]
        },
        {
          "id": "736d33db-dfc7-4512-a08d-7d30c4474c18",
          "name": "getPageCallToAction",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;page-call-to-action-id&#125;?android_appApplication=android_appApplication&android_deeplinkstring=android_deeplinkstring&android_destination_typeenum=android_destination_typeenum&android_package_namestring=android_package_namestring&android_urlstring=android_urlstring&created_timedatetime=created_timedatetime&email_addressstring=email_addressstring&fromPage=fromPage&idnumeric string=idnumeric%20string&intl_number_with_plusstring=intl_number_with_plusstring&iphone_appApplication=iphone_appApplication&iphone_deeplinkstring=iphone_deeplinkstring&iphone_destination_typeenum=iphone_destination_typeenum&iphone_urlstring=iphone_urlstring&statusenum=statusenum&typeenum=typeenum&updated_timedatetime=updated_timedatetime&web_destination_typeenum=web_destination_typeenum&web_urlstring=web_urlstring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Page Call To Action"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "682b91ad-bc43-40fb-9dfe-9cd0e2fcd8f4"
            }
          ]
        },
        {
          "id": "18ca9884-f5f3-4bba-b526-639546f60011",
          "name": "getPageLabel",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;page-label-id&#125;?creation_timedatetime=creation_timedatetime&creator_idProfile=creator_idProfile&fromPage=fromPage&idnumeric string=idnumeric%20string&namestring=namestring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Page Label"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb033471-154e-41e5-b876-296461ca2a44"
            }
          ]
        }
      ]
    },
    {
      "name": "Pages",
      "item": [
        {
          "id": "1b5c7ab1-855e-41ac-a5e8-a6ad17ab2e51",
          "name": "getPagesPlatformComponentFlowServiceConfig",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;pages-platform-component-flow-service-config-id&#125;?deeplinkstring=deeplinkstring&flow_categoryenum=flow_categoryenum&idnumeric string=idnumeric%20string&labelstring=labelstring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Pages Platform Component Flow Service Config"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bdd07ff-dd20-47a5-bd2d-16fab01c0ff1"
            }
          ]
        }
      ]
    },
    {
      "name": "Payment",
      "item": [
        {
          "id": "51e06701-bc60-4de8-ba88-3d8160d929e3",
          "name": "getPayment",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;payment-id&#125;?actions=actions&amount=amount&application=application&country=country&created_time=created_time&currency=currency&disputes=disputes&id=id&items=items&payout_foreign_exchange_rate=payout_foreign_exchange_rate&product=product&quantity=quantity&reason=reason&request_id=request_id&status=status&tax=tax&tax_amount=tax_amount&tax_country=tax_country&test=test&time_created=time_created&time_updated=time_updated&type=type&user=user&user_comment=user_comment&user_email=user_email",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The details of a payment made in an app using Facebook Payments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03feac1b-564f-4dea-9795-3e176909777a"
            }
          ]
        },
        {
          "id": "a99d6013-35cc-4104-9d47-08a292e93d00",
          "name": "postPaymentDisupdatee",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;payment-id&#125;/dispute?reason=reason",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Used to settle any payment disputes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e526f8ac-63e5-4d79-b6bf-eec04bcf8f40"
            }
          ]
        },
        {
          "id": "9ee3ff94-f481-4ed8-9446-8c7c244457ae",
          "name": "postPaymentRefunds",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;payment-id&#125;/refunds?amount=amount&currency=currency&reason=reason",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Used to issue any payment refunds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fcfed89-6f79-4225-b8f7-6ef01fbde704"
            }
          ]
        }
      ]
    },
    {
      "name": "Place",
      "item": [
        {
          "id": "6a745b0a-4684-4bca-a7e9-5e8fee6b6597",
          "name": "getPlaceTag",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;place-tag-id&#125;?created_timedatetime=created_timedatetime&idnumeric string=idnumeric%20string&placePage=placePage",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Place Tag"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "899a21ce-02ee-44aa-8757-618710740622"
            }
          ]
        },
        {
          "id": "ea8548e4-e2f6-445d-89cb-54216d913768",
          "name": "getPlaceTopic",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;place-topic-id&#125;?countunsigned int32=countunsigned%20int32&has_childrenbool=has_childrenbool&icon_urlstring=icon_urlstring&idnumeric string=idnumeric%20string&namestring=namestring&parent_idslistid=parent_idslistid&plural_namestring=plural_namestring&top_subtopic_namesliststring=top_subtopic_namesliststring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Place Topic"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33e1eb93-7c4f-4d2e-9ff9-a235642c07f5"
            }
          ]
        }
      ]
    },
    {
      "name": "Posts",
      "item": [
        {
          "id": "a406ad24-60f4-4d0e-8ebd-189de9fc3199",
          "name": "getAdd",
          "request": {
            "url": "http://graph.facebook.com/v3.0/post-id?admin_creator=admin_creator&age_max=age_max&age_min=age_min&allow=allow&application=application&call_to_action=call_to_action&can_reply_privately=can_reply_privately&caption=caption&cities=cities&college_years=college_years&context=context&countries=countries&created_time=created_time&deny=deny&description=description&education_statuses=education_statuses&feed_targeting=feed_targeting&friends=friends&from=from&full_picture=full_picture&genders=genders&href=href&icon=icon&id=id&instagram_eligibility=instagram_eligibility&interested_in=interested_in&interests=interests&is_hidden=is_hidden&is_instagram_eligible=is_instagram_eligible&is_published=is_published&length=length&link=link&locales=locales&message=message&message_tags=message_tags&name=name&object_id=object_id&offset=offset&parent_id=parent_id&permalink_url=permalink_url&picture=picture&place=place&privacy=privacy&promotable_id=promotable_id&promotion_status=promotion_status&properties=properties&regions=regions&relationship_statuses=relationship_statuses&shares=shares&source=source&status_type=status_type&story=story&story_tags=story_tags&targeting=targeting&text=text&to=to&type=type&updated_time=updated_time&value=value&with_tags=with_tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "An individual entry in a profile&#039;s feed. The profile could be a user, page, app, or group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "063fbd5a-db07-421d-974d-eef0ba8518b6"
            }
          ]
        },
        {
          "id": "5c2a9862-8e92-4638-8111-9c06f691deb0",
          "name": "postAdd",
          "request": {
            "url": "http://graph.facebook.com/v3.0/post-id",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "An individual entry in a profile&#039;s feed. The profile could be a user, page, app, or group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e3683b7-20b2-4690-8d27-841ce6c2eb70"
            }
          ]
        },
        {
          "id": "42702a5b-e843-4063-9a01-bad6f69477ae",
          "name": "deleteAdd",
          "request": {
            "url": "http://graph.facebook.com/v3.0/post-id",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "An individual entry in a profile&#039;s feed. The profile could be a user, page, app, or group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea618eb7-fa23-44c6-b3ad-0839d741e473"
            }
          ]
        }
      ]
    },
    {
      "name": "Attachments",
      "item": [
        {
          "id": "52c03c30-b31f-4767-bb23-b6dd56281a98",
          "name": "getAddAttachments",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;post-id&#125;/attachments?description=description&description_tags=description_tags&title=title&type=type&url=url&Vector=Vector",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Media content associated with a story or comment. Story attachments are accessed from the following endpoints:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de3f5844-6a2d-4535-a40e-861aa35cdd6a"
            }
          ]
        }
      ]
    },
    {
      "name": "Promotion",
      "item": [
        {
          "id": "5647a839-3dec-422e-9e54-588e13d713f1",
          "name": "getPromotionInfo",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;promotion-info-id&#125;?budgetunsigned int32=budgetunsigned%20int32&currencystring=currencystring&spentunsigned int32=spentunsigned%20int32",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Promotion Info"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bde94e94-3e99-4aa7-85c3-acb24874492f"
            }
          ]
        }
      ]
    },
    {
      "name": "Rtb",
      "item": [
        {
          "id": "58854f01-3728-42dd-9179-0a8036214fdb",
          "name": "getRtbDynamicAdd",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;rtb-dynamic-post-id&#125;?child_attachmentslistDynamicPostChildAttachment=child_attachmentslistDynamicPostChildAttachment&createddatetime=createddatetime&descriptionstring=descriptionstring&idnumeric string=idnumeric%20string&image_urlstring=image_urlstring&linkstring=linkstring&messagestring=messagestring&owner_idnumeric string=owner_idnumeric%20string&place_idnumeric string=place_idnumeric%20string&product_idnumeric string=product_idnumeric%20string&titlestring=titlestring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Rtb Dynamic Post"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91990732-7de2-4e37-a20c-6b1b0875c393"
            }
          ]
        }
      ]
    },
    {
      "name": "Request",
      "item": [
        {
          "id": "eb5d8fce-0b4a-4df5-8445-9c0c94b9d120",
          "name": "getRequest",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;request-id&#125;?application=application&created_time=created_time&from=from&id=id&message=message&to=to",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "An individual game request received by someone, sent by an app or by another person."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3946b82-ec4e-46ad-baf5-fc0f2b2b8cdb"
            }
          ]
        },
        {
          "id": "ce93bb0c-e4fe-4e31-819b-4ac6521e17c3",
          "name": "deleteRequest",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;request-id&#125;",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "An individual game request received by someone, sent by an app or by another person."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0062f47-a625-455a-9cc1-32cd7722c7de"
            }
          ]
        }
      ]
    },
    {
      "name": "Sales",
      "item": [
        {
          "id": "48389c3c-213a-45f7-ab4e-01edfb29d203",
          "name": "getSalesPromo",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;sales-promo-id&#125;?availability_locationenum=availability_locationenum&descriptionstring=descriptionstring&destination_uristring=destination_uristring&discount_codestring=discount_codestring&expiration_timedatetime=expiration_timedatetime&idnumeric string=idnumeric%20string&pagePage=pagePage&schedule_timedatetime=schedule_timedatetime&start_timedatetime=start_timedatetime&terms_and_conditionsstring=terms_and_conditionsstring&titlestring=titlestring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Offer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0125b400-f77a-46c4-8e10-0156cce8bc5d"
            }
          ]
        }
      ]
    },
    {
      "name": "Saved",
      "item": [
        {
          "id": "4bda7a05-30f5-4543-9d46-6574cfea8f92",
          "name": "getSavedMessageResponse",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;saved-message-response-id&#125;?categorystring=categorystring&idnumeric string=idnumeric%20string&imagestring=imagestring&is_enabledbool=is_enabledbool&messagestring=messagestring&titlestring=titlestring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Saved Message Response"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8c21868-0c17-4677-8012-5d19e20c00e0"
            }
          ]
        }
      ]
    },
    {
      "name": "Status",
      "item": [
        {
          "id": "f4d0b545-00e8-49e2-b91c-7e34df6449b1",
          "name": "getStatus",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;status-id&#125;?event=event&from=from&id=id&message=message&name=name&place=place&updated_time=updated_time",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A status message in a profile&#039;s feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9963f24-078a-45f9-8829-93802483cc53"
            }
          ]
        }
      ]
    },
    {
      "name": "From.",
      "item": [
        {
          "id": "6e746168-7fdb-4d80-bf02-26d01393c8d1",
          "name": "postFrom.Status",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;from.id&#125;_&#123;status-id&#125;",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "A status message in a profile&#039;s feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c753777-96a3-4ce9-a61a-6e264636917e"
            }
          ]
        },
        {
          "id": "d499de17-a5ab-475d-90d2-6cb09469abf8",
          "name": "deleteFrom.Status",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;from.id&#125;_&#123;status-id&#125;",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "A status message in a profile&#039;s feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f20652d5-ee8e-454c-b4c2-589e913c0618"
            }
          ]
        }
      ]
    },
    {
      "name": "Test",
      "item": [
        {
          "id": "34a6b6f4-0c6d-4aab-8092-5f1b0b91d1ed",
          "name": "postTestUser",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;test-user-id&#125;?name=name&password=password",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "A test user associated with a Facebook app. Test users are created and associated using the /&#123;app-id&#125;/accounts/test-users edge or in the App Dashboard."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bbb7b31b-b3f5-4440-9f52-fdaa5a5c6718"
            }
          ]
        },
        {
          "id": "83b9d6db-34c3-47a7-b6eb-1ff644cb29c2",
          "name": "deleteTestUser",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;test-user-id&#125;",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "A test user associated with a Facebook app. Test users are created and associated using the /&#123;app-id&#125;/accounts/test-users edge or in the App Dashboard."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cbf6a65-7301-49de-b218-edd10fe28265"
            }
          ]
        },
        {
          "id": "3b45af2b-8c3f-438e-8a3a-2efa59f05aff",
          "name": "postTestUser1FriendsTestUser2",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;test-user-1&#125;/friends/&#123;test-user-2&#125;",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The friends of a test user. This is identical to the /&#123;user-id&#125;/friends edge aside from the publishing operation explained below."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f42188f3-0057-4283-af4f-1bc8d6f04753"
            }
          ]
        }
      ]
    },
    {
      "name": "Thread",
      "item": [
        {
          "id": "a0596b2b-8be3-4b18-a361-11cf430fab2a",
          "name": "getThread",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;thread-id&#125;?comments=comments&id=id&to=to&unread=unread&unseen=unseen&updated_time=updated_time",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A Facebook Messages conversation thread. This endpoint is only accessible for users that are developers of the app making the request. Pages should use the Conversation object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08710fa5-9609-45b1-bf51-5534f6bb2820"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "39e7b923-69be-4d25-af10-335d511a7e7c",
          "name": "getUser",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;?aboutstring=aboutstring&addressLocation=addressLocation&admin_noteslistPageAdminNote=admin_noteslistPageAdminNote&age_rangeAgeRange=age_rangeAgeRange&birthdaystring=birthdaystring&contextUserContext=contextUserContext&coverUserCoverPhoto=coverUserCoverPhoto&currencyCurrency=currencyCurrency&deviceslistUserDevice=deviceslistUserDevice&educationlistEducationExperience=educationlistEducationExperience&emailstring=emailstring&employee_numberstring=employee_numberstring&favorite_athleteslistExperience=favorite_athleteslistExperience&favorite_teamslistExperience=favorite_teamslistExperience&first_namestring=first_namestring&genderstring=genderstring&hometownPage=hometownPage&idnumeric string=idnumeric%20string&inspirational_peoplelistExperience=inspirational_peoplelistExperience&installedbool=installedbool&install_typeenum=install_typeenum&interested_inliststring=interested_inliststring&is_shared_loginbool=is_shared_loginbool&is_verifiedbool=is_verifiedbool&labelslistPageLabel=labelslistPageLabel&languageslistExperience=languageslistExperience&last_namestring=last_namestring&linkstring=linkstring&localestring=localestring&local_news_megaphone_dismiss_statusbool=local_news_megaphone_dismiss_statusbool&local_news_subscription_statusbool=local_news_subscription_statusbool&locationPage=locationPage&meeting_forliststring=meeting_forliststring&middle_namestring=middle_namestring&namestring=namestring&name_formatstring=name_formatstring&payment_pricepointsPaymentPricepoints=payment_pricepointsPaymentPricepoints&politicalstring=politicalstring&public_keystring=public_keystring&quotesstring=quotesstring&relationship_statusstring=relationship_statusstring&religionstring=religionstring&security_settingsSecuritySettings=security_settingsSecuritySettings&shared_login_upgrade_required_bydatetime=shared_login_upgrade_required_bydatetime&significant_otherUser=significant_otherUser&sportslistExperience=sportslistExperience&test_groupunsigned int32=test_groupunsigned%20int32&third_party_idstring=third_party_idstring&timezonefloat (min: -24) (max: 24)=timezonefloat%20%28min%3A%20-24%29%20%28max%3A%2024%29&token_for_businessstring=token_for_businessstring&updated_timedatetime=updated_timedatetime&verifiedbool=verifiedbool&video_upload_limitsVideoUploadLimits=video_upload_limitsVideoUploadLimits&viewer_can_send_giftbool=viewer_can_send_giftbool&websitestring=websitestring&worklistWorkExperience=worklistWorkExperience",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e779de1e-a09c-4fc8-9fed-afe5716e491e"
            }
          ]
        },
        {
          "id": "420db025-3cbc-40c0-86d1-ae11b3775be6",
          "name": "getUserContext",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-context-id&#125;?idstring=idstring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Context"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85399af9-d149-45fa-b094-a45726d36ed3"
            }
          ]
        },
        {
          "id": "2d1513ff-a257-4a9b-b03c-19094d1e6fe1",
          "name": "getUserAchievements",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/achievements?100=100",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Achievements"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae9e72ba-2334-4e43-b68f-d8184223a5ab"
            }
          ]
        },
        {
          "id": "7c079e25-4e97-40d5-9865-a537e3c810ec",
          "name": "getUserAdStudies",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/ad_studies?total_countunsigned int32=total_countunsigned%20int32",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Ad Studies"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "713849c6-70da-43c4-bbfc-3438926222c3"
            }
          ]
        },
        {
          "id": "7997abfb-76a5-43bf-bbf3-7eb7f9617f7f",
          "name": "getUserAdaccounts",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/adaccounts?total_countunsigned int32=total_countunsigned%20int32",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Adaccounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17e82d47-3789-4b98-940d-b10efcb169f4"
            }
          ]
        },
        {
          "id": "aa092ea1-b9e3-4d49-8283-8f294463dde1",
          "name": "getUserAdcontracts",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/adcontracts?200=200&278=278",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Adcontracts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a884e53-1fac-4955-b59b-8e360a2bb7dd"
            }
          ]
        },
        {
          "id": "b271672b-c697-4828-9fa3-ccf34d5fec21",
          "name": "getUserAdnetworkanalytics",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/adnetworkanalytics?100=100&3001=3001&3011=3011",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Adnetworkanalytics"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8929c23c-4581-4406-8b91-22e297baf990"
            }
          ]
        },
        {
          "id": "13d1e11b-b31a-459d-a57a-1ff10dadf14c",
          "name": "getUserAlbums",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/albums?100=100&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Albums"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22cd6c22-65f1-4111-a900-c05fa93d0248"
            }
          ]
        },
        {
          "id": "a6bda6dd-d8be-4ce5-b42e-58995aebd584",
          "name": "getUserApprequestformerrecipients",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/apprequestformerrecipients?110=110&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Apprequestformerrecipients"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa406685-9542-4760-bfa5-384e82d5355d"
            }
          ]
        },
        {
          "id": "c0c2b056-c9aa-4a79-aaa0-837095a29be4",
          "name": "getUserApprequests",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/apprequests?100=100&159=159&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Apprequests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea2cfc8b-a640-4d6f-b8ff-b224dd563e04"
            }
          ]
        },
        {
          "id": "8d0f5cc9-2b67-464c-909b-5cd08705bb74",
          "name": "getUserAsset3ds",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/asset3ds?100=100",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Asset3ds"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a154122-5abf-443c-ac3c-f8247b3320e8"
            }
          ]
        },
        {
          "id": "e253d0dc-f406-4ea9-92a5-10a48793d72c",
          "name": "getUserAssignedAdAccounts",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/assigned_ad_accounts?permitted_rolesliststring=permitted_rolesliststring&rolestring=rolestring&tasksliststring=tasksliststring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Assigned Ad Accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6264c7e0-f44e-4f2d-bc42-5f5a7a8a427f"
            }
          ]
        },
        {
          "id": "37b81566-1ba7-4380-89ba-bab463731e33",
          "name": "getUserAssignedMonetizationProperties",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/assigned_monetization_properties?permitted_rolesliststring=permitted_rolesliststring&rolestring=rolestring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Assigned Monetization Properties"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2aad57c0-8e88-49a7-b618-e6b90a5fe33d"
            }
          ]
        },
        {
          "id": "6970e861-81ce-4bf5-b1bf-1fc1810ee474",
          "name": "getUserAssignedPages",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/assigned_pages?permitted_rolesliststring=permitted_rolesliststring&rolestring=rolestring&tasksliststring=tasksliststring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Assigned Pages"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a04e658a-b4d2-4bf8-92b4-2d2fc3fd3a6a"
            }
          ]
        },
        {
          "id": "4d139e5f-b271-4386-af6c-4714544ca3eb",
          "name": "getUserAssignedProductCatalogs",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/assigned_product_catalogs?access_typestring=access_typestring&permitted_rolesliststring=permitted_rolesliststring&rolestring=rolestring&roles_and_tasksliststring=roles_and_tasksliststring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Assigned Product Catalogs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee4687db-06c0-4f78-b365-3391df42ebe3"
            }
          ]
        },
        {
          "id": "7b87696e-c4f5-4201-a475-7227e5578676",
          "name": "getUserBooks",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/books?created_timedatetime=created_timedatetime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Books"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "456d0b57-c02c-4b25-8404-11e6d9a0d1bf"
            }
          ]
        },
        {
          "id": "18f21385-0b56-4b45-9e5a-fde168a40b58",
          "name": "getUserBusinessActivities",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/business_activities?100=100",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Business Activities"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7700b57-67ed-4143-9b06-2dcf2464f0f5"
            }
          ]
        },
        {
          "id": "d9de1b04-4983-4673-b094-905f064d4875",
          "name": "getUserBusinesses",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/businesses?permitted_rolesliststring=permitted_rolesliststring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Businesses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "832ecb48-d5d9-401a-939b-e713923159f0"
            }
          ]
        },
        {
          "id": "e9df691d-a913-4c91-ac96-18a9778de33a",
          "name": "getUserConversations",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/conversations?100=100&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Conversations"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9138225c-2645-4219-9f82-5e5e556ca6ef"
            }
          ]
        },
        {
          "id": "6f8a28a2-9aae-44cf-95de-003fecd18497",
          "name": "getUserCustomLabels",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/custom_labels?100=100&210=210",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Custom Labels"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e80ed82e-d596-4f78-b3bd-a5533149d07f"
            }
          ]
        },
        {
          "id": "a3d2db26-a020-4532-b740-320df708d578",
          "name": "getUserDomains",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/domains?110=110",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Domains"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "373fd565-3417-4710-97fd-928eab878c6c"
            }
          ]
        },
        {
          "id": "7b8616ae-1c6e-48fb-adab-4aa7d89c4c97",
          "name": "getUserEvents",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/events?rsvp_statusstring=rsvp_statusstring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Events"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff3a9029-afbf-4273-998a-2bd7335ab173"
            }
          ]
        },
        {
          "id": "27b22e3a-8bc4-40b6-a6d8-bdaeab155ac7",
          "name": "getUserFamily",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/family?relationshipstring=relationshipstring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Family"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1185e7c0-8165-4a93-a0b0-9e11044cafcc"
            }
          ]
        },
        {
          "id": "9c1dbf40-fc99-4037-bdf6-1a5babcbe4e5",
          "name": "getUserFavoriteRequests",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/favorite_requests?100=100&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Favorite Requests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29d5b266-9160-4832-8c7e-64b5901de714"
            }
          ]
        },
        {
          "id": "f9eddc32-4b4c-4a30-abfd-f2c021e0fc78",
          "name": "getUserFriendlists",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/friendlists?100=100",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Friendlists"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2805ca0b-96e8-479a-aff1-285c3620eacf"
            }
          ]
        },
        {
          "id": "9c7f57b5-5c2b-4c47-adfd-b5b411fd0bb7",
          "name": "getUserGames",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/games?created_timedatetime=created_timedatetime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Games"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd0172b8-413a-4377-9074-95c700e860f6"
            }
          ]
        },
        {
          "id": "bc950f31-4044-4513-b5fe-4aef972c2da8",
          "name": "getUserGroups",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/groups?administratorbool=administratorbool&bookmark_orderunsigned int32=bookmark_orderunsigned%20int32&unreadunsigned int32=unreadunsigned%20int32",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Groups"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60145066-6f99-477b-8323-2643432ecdab"
            }
          ]
        },
        {
          "id": "153597d0-eb65-4513-8bfc-07a236ea1d2b",
          "name": "getUserSForApps",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/ids_for_apps?100=100&1203=1203",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Ids For Apps"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4d92b9a-d300-410b-adc4-3a8e12cbf289"
            }
          ]
        },
        {
          "id": "0b8c0377-1d1b-4747-a0f4-79248ad1abbd",
          "name": "getUserSForBusiness",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/ids_for_business?100=100&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User IDs for Business"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64c6dbe4-0e88-4836-a03d-88aeb4919650"
            }
          ]
        },
        {
          "id": "b21928ca-8f8b-402f-b476-7ad4f35408f6",
          "name": "getUserSForPages",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/ids_for_pages?100=100",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Ids For Pages"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f0df9b9-6ff1-4a51-b732-eed76d7302cf"
            }
          ]
        },
        {
          "id": "09bcf329-0115-40e8-808e-43811d43d72a",
          "name": "getUserInvitableFriends",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/invitable_friends?100=100&110=110&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Invitable Friends"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c378ced-acb8-4d1d-ab28-9e6c4cb3ebd5"
            }
          ]
        },
        {
          "id": "70aa2e8a-40d6-4312-a13a-ec0023878f4f",
          "name": "getUserLeadgenForms",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/leadgen_forms?100=100&200=200&275=275&278=278",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Leadgen Forms"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bfd9309e-b973-4a26-8a0b-971416faad19"
            }
          ]
        },
        {
          "id": "ddc70443-f141-4791-b4a3-b508a9ca5eb7",
          "name": "getUserLiveVeos",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/live_videos?100=100&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Live Videos"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5331b90-93d3-4ea9-b854-29173289e1d6"
            }
          ]
        },
        {
          "id": "428d00f7-3411-4f35-bc85-c114cc7b926c",
          "name": "getUserMovies",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/movies?created_timedatetime=created_timedatetime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Movies"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "722e3537-a973-497f-8ef1-b460210386ad"
            }
          ]
        },
        {
          "id": "44a59e49-8187-463c-8c87-8c5ef87cef67",
          "name": "getUserMusic",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/music?created_timedatetime=created_timedatetime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Music"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48148bbf-2302-4769-8e67-88fe3a3ef61b"
            }
          ]
        },
        {
          "id": "9a2cbf0c-13d7-478a-a8da-ece5e3702167",
          "name": "getUserPermissions",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/permissions?100=100&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Permissions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8e19eb2-a225-4cec-8763-c0fd14ac845d"
            }
          ]
        },
        {
          "id": "d5120163-769b-4d36-9438-25542b5685d9",
          "name": "getUserPersonalAdAccounts",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/personal_ad_accounts?total_countunsigned int32=total_countunsigned%20int32",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Personal Ad Accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10f5d836-2bc6-4c29-ab26-5842608589ba"
            }
          ]
        },
        {
          "id": "f3d00daa-2986-4223-8df7-4ac327b9fc73",
          "name": "getUserPhotos",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/photos?100=100&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Photos"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e043953-390b-4d3b-8fe7-c3e7e0885916"
            }
          ]
        },
        {
          "id": "56243bb5-cf21-4bbe-8cfd-ba6a3cc4125c",
          "name": "getUserPicture",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/picture?100=100&1203=1203&159=159&200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Picture"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ce7e8c7-1e35-40d2-9886-5a9535e48e74"
            }
          ]
        },
        {
          "id": "cf44dda1-4332-416e-b49c-ffd99224bf5c",
          "name": "getUserPromotableDomains",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/promotable_domains?200=200&275=275&278=278",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Promotable Domains"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6cf6837-cd07-42ca-994a-751219207044"
            }
          ]
        },
        {
          "id": "20c77922-fea8-4a78-a41d-8d398cf1dc05",
          "name": "getUserPromotableEvents",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/promotable_events?100=100&200=200&270=270&275=275&278=278",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Promotable Events"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2cf9f702-18c9-4882-aa7c-dabc432c376e"
            }
          ]
        },
        {
          "id": "fff1ce0d-2f5a-46e6-94b7-49f6c15e86f9",
          "name": "getUserRequestHistory",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/request_history?200=200",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Request History"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8937f66d-1a13-42cc-9891-4d2a9127d4f5"
            }
          ]
        },
        {
          "id": "251fecf0-b5ca-42d9-96c1-83b25df34ad1",
          "name": "getUserRichMediaDocuments",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/rich_media_documents?100=100",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Rich Media Documents"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26fa46d4-dc50-45c9-84f3-1304c0227350"
            }
          ]
        }
      ]
    },
    {
      "name": "Veo",
      "item": [
        {
          "id": "596e43c5-74eb-4772-ac62-c3279466f551",
          "name": "getVeo",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;video-id&#125;?ad_breakslistinteger=ad_breakslistinteger&backdated_timedatetime=backdated_timedatetime&backdated_time_granularityenum=backdated_time_granularityenum&content_categoryenum=content_categoryenum&content_tagslistnumeric string=content_tagslistnumeric%20string&created_timedatetime=created_timedatetime&custom_labelsliststring=custom_labelsliststring&descriptionstring=descriptionstring&embeddablebool=embeddablebool&embed_htmlstring=embed_htmlstring&eventEvent=eventEvent&formatlistVideoFormat=formatlistVideoFormat&fromUser|Page=fromUser%7CPage&iconstring=iconstring&idnumeric string=idnumeric%20string&is_crossposting_eligiblebool=is_crossposting_eligiblebool&is_crosspost_videobool=is_crosspost_videobool&is_instagram_eligiblebool=is_instagram_eligiblebool&lengthfloat=lengthfloat&live_statusenum=live_statusenum&permalink_urlstring=permalink_urlstring&picturestring=picturestring&placePlace=placePlace&privacyPrivacy=privacyPrivacy&publishedbool=publishedbool&scheduled_publish_timedatetime=scheduled_publish_timedatetime&sourcestring=sourcestring&statusVideoStatus=statusVideoStatus&titlestring=titlestring&universal_video_idstring=universal_video_idstring&updated_timedatetime=updated_timedatetime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Video"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47f65f83-91c8-4b32-83a7-5bb728734595"
            }
          ]
        },
        {
          "id": "d1b36503-a41b-45be-8c90-1e3b4b72e643",
          "name": "getVeoCopyrightRule",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;video-copyright-rule-id&#125;?condition_groupslistVideoCopyrightConditionGroup=condition_groupslistVideoCopyrightConditionGroup&copyrightslistnumeric string=copyrightslistnumeric%20string&created_datedatetime=created_datedatetime&creatorUser=creatorUser&idnumeric string=idnumeric%20string&is_in_migrationbool=is_in_migrationbool&namestring=namestring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Video Copyright Rule"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acb9f3b4-f115-4d7e-9cc3-d2dd6ba521a6"
            }
          ]
        },
        {
          "id": "7ec40f39-6240-414b-ac7e-80aa235e3118",
          "name": "getVeoList",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;video-list-id&#125;?creation_timedatetime=creation_timedatetime&descriptionstring=descriptionstring&idnumeric string=idnumeric%20string&last_modifieddatetime=last_modifieddatetime&ownerUser|Page=ownerUser%7CPage&season_numberint32=season_numberint32&thumbnailstring=thumbnailstring&titlestring=titlestring&videos_countint32=videos_countint32",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Video List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d076039-f73b-40e2-8979-6240ecc1f440"
            }
          ]
        }
      ]
    },
    {
      "name": "Asset3d",
      "item": [
        {
          "id": "239be073-06c8-4227-ba12-18982421b297",
          "name": "getWithAsset3d",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;with-asset3d-id&#125;?idnumeric string=idnumeric%20string",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "With Asset3d"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b1093dd-0b9f-459b-b9e4-af7ba4719ceb"
            }
          ]
        }
      ]
    },
    {
      "name": "Work",
      "item": [
        {
          "id": "bde14032-49ae-484e-ae85-5e768e3a152a",
          "name": "getWorkExperience",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;work-experience-id&#125;?descriptionstring=descriptionstring&employerPage=employerPage&end_datestring=end_datestring&fromUser=fromUser&idnumeric string=idnumeric%20string&locationPage=locationPage&positionPage=positionPage&projectslistProjectExperience=projectslistProjectExperience&start_datestring=start_datestring&withlistUser=withlistUser",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Work Experience"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d345e41-3fe7-419c-8c62-26b87b7124e1"
            }
          ]
        }
      ]
    },
    {
      "name": "App",
      "item": [
        {
          "id": "5c49b36e-0c4b-4088-9a4f-7f8444cf2d76",
          "name": "getAppRequest",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;app-request-id&#125;?action_typestring=action_typestring&applicationApplication=applicationApplication&created_timedatetime=created_timedatetime&datastring=datastring&fromUser=fromUser&idtoken with structure: ID or ID or ID=idtoken%20with%20structure%3A%20ID%20or%20ID%20or%20ID&messagestring=messagestring&objectOpenGraphObject:generic=objectOpenGraphObject%3Ageneric&toUser=toUser",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "App Request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29968414-da22-4328-ab05-928a51ddefa3"
            }
          ]
        }
      ]
    },
    {
      "name": "Async",
      "item": [
        {
          "id": "1ef959cc-3532-4f7b-86b6-6ff2ed1e8772",
          "name": "getAsyncSession",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;async-session-id&#125;?appApplication=appApplication&complete_timedatetime=complete_timedatetime&error_codeinteger=error_codeinteger&exceptionstring=exceptionstring&idnumeric string=idnumeric%20string&methodenum=methodenum&namestring=namestring&pagePage=pagePage&percent_completedinteger=percent_completedinteger&platform_versionenum=platform_versionenum&resultstring=resultstring&start_timedatetime=start_timedatetime&statusenum=statusenum&uristring=uristring&userUser=userUser",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Async Session"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57317658-f6bf-476d-af8c-8bd92d19e437"
            }
          ]
        }
      ]
    }
  ]
}