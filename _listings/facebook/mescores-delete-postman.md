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
            "url": "http://graph.facebook.com/v