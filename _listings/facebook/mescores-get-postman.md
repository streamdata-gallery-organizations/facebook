{
  "info": {
    "name": "Facebook Get Me Scores",
    "_postman_id": "b07a5717-b867-4849-90ab-7baa5a180bb6",
    "description": "As of April 4, 2018, this endpoint only returns an empty data set. Please see the changelog for more information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Object",
      "item": [
        {
          "id": "839a76f3-e38c-4947-828e-7633b8a91976",
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
              "id": "87b09acd-b7fe-45d4-8ab6-7c5242f90edc"
            }
          ]
        },
        {
          "id": "79117836-2bd0-4fab-9978-097bd36d6059",
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
              "id": "53ea8917-cc7a-4b92-86d3-090f93579462"
            }
          ]
        },
        {
          "id": "3e98f18f-e7fa-4238-8968-8fdcb934df6d",
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
              "id": "593d1838-3dc1-4966-a3b5-15587a810cd0"
            }
          ]
        },
        {
          "id": "b8fbc771-2699-4ee1-8800-7f252740fba6",
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
              "id": "a4ca8fb7-9564-44ff-b318-dd97e945d7e0"
            }
          ]
        },
        {
          "id": "ccf4e15c-3a79-4402-a5a8-6ff3a1dec76b",
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
              "id": "e977f6b4-0df1-4616-862a-673edcf76e5e"
            }
          ]
        },
        {
          "id": "f1483d46-5b75-45ad-821f-e907a6b3d7e9",
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
              "id": "cce513fa-5315-40d8-a523-17fd10593a7a"
            }
          ]
        },
        {
          "id": "22a5da35-5eb7-4490-9392-73d73d85c412",
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
              "id": "6830f887-ae22-47ec-8ad1-e311123fddf2"
            }
          ]
        }
      ]
    },
    {
      "name": "Achievement",
      "item": [
        {
          "id": "34e47ae9-877f-43e6-a9c5-f837a0f24653",
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
              "id": "7853ea92-5b64-4b25-bc6b-2b19f079fb63"
            }
          ]
        }
      ]
    },
    {
      "name": "Album",
      "item": [
        {
          "id": "a5945987-341f-406d-b8d9-2c9231effc56",
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
              "id": "7c3073ea-5f2e-4f11-877f-d605265a6222"
            }
          ]
        },
        {
          "id": "80d5711c-5207-4754-bbd6-e66dde5efd93",
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
              "id": "8a62f6cc-8611-47bb-a2ee-8b5555736bfa"
            }
          ]
        },
        {
          "id": "c3d37caa-0abe-4a79-b6de-d81d5767aac8",
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
              "id": "df7d29cf-684f-44df-92a3-9499f04b5b16"
            }
          ]
        }
      ]
    },
    {
      "name": "Canvas",
      "item": [
        {
          "id": "bf96d5bd-1c39-4e79-bd5a-fb0e293018d1",
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
              "id": "8d442bc0-2d7b-49e2-9c25-115378cafc05"
            }
          ]
        },
        {
          "id": "af065378-b27e-4edd-987c-e129c1cfe20e",
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
              "id": "fd275bcd-1cf4-4e7a-ba30-03e86d7548e1"
            }
          ]
        },
        {
          "id": "03497fe8-7da4-43db-a2a4-255f457e0df3",
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
              "id": "b471030d-2d5b-4e25-a381-5a7065f5b431"
            }
          ]
        },
        {
          "id": "72ac4b37-d996-437b-b145-759f7b4d13b8",
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
              "id": "cbdcf9b0-e2cc-4aeb-99e5-40f7c9a624d1"
            }
          ]
        },
        {
          "id": "d18cc9d2-eeef-4dbf-b208-00cbe7ce497f",
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
              "id": "7f6fd3c3-a94b-478c-849e-8fc133a56e70"
            }
          ]
        },
        {
          "id": "96e20de5-98d9-4291-889c-7b14210b7a2c",
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
              "id": "4199d20e-da8a-4dc1-98c7-80868ce2a908"
            }
          ]
        },
        {
          "id": "63e04f7e-c643-41a8-8c89-414ca8d56f1a",
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
              "id": "60fe01d4-a828-46b3-ab7e-05bd01e490f5"
            }
          ]
        },
        {
          "id": "b6daa891-0a3d-47a8-8e3a-c61d12dc9988",
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
              "id": "a5656ca7-664b-48d9-811b-2d74863f724d"
            }
          ]
        },
        {
          "id": "09baa183-8b8d-4e39-b426-af77ee6d33be",
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
              "id": "26675559-0c22-4062-afb8-cff62cd746ac"
            }
          ]
        },
        {
          "id": "0f891bb2-76df-4065-ae66-a0452ace2952",
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
              "id": "9285d8f7-87dc-4164-929e-b1cfdd3acaa4"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "ac34b910-2d66-416c-95ec-b08ed531aa44",
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
              "id": "2d4f0e12-d487-4b67-ba3e-fb86849ed1e7"
            }
          ]
        },
        {
          "id": "f541c2b3-eac3-49d5-ae79-ef50f7ecdb76",
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
              "id": "93438973-8636-4f68-9161-0b21790d4474"
            }
          ]
        }
      ]
    },
    {
      "name": "Analytics",
      "item": [
        {
          "id": "417863b8-de42-4ea3-87b4-28c79608d875",
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
              "id": "8cac888c-e55a-4396-b4bd-164d95d70f97"
            }
          ]
        }
      ]
    },
    {
      "name": "Audience",
      "item": [
        {
          "id": "b2e91bd7-b0d7-4fe7-a742-c64dd95f1b3c",
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
              "id": "e473b7de-c9d9-4c7e-9ac3-848df40a74e8"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "649cfb49-6b0e-46b5-9afd-bfcdc2d2c1df",
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
              "id": "24b0f8ba-4990-4887-b8ca-62d513b06246"
            }
          ]
        },
        {
          "id": "3bcb6faa-9abb-4881-b04e-092c5b6552be",
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
              "id": "b89d6184-8114-4b49-b2a9-5c5c8cabf4e9"
            }
          ]
        },
        {
          "id": "e542c2b9-2cc3-4a81-94a3-d7c00cc010a8",
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
              "id": "745ff3b0-68a1-47fb-b899-084c4772cb1a"
            }
          ]
        }
      ]
    },
    {
      "name": "Conversation",
      "item": [
        {
          "id": "add5548a-a1b0-4ce6-919f-b85121c1b8c2",
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
              "id": "4e1b5952-d0fd-461e-b806-3c37f7e06763"
            }
          ]
        },
        {
          "id": "5c5e7179-3c35-4738-97f9-0bde43f5c958",
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
              "id": "902f098b-95cc-40ed-93dc-e67f3b7ff990"
            }
          ]
        },
        {
          "id": "f07f9ce7-c93e-47a2-a5a4-ed626caa4aea",
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
              "id": "0972b46c-4b9f-45a6-8602-8fec9bb60578"
            }
          ]
        }
      ]
    },
    {
      "name": "Debug",
      "item": [
        {
          "id": "78842298-ddf9-4acd-9750-a324b8df596a",
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
              "id": "7c050b10-f63e-4d54-adfe-efad440dd2df"
            }
          ]
        }
      ]
    },
    {
      "name": "Doc",
      "item": [
        {
          "id": "ea794e0e-d979-4a3f-ab24-816a84eafe89",
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
              "id": "f72ac355-a51e-4cc7-96ad-9265e51e495c"
            }
          ]
        }
      ]
    },
    {
      "name": "Domain",
      "item": [
        {
          "id": "d4c128e6-0514-4754-a189-9f8e56927906",
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
              "id": "7041b498-7228-4468-81f8-0d3b9039a4cc"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "fb4a60fa-a3d3-4b68-9aae-b29487a2d0f7",
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
              "id": "1756b664-92db-424e-94de-bdf28945cbc5"
            }
          ]
        }
      ]
    },
    {
      "name": "Friend",
      "item": [
        {
          "id": "33c2eb9d-563b-4d14-a159-09cba7138e3a",
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
              "id": "1f89887b-464c-40b9-9d39-d0cba8ef4cbb"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "06c79c91-7951-4e90-8130-08a90f009832",
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
              "id": "0019d15c-ef43-4bc3-9df5-78d56cf6904e"
            }
          ]
        },
        {
          "id": "4c0fd36a-f0cb-45d8-8d56-923ee288bada",
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
              "id": "c15accf5-8181-44ad-bda3-d72fbed84271"
            }
          ]
        },
        {
          "id": "387f4180-65fb-4717-8ead-3b8c6aedc453",
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
              "id": "a607b735-4a59-4db9-b009-d38c0f2ab13a"
            }
          ]
        },
        {
          "id": "06924b3f-58b6-4c24-9b6a-32d9a6abe961",
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
              "id": "d3689883-b62d-4ee0-bb69-65960ad834b2"
            }
          ]
        },
        {
          "id": "66699dbf-e1c0-4ad8-b7c6-f702d099ac5b",
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
              "id": "003de9a5-d175-484d-bb8b-a2fc1f345526"
            }
          ]
        },
        {
          "id": "34c9ea4e-0be0-440a-b77c-ee603a5ac556",
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
              "id": "ed542403-57cb-466c-a8ca-04969e436bb6"
            }
          ]
        },
        {
          "id": "8da47930-4fa1-4f90-ba09-922fb5929144",
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
              "id": "d5f373d0-3501-43d3-99fb-3a35bc60b75f"
            }
          ]
        },
        {
          "id": "1103db6f-45ee-49f9-bde9-6c5cdc0a533e",
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
              "id": "72372856-d473-433f-a315-99565c0bd803"
            }
          ]
        },
        {
          "id": "f2ec89a5-fb1d-4316-b734-edd73b27a9a0",
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
              "id": "171a7042-01a3-4342-9e32-83ef46b681bb"
            }
          ]
        },
        {
          "id": "bb76e7b8-15fe-46d1-9823-b3deedd523eb",
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
              "id": "a8450219-fefe-4ec6-ab1f-8db1084658f4"
            }
          ]
        }
      ]
    },
    {
      "name": "Me",
      "item": [
        {
          "id": "f2a0d9c7-7b59-449d-afd8-2bb2a41906ea",
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
              "id": "2760ca93-d959-4ef6-a07e-4a9dc34c91d8"
            }
          ]
        },
        {
          "id": "01969eac-a3c8-4b56-875e-466f436a41b7",
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
              "id": "12bef50d-84e5-43b9-8fdb-809319569800"
            }
          ]
        },
        {
          "id": "ad4f9894-6214-42da-b806-1beb6da1cabb",
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
              "id": "918a0051-9fbc-4d86-acce-9d82622bd5c5"
            }
          ]
        },
        {
          "id": "6aa8fa84-256b-4b8a-a479-15de7254feae",
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
              "id": "3cc45354-5936-47b1-ada4-82ecec74f668"
            }
          ]
        },
        {
          "id": "45770f25-dae2-4e87-aabf-82db1724d012",
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
              "id": "04390589-3f4c-4579-ac9c-9133ff63ac18"
            }
          ]
        },
        {
          "id": "a640b0be-e697-4c50-a035-a9f7e6411691",
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
              "id": "17452583-3b6e-43df-94d0-ae7cae2b92a7"
            }
          ]
        },
        {
          "id": "99ab4873-6cf7-456d-8060-03db606692e6",
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
              "id": "16b59088-a9cf-4d61-aa6d-53f9076f99c0"
            }
          ]
        },
        {
          "id": "40cf8b9c-28b8-4b86-b86a-3bf6db9be176",
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
              "id": "79a61a09-c476-4a7c-bc92-5a8fc5a1f6cc"
            }
          ]
        },
        {
          "id": "71c1d64e-b60c-4440-99f2-6f59498346da",
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
              "id": "25669b64-0cf5-495e-b5cd-5224c74f8e04"
            }
          ]
        }
      ]
    },
    {
      "name": "Life",
      "item": [
        {
          "id": "2f5eb7b2-ddc1-4bd1-bf32-5a33a536158d",
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
              "id": "d5ede497-a865-47b2-acb6-0a6bb3ea24e7"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "540269fa-eaf9-407b-a190-588a0beed522",
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
              "id": "e7e30fad-0a54-4c1b-8991-3cfddbfd5cc9"
            }
          ]
        },
        {
          "id": "51e61c8e-d577-4f0a-9137-fd61f0070259",
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
              "id": "f1cda693-e610-465c-90db-9b1f2df607da"
            }
          ]
        }
      ]
    },
    {
      "name": "Live",
      "item": [
        {
          "id": "99608317-26e3-4b00-a9f1-2aa677f7bf7f",
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
              "id": "0f01eb61-d0ea-41d6-99fc-b503d63bf670"
            }
          ]
        }
      ]
    },
    {
      "name": "Mailing",
      "item": [
        {
          "id": "1fba9498-6429-4e80-979e-e163e384725a",
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
              "id": "db2c2f8d-645f-4dc8-8018-e49c3e7dcaed"
            }
          ]
        }
      ]
    },
    {
      "name": "Message",
      "item": [
        {
          "id": "6836b4b8-9726-450a-956b-971bc6fbc328",
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
              "id": "06e1dac0-88ce-4e03-98e5-3933f14a1766"
            }
          ]
        },
        {
          "id": "9cc6645d-a586-4117-81ba-a612be0ae23c",
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
              "id": "6eb38b5f-2962-4440-a2a7-394367eb5fcb"
            }
          ]
        },
        {
          "id": "82002503-9133-453c-853d-64d95413593a",
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
              "id": "1698e9a0-5abe-4032-a9c2-5fc74ebd1e61"
            }
          ]
        }
      ]
    },
    {
      "name": "Milestone",
      "item": [
        {
          "id": "03e8455a-9a16-4d4b-a8b4-8bde1fb71654",
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
              "id": "62bc6e5b-7d51-4bd8-a280-3560d3ea7559"
            }
          ]
        }
      ]
    },
    {
      "name": "Notification",
      "item": [
        {
          "id": "ba775176-00d0-4f91-aebf-5f4d1d38bd1f",
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
              "id": "b565b652-e851-44d7-9e36-eec1b7f7779c"
            }
          ]
        }
      ]
    },
    {
      "name": "Open",
      "item": [
        {
          "id": "f04d4032-0603-4c14-9993-e378dafe9bdb",
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
              "id": "bf0f5635-f6ce-4957-9010-70510a1d1c64"
            }
          ]
        },
        {
          "id": "1055a4d4-4877-484d-8d64-ee3c7d4b090f",
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
              "id": "271be783-9955-4a00-9f2f-a4e8010abefc"
            }
          ]
        },
        {
          "id": "c1134efb-57da-4237-bd1c-3b74e4c20e42",
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
              "id": "be943f8c-9004-41f6-a511-c097e7e29f9b"
            }
          ]
        }
      ]
    },
    {
      "name": "Page",
      "item": [
        {
          "id": "340b311b-ba11-4a74-b157-fa1e5ef9a94f",
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
              "id": "f2eb6e09-e8a3-4b4e-aa8e-f56729ee85cb"
            }
          ]
        },
        {
          "id": "6fa41f53-dc32-44bd-b331-f879d4ecb1e1",
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
              "id": "222e7ffb-0fec-4b65-9f10-66bf7a30b7a8"
            }
          ]
        },
        {
          "id": "53a36dd9-c6c8-47da-8655-052bab69c7e1",
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
              "id": "1891065f-698e-4d01-bc29-5004dfa3fb7a"
            }
          ]
        }
      ]
    },
    {
      "name": "Pages",
      "item": [
        {
          "id": "74773609-90f8-41f8-9649-85d8d3354ceb",
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
              "id": "741faf68-d3ad-4864-9201-3bc67b5c1d68"
            }
          ]
        }
      ]
    },
    {
      "name": "Payment",
      "item": [
        {
          "id": "be08c1b3-1d20-4c37-94a4-0d6188e8fdde",
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
              "id": "7db9e61c-0044-4fac-9614-8034703c68f6"
            }
          ]
        },
        {
          "id": "220eb946-50ee-4361-ab56-c42791f6fedc",
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
              "id": "cfa3940e-3eb5-469f-8fe3-ed1ebf1769ce"
            }
          ]
        },
        {
          "id": "958c1aee-20bc-4072-a389-dfa49fe0a47f",
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
              "id": "c6ae7185-b512-4339-bc0d-c48927508e3a"
            }
          ]
        }
      ]
    },
    {
      "name": "Place",
      "item": [
        {
          "id": "1c62f4c3-b028-4390-a09e-e7a7d211377b",
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
              "id": "4c5ae29d-a877-4aa8-a280-99b0f4465b64"
            }
          ]
        },
        {
          "id": "cbe58acc-5455-4c66-9379-ec61b31c7aa7",
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
              "id": "62f9980d-562e-4be6-b3cd-84478907a984"
            }
          ]
        }
      ]
    },
    {
      "name": "Posts",
      "item": [
        {
          "id": "be2de285-1215-4e69-8bec-5408ea4b83d5",
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
              "id": "2311dc0a-f1e6-484f-88cc-eb778b8b2e47"
            }
          ]
        },
        {
          "id": "3163d289-b4b2-4b0e-8646-169330e26253",
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
              "id": "9cb308b2-c41e-4e07-884b-06add486e6f3"
            }
          ]
        },
        {
          "id": "26f64d75-cf44-495d-a9b4-1746e07a24af",
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
              "id": "9f1daee8-63da-4056-930a-72d387ef6775"
            }
          ]
        }
      ]
    },
    {
      "name": "Attachments",
      "item": [
        {
          "id": "bda941c6-07e7-4cb5-a2fe-fe07eb80a214",
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
              "id": "6dd58d95-f69b-454e-91a6-a533d74d0028"
            }
          ]
        }
      ]
    },
    {
      "name": "Promotion",
      "item": [
        {
          "id": "fc0a2a9c-c9ea-40ad-a71d-6d383c9e5e95",
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
              "id": "901abfd5-ac4e-4b33-ab62-da83cba7a482"
            }
          ]
        }
      ]
    },
    {
      "name": "Rtb",
      "item": [
        {
          "id": "979e6d6e-10d0-4f62-b9ec-fbffa0fcd1f7",
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
              "id": "004b50b5-ddbb-489e-97db-76e166d604c8"
            }
          ]
        }
      ]
    },
    {
      "name": "Request",
      "item": [
        {
          "id": "ee41e564-9e41-4088-8101-3978c0812543",
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
              "id": "9d6fc09e-73b2-44d5-b079-176106e3dad3"
            }
          ]
        },
        {
          "id": "778e3a28-ae34-41c6-8dbe-8809fd517c55",
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
              "id": "e707dba4-e9a8-490b-8537-3c723d48c7ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Sales",
      "item": [
        {
          "id": "5c109ca1-6c0f-4da5-b92a-60613de744bb",
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
              "id": "271a57cb-591b-4b03-90ec-c3d55f4ecf08"
            }
          ]
        }
      ]
    },
    {
      "name": "Saved",
      "item": [
        {
          "id": "7ef46ed1-5f61-46da-aa04-3f3d276892c9",
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
              "id": "1ac109d0-8919-4fbd-a9b5-06ab0a05940e"
            }
          ]
        }
      ]
    },
    {
      "name": "Status",
      "item": [
        {
          "id": "2365fc25-94e0-44c6-b12d-bcac19eb7a26",
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
              "id": "cd503e4c-0edc-42ef-8983-730377db7ad7"
            }
          ]
        }
      ]
    },
    {
      "name": "From.",
      "item": [
        {
          "id": "67a37f62-b777-4528-8402-792136ef311e",
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
              "id": "90895c14-83b2-4b3a-9e53-ff06ca9305d7"
            }
          ]
        },
        {
          "id": "3aff2332-48fa-489e-9738-a387cac8d314",
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
              "id": "80d0b1c9-03de-4f2d-8817-71813816334b"
            }
          ]
        }
      ]
    },
    {
      "name": "Test",
      "item": [
        {
          "id": "83fbb57e-1558-4f2d-a96a-e6aba620a30f",
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
              "id": "3824c9ee-50d4-4caa-b45b-749f61955e2b"
            }
          ]
        },
        {
          "id": "8dcc5c46-db20-47b4-8283-d4c53318c5ce",
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
              "id": "a893fa31-abab-4f8b-8817-34e3b7a746d9"
            }
          ]
        },
        {
          "id": "ea7d68a0-37a1-433b-982c-5695a64b8cdb",
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
              "id": "79532630-8f0d-4228-8be2-7be15d8da2ce"
            }
          ]
        }
      ]
    },
    {
      "name": "Thread",
      "item": [
        {
          "id": "6fae253a-58c1-4467-8f1f-afe805be3319",
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
              "id": "91367e01-6132-49c4-a007-770b2e4754d2"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "39bd29fc-8407-4b18-8a5e-c83544d7650b",
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
              "id": "566fd252-20d5-499b-a822-53cf76685908"
            }
          ]
        },
        {
          "id": "c783aa51-cd91-41c4-a8ac-f4b0d700f151",
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
              "id": "ced6b2d5-2bb8-4275-a731-f0a7c80872d3"
            }
          ]
        },
        {
          "id": "a8365826-b611-4294-90ad-8f95b8d0c60d",
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
              "id": "a789d330-ca96-477a-87a8-1e3777ca88c3"
            }
          ]
        },
        {
          "id": "b1c27d0c-4ec6-4ae3-89b3-2168be9329a3",
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
              "id": "418ebc0d-5691-4482-a304-664768c9e79e"
            }
          ]
        },
        {
          "id": "9e127bc6-d493-4d43-9f09-9cb7fe32709a",
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
              "id": "901b9d29-90f5-4c39-988e-933556b6324c"
            }
          ]
        },
        {
          "id": "fc027cb7-cfb2-493a-afcc-f301df7f5656",
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
              "id": "702dcaf5-31fe-4310-acba-5ce05f409a8e"
            }
          ]
        },
        {
          "id": "fc5142d8-3f51-490d-8b3e-ed24f1f4ef6d",
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
              "id": "f6427629-8081-494e-a779-0308374c2467"
            }
          ]
        },
        {
          "id": "0c59cb5c-2b7a-4ce7-894d-497c3f93ca56",
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
              "id": "c156d3d2-5873-445e-ac32-27f5254d300d"
            }
          ]
        },
        {
          "id": "50ea137c-a1e7-4310-b9ae-1d384b4b7543",
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
              "id": "34fed943-6036-4c08-89f2-182ef2e1ff79"
            }
          ]
        },
        {
          "id": "c524511b-d6b6-488b-808f-8dd8e8dca51f",
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
              "id": "75d3b3c9-8f60-4ede-bacc-95585a4ae61d"
            }
          ]
        },
        {
          "id": "05524698-5537-4e13-b257-7685ee46df42",
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
              "id": "23c2dc25-d4d7-4f89-9737-f151e5982880"
            }
          ]
        },
        {
          "id": "90aa10ac-52eb-4e72-85dc-a8f3d11ce3a2",
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
              "id": "e8d00e75-df22-44d3-ac7e-a436630d4186"
            }
          ]
        },
        {
          "id": "984d1600-88cd-45e6-a241-51f5ca1a402b",
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
              "id": "e2449c0e-89ec-4092-a547-16f8f9d7f4e3"
            }
          ]
        },
        {
          "id": "a23ab0cf-a2c2-456f-9ecd-9376cdacd019",
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
              "id": "6f34f3fb-aeec-4791-8d06-651a172ee1bd"
            }
          ]
        },
        {
          "id": "46e5f0ca-9fc9-4b87-80cd-dc3fcda44587",
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
              "id": "cc529ddf-30fa-4148-86d3-cdee522a384d"
            }
          ]
        },
        {
          "id": "4de17d9b-2f0b-4201-8e90-f2141b832629",
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
              "id": "9c10aba3-85d1-4d6d-8550-618545ce7c5b"
            }
          ]
        },
        {
          "id": "f3287201-5240-424d-8a83-ac954623612a",
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
              "id": "4f6e3c54-75f9-441f-8f95-f319345540b8"
            }
          ]
        },
        {
          "id": "920da4af-0c96-446a-b4d3-3ca0731bdaa9",
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
              "id": "9b3474fd-6b8c-47d4-a617-656a5cb286c7"
            }
          ]
        },
        {
          "id": "e138bdfe-fe53-4a05-9bae-3185b88fea8a",
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
              "id": "8b0fadfa-d1de-44ef-a6dc-2aea7e981173"
            }
          ]
        },
        {
          "id": "68443fd4-f96f-4e97-9e1c-df47815937af",
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
              "id": "b9964463-9983-4698-8018-a3b9d54ac640"
            }
          ]
        },
        {
          "id": "09102df4-f961-4af3-b9a6-11e3dd5bbc43",
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
              "id": "17e5de06-b663-4a9e-9382-1b0199b48082"
            }
          ]
        },
        {
          "id": "d1f36118-2b8b-4209-b1ae-a3830f069fe5",
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
              "id": "12d02816-f3f7-4c1d-a89e-a186d865bf81"
            }
          ]
        },
        {
          "id": "73c54f2c-c8f5-44d4-9ea4-030ac097fe2b",
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
              "id": "b4df2e7d-9c83-4683-bf20-942cfa335011"
            }
          ]
        },
        {
          "id": "cc969cfd-260a-4169-89df-24984dd69c3c",
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
              "id": "db0c5780-724d-4ec0-bea5-9e4a2df72875"
            }
          ]
        },
        {
          "id": "9ee0a904-87ff-445e-87f9-0c3a3a55972a",
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
              "id": "717f0827-bd71-4b61-b06e-8e73b4a3e937"
            }
          ]
        },
        {
          "id": "da068e82-8e74-4d09-882e-dd2691ee2103",
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
              "id": "3e92f0d8-c78e-4fb6-af0d-84fc4d7d1e3e"
            }
          ]
        },
        {
          "id": "35121236-4b6c-451e-af33-6f49ff03ef4b",
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
              "id": "8a927ac6-448e-4584-bb2b-d7cdbe7d71a7"
            }
          ]
        },
        {
          "id": "64196510-6836-43de-bf24-4b19ae5a6b7b",
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
              "id": "775b944e-fa7a-4928-bf1a-3a83c7018e0e"
            }
          ]
        },
        {
          "id": "38a4bbfd-3c03-4f3a-9a11-317a3154271d",
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
              "id": "c8f0d4d5-abc9-464e-bd65-19578e8880de"
            }
          ]
        },
        {
          "id": "08af6108-fd01-4481-a598-05c456ac1e36",
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
              "id": "3986c3f9-71fe-4ab5-ab20-e08808be9d74"
            }
          ]
        },
        {
          "id": "ba6961bc-a075-4099-a1b7-8f857a4c7686",
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
              "id": "3d5f21d1-cc06-492e-b8bf-d6917dc5efd8"
            }
          ]
        },
        {
          "id": "97150c6b-3c21-44e7-82b0-2e1d285beef4",
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
              "id": "209c8f59-e693-4177-aa47-82ac950b84ce"
            }
          ]
        },
        {
          "id": "da66e9b5-a0fd-4d95-b765-249518e1fa70",
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
              "id": "28b1f15e-c8f6-4c08-b301-7c3d8542f387"
            }
          ]
        },
        {
          "id": "1f796bb4-aa02-44b0-814e-50b794bd615b",
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
              "id": "6f783b0a-69e3-4b3b-8081-91a708749cbd"
            }
          ]
        },
        {
          "id": "7294fdb4-408b-4fd8-8df8-39aac7548848",
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
              "id": "e6ae45b9-792d-4dfe-8444-8850b6df79bf"
            }
          ]
        },
        {
          "id": "8cf8f4ca-7961-448e-af51-84cdb4c8eba2",
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
              "id": "74eb73d1-cc28-49f2-b01d-0f6f3a8cf1f9"
            }
          ]
        },
        {
          "id": "94c2b035-66fb-49a2-bd7b-44391f73d2d1",
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
              "id": "81e17708-ca90-4d8e-9199-d791090990c2"
            }
          ]
        },
        {
          "id": "5fc8ab46-785a-49d0-9074-7c634d47eccc",
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
              "id": "29184553-7b84-47e0-9032-9f733528a6f5"
            }
          ]
        },
        {
          "id": "cf75f502-9f4b-4beb-a841-cec97c3fd3d8",
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
              "id": "c31afab4-9f62-43ea-bcfe-6a500788c82f"
            }
          ]
        },
        {
          "id": "217a04cb-8935-4b61-8b84-1ef225fbdb14",
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
              "id": "c242b19f-f2be-4bf7-950b-ebcc50ed2c16"
            }
          ]
        },
        {
          "id": "33039aa8-d34f-434d-908b-b8761bfd04e4",
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
              "id": "ef9d7ac6-7b8b-486d-84c5-ead1de935016"
            }
          ]
        },
        {
          "id": "3082a731-c2fd-4611-a7fb-710e0f2ddfd3",
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
              "id": "bacd4125-fc1e-4e85-ba63-e379aed59022"
            }
          ]
        },
        {
          "id": "057ae8d9-ad88-4887-b28b-bf02517cf2f0",
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
              "id": "801a3e36-243d-4a76-bda6-1de44c14d240"
            }
          ]
        }
      ]
    },
    {
      "name": "Veo",
      "item": [
        {
          "id": "90452502-6921-42e2-aa6b-2db5d138a288",
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
              "id": "6f4b027d-4eef-4329-9f9d-070c01796f2e"
            }
          ]
        },
        {
          "id": "5125c15d-d2f4-46bd-913b-c36ee53b19e8",
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
              "id": "03f13496-d630-4f82-8de4-3986ad8cd326"
            }
          ]
        },
        {
          "id": "17a4ccab-c947-46ad-a64a-d756acbeb656",
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
              "id": "83bb00a7-ae50-49b9-937a-346fa5712b47"
            }
          ]
        }
      ]
    },
    {
      "name": "Asset3d",
      "item": [
        {
          "id": "13934c1d-0cda-4f94-89ac-23e2854a26ea",
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
              "id": "c2f2f320-b02c-4e2c-bc44-568585fa2534"
            }
          ]
        }
      ]
    },
    {
      "name": "Work",
      "item": [
        {
          "id": "a20a3bcc-8524-4400-829c-b75170c2674a",
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
              "id": "aca68160-5822-4fb5-b5db-03f846996e24"
            }
          ]
        }
      ]
    },
    {
      "name": "App",
      "item": [
        {
          "id": "ed5e2516-fe37-454b-8db8-59e802fb89ee",
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
              "id": "74c85391-70cc-415e-b38e-a2a0c6ee39c1"
            }
          ]
        }
      ]
    },
    {
      "name": "Async",
      "item": [
        {
          "id": "1d23716f-b147-48ae-9902-5346eec94b8c",
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
              "id": "ff9005d9-1c5d-4eae-bf67-17ae50c379f9"
            }
          ]
        }
      ]
    }
  ]
}