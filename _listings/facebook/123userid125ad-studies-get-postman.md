{
  "info": {
    "name": "Facebook Get User Ad Studies",
    "_postman_id": "653f79c5-d0f2-4fd2-8733-090bc72975c8",
    "description": "User Ad Studies",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Object",
      "item": [
        {
          "id": "3871f47e-32cc-48aa-90b3-916206f38e8a",
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
              "id": "7f6ec36d-d26a-4692-a572-680f8d13da75"
            }
          ]
        },
        {
          "id": "42463dd1-4fc4-40a4-b4b1-6ba8b8b66c91",
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
              "id": "46949da2-761b-4f5f-a7ac-e82b13fdf195"
            }
          ]
        },
        {
          "id": "9ddedd5b-0f07-44b0-826a-0dee71084fe6",
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
              "id": "09f6e464-0f23-467d-9401-5a61e755e64d"
            }
          ]
        },
        {
          "id": "c8ec4e4c-48bf-46b2-8835-bba2c4000045",
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
              "id": "8ecb294d-6925-4ed5-b8f7-71291838c719"
            }
          ]
        },
        {
          "id": "8e16e7d3-5308-4d08-8d3e-b9f3532c53e2",
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
              "id": "35b4490e-a1b8-4ac9-b76d-5cad8129cde5"
            }
          ]
        },
        {
          "id": "5960eefd-affe-440c-b320-02638728fb58",
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
              "id": "d0d8ad24-3430-4485-9303-f2ab8ab64eae"
            }
          ]
        },
        {
          "id": "786e4551-363a-4b54-adce-d740e7d14833",
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
              "id": "e87806c4-c037-4ecd-b9ef-a4fd6b045fd9"
            }
          ]
        }
      ]
    },
    {
      "name": "Achievement",
      "item": [
        {
          "id": "8c22471a-1988-4bdb-b076-c13e96151edc",
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
              "id": "0b769673-970e-4a4e-9987-a0317248a0fb"
            }
          ]
        }
      ]
    },
    {
      "name": "Album",
      "item": [
        {
          "id": "87bff2ae-3544-4905-a965-0a0d957645fe",
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
              "id": "43c0c62c-97bf-490c-8bb6-acb30504e4dc"
            }
          ]
        },
        {
          "id": "9adfd29e-5ed7-45ed-9ee8-018e6f8d71a6",
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
              "id": "907d2028-e84a-41d4-9960-53c6cb56c96f"
            }
          ]
        },
        {
          "id": "8223e4ec-8702-4448-accb-1dd395e29f2c",
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
              "id": "7dd9f9ef-d7a4-472a-bbd8-3f779c8e3f48"
            }
          ]
        }
      ]
    },
    {
      "name": "Canvas",
      "item": [
        {
          "id": "bb367a78-4728-4958-aa7f-abf615df0546",
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
              "id": "89de79c6-5cc8-45e3-b1ba-121ac2b5d00e"
            }
          ]
        },
        {
          "id": "67ceab94-a42e-40a9-98a9-ae6326a5321b",
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
              "id": "ef1b8293-5387-4f1b-b90a-25f22dc18196"
            }
          ]
        },
        {
          "id": "4f8386fe-0fb3-4505-9f11-c681a0d24627",
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
              "id": "db87da21-577f-423d-8a81-6a9b075c4004"
            }
          ]
        },
        {
          "id": "5f4ee670-5793-4d99-a642-5032d127c826",
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
              "id": "d2f794b3-ed0c-4bce-9be7-ca962f364e4a"
            }
          ]
        },
        {
          "id": "f8704437-6021-4eed-ae7d-e7e8c032f04b",
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
              "id": "12cadb13-4fe9-4150-9554-de69bf823ea3"
            }
          ]
        },
        {
          "id": "66ff0b73-b78b-4968-ab0b-f66ee5af1bcc",
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
              "id": "e316b177-eac2-4862-8e46-1b035f35ad86"
            }
          ]
        },
        {
          "id": "4bc0ec6b-21ac-454e-8337-cecf75c87b36",
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
              "id": "3e0fa7c8-da3d-4142-985a-7056f1ea5044"
            }
          ]
        },
        {
          "id": "272355c6-86d9-4afd-8ca7-b75059892176",
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
              "id": "f796741d-4750-482f-a14c-7f6536b27e9b"
            }
          ]
        },
        {
          "id": "1d75349f-f01e-4d4a-ab21-42edfa5e3cee",
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
              "id": "e2c22829-a2ba-4cd7-b0ff-a071be8d5fdf"
            }
          ]
        },
        {
          "id": "ee287362-481e-45ec-8795-7c2fd2a64143",
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
              "id": "11b92435-671b-4f5c-9c5b-143bc08cfb5c"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "953d1725-686b-4240-831b-f090df270e67",
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
              "id": "5dd73958-dece-4511-86ec-a4c517d7ee40"
            }
          ]
        },
        {
          "id": "c61a6e9e-0f4a-468a-946c-bd8847187579",
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
              "id": "8feb024e-d087-431a-acfb-71205e8c019f"
            }
          ]
        }
      ]
    },
    {
      "name": "Analytics",
      "item": [
        {
          "id": "d793d991-3a32-4717-9aa1-70aec9d962b9",
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
              "id": "fcd7b3b5-71ab-4a81-83b5-e922921ff97e"
            }
          ]
        }
      ]
    },
    {
      "name": "Audience",
      "item": [
        {
          "id": "d9a00da6-b176-4281-a2f9-1899ef371f14",
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
              "id": "7b079547-9363-4974-8868-b86f27509e10"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "6e0c0c02-f8e2-4079-bd87-8fac8f968ce2",
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
              "id": "d7b0b2bd-7f7f-4d16-83d7-f69c566ccd15"
            }
          ]
        },
        {
          "id": "5f786cba-4b15-46ba-a941-a71db34854b6",
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
              "id": "d45cca04-44d8-47c8-8004-6afaad2fe924"
            }
          ]
        },
        {
          "id": "4fe80455-019e-4167-b303-b3dbd29434da",
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
              "id": "5d7d6717-5fa3-4561-b0b8-5ce1e829278c"
            }
          ]
        }
      ]
    },
    {
      "name": "Conversation",
      "item": [
        {
          "id": "a9022637-c6b8-4b1b-91bd-9f26608af329",
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
              "id": "2fbd1058-f601-4e99-9e80-f31bcea24a39"
            }
          ]
        },
        {
          "id": "be0f0ee8-82c5-484c-906c-2ff790a6881a",
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
              "id": "9680963e-3fec-49b5-b18f-0199c578e94e"
            }
          ]
        },
        {
          "id": "3c5f6638-a066-4f00-969d-acbd85b187a3",
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
              "id": "4aa049da-f09c-45d6-a7ca-3c08cd8e562d"
            }
          ]
        }
      ]
    },
    {
      "name": "Debug",
      "item": [
        {
          "id": "934e6efd-c94c-4e02-8932-126728e37f0f",
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
              "id": "91944c19-1743-4d3c-bbfc-c8285ceb4acb"
            }
          ]
        }
      ]
    },
    {
      "name": "Doc",
      "item": [
        {
          "id": "3b9be3ed-cf24-4b27-b878-ee9a50141aa7",
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
              "id": "abb1cdc5-8a6f-4bf1-8566-a9461564aa98"
            }
          ]
        }
      ]
    },
    {
      "name": "Domain",
      "item": [
        {
          "id": "831e42a3-35b9-437e-a657-e310a83bcde3",
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
              "id": "e35d7e17-b1cf-4dc1-92a5-91ff61960274"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "78fd2155-1f27-4007-858d-e03eb683a706",
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
              "id": "2074606c-c4db-40b7-a065-e2c7add544c7"
            }
          ]
        }
      ]
    },
    {
      "name": "Friend",
      "item": [
        {
          "id": "701592d8-be10-4744-8416-59d020d42031",
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
              "id": "23e1a162-a506-4d03-a59a-7270c257ae96"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "2da4c8b8-6477-4c5a-aa7d-9e94ecdc0131",
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
              "id": "b468171d-5086-415b-bc04-9cdc20603145"
            }
          ]
        },
        {
          "id": "d50d31a2-9a47-472b-83f4-d6d49465c3a5",
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
              "id": "07d70495-686e-4ae7-925c-a5c35dd5f3be"
            }
          ]
        },
        {
          "id": "1ed512a1-6e82-49e1-a023-c5c9fc4489a3",
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
              "id": "ffe65cb7-83d0-4da3-acd3-6c5c045c86b4"
            }
          ]
        },
        {
          "id": "ba7faa98-7de1-456d-ad85-24988bdb49f0",
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
              "id": "8b60d197-d744-482d-9213-d6496ddb356d"
            }
          ]
        },
        {
          "id": "de085b59-08fd-4f1d-ad9a-3851ebcb770e",
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
              "id": "23309385-f230-46ec-893e-64beb7bea140"
            }
          ]
        },
        {
          "id": "0ae8c863-19f6-4b02-988c-148fa065cdd0",
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
              "id": "f060454b-ce3c-45ff-922a-ea5c621b9a5d"
            }
          ]
        },
        {
          "id": "3833e78e-39c0-4d9d-90c9-36ebfbcf1642",
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
              "id": "86e97578-9cf7-4cc9-b026-3d7175d08964"
            }
          ]
        },
        {
          "id": "d0c1f77b-a971-460d-b1a0-f23d4c54af47",
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
              "id": "c2446231-fa9e-4e41-9337-4eacc054a9ec"
            }
          ]
        },
        {
          "id": "413fffdc-1e8c-4283-b0f1-9b4806e5ec29",
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
              "id": "14a3ced9-1b05-477b-b3f5-bf793c512480"
            }
          ]
        },
        {
          "id": "4366b781-20f6-4af8-8e60-89be877e85a1",
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
              "id": "c53e5053-d736-4623-a760-e1fd8312b8b6"
            }
          ]
        }
      ]
    },
    {
      "name": "Me",
      "item": [
        {
          "id": "7a4593d7-32de-4103-9d1a-1694e5b5a802",
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
              "id": "7ff48897-5130-467f-ad40-bb4014e2615e"
            }
          ]
        }
      ]
    },
    {
      "name": "Life",
      "item": [
        {
          "id": "2d90ff15-414d-4d0f-b7ab-e2ab36db8369",
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
              "id": "ff75c057-49df-4289-a03f-8fd0c03a43cc"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "3b8eddc7-ce02-4acd-9707-a297d624d1a8",
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
              "id": "3ec96a98-32e8-44cb-919a-fd46bf360653"
            }
          ]
        },
        {
          "id": "f9165564-134b-452e-9da8-72c1f7081a49",
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
              "id": "9624b5bc-963a-49d8-941a-5c7f44fde655"
            }
          ]
        }
      ]
    },
    {
      "name": "Live",
      "item": [
        {
          "id": "7d25b87b-d595-480c-89a3-7c3f7bb392ac",
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
              "id": "14e37dff-bc8c-4966-b365-6e91d9d4a8e9"
            }
          ]
        }
      ]
    },
    {
      "name": "Mailing",
      "item": [
        {
          "id": "f4d518cd-7c1b-45ad-8218-05b430696ba7",
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
              "id": "f2e9a361-107d-4fe1-a3c0-e82f62ddbf9b"
            }
          ]
        }
      ]
    },
    {
      "name": "Message",
      "item": [
        {
          "id": "8940f0d1-7daa-429b-bead-b79cc7ee8138",
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
              "id": "238dbfb7-2faf-454b-9dfa-ff47ed04bda8"
            }
          ]
        },
        {
          "id": "191cbac8-cb69-4a7d-b7f5-8c9a753c0594",
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
              "id": "8283e1a7-25ff-4fa4-8df5-746591a621f5"
            }
          ]
        },
        {
          "id": "2c4ef6d7-25f3-4bd9-bc13-c68ec47871cd",
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
              "id": "2715a0ad-0693-4b64-9a7b-56e8a851a7c0"
            }
          ]
        }
      ]
    },
    {
      "name": "Milestone",
      "item": [
        {
          "id": "ec6215e7-a22c-4b2f-b91c-2b1f0161656b",
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
              "id": "8da18d20-4394-4e31-baf6-b0a5fcd3c2e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Notification",
      "item": [
        {
          "id": "44fea125-d8aa-42ea-945a-e3f9ded6ad62",
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
              "id": "0a8c3de5-a352-459a-b98f-a2ce7734abfe"
            }
          ]
        }
      ]
    },
    {
      "name": "Open",
      "item": [
        {
          "id": "0a7f806b-e717-4d65-8e75-06ed177675d6",
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
              "id": "4f732383-86c0-4b2a-8a03-50fa5dc8b6a9"
            }
          ]
        },
        {
          "id": "42da4742-7e9e-42ef-aaf2-f8e7eeffeb29",
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
              "id": "a6a96dfd-9439-4047-a071-e0b8a0fdb7fb"
            }
          ]
        },
        {
          "id": "07b31eac-744a-4792-976e-731ff36ef371",
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
              "id": "9a16310e-877a-4a6d-9a37-f1de4543cd7f"
            }
          ]
        }
      ]
    },
    {
      "name": "Page",
      "item": [
        {
          "id": "eb4eacd1-02a2-4880-a364-1f5d8a47a9e1",
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
              "id": "b25977ad-96f6-42bf-8afc-e7ef888239a0"
            }
          ]
        },
        {
          "id": "ee50c7db-6bd9-42c4-8bf2-ed80bed0ac9d",
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
              "id": "258c9f25-8ece-4ad6-aba3-3d8ebb1c0f08"
            }
          ]
        },
        {
          "id": "fc7fdf27-60ae-42d1-b632-fbb142d4cf97",
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
              "id": "f867428f-7d13-46b0-9af6-7580779a6796"
            }
          ]
        }
      ]
    },
    {
      "name": "Pages",
      "item": [
        {
          "id": "a39674f7-b1f7-4d71-9fe5-b1c5b5819890",
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
              "id": "8161b1d3-b97f-4991-bdf9-84bcf6faf4ad"
            }
          ]
        }
      ]
    },
    {
      "name": "Payment",
      "item": [
        {
          "id": "75a48635-4a95-41cc-8bb1-a27b5c8b77a8",
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
              "id": "31d0b064-7007-4918-bd22-884589688f57"
            }
          ]
        },
        {
          "id": "b74b9e6d-924a-4166-a496-4e78500c598a",
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
              "id": "33722014-26d7-4d73-9850-f610574fde9d"
            }
          ]
        },
        {
          "id": "7acdb6cd-ec9e-4160-b8e6-247b627885bc",
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
              "id": "dff92bf3-52f6-4a25-bf50-a81d222c20d4"
            }
          ]
        }
      ]
    },
    {
      "name": "Place",
      "item": [
        {
          "id": "7b509be3-370b-40c3-98df-9a662d4734c9",
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
              "id": "c725259c-94eb-4acb-9e1c-c3cb197c2a9a"
            }
          ]
        },
        {
          "id": "76d2558c-7221-46b4-be6a-2929b541e504",
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
              "id": "0c6f7337-b929-4546-b01f-a466e8d63b24"
            }
          ]
        }
      ]
    },
    {
      "name": "Posts",
      "item": [
        {
          "id": "5340cafb-8c5b-4af1-8a49-cb4b2f289df2",
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
              "id": "395c0dee-6d42-4fb9-805f-c4dfc19fa39b"
            }
          ]
        },
        {
          "id": "fc17f665-2485-4ef2-8285-4ee7db20e59e",
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
              "id": "c91926fe-0727-4afd-a079-31a05f3f4ac4"
            }
          ]
        },
        {
          "id": "f606429e-c79d-4ccd-91ce-55bd289cdbb3",
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
              "id": "c1a06878-6d17-4fa9-8c05-f622c0b8c8f8"
            }
          ]
        }
      ]
    },
    {
      "name": "Attachments",
      "item": [
        {
          "id": "94f1eae4-082b-41d3-98c4-d4782df11e86",
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
              "id": "a39de0c1-0e06-4daf-94a5-6d98954a68bc"
            }
          ]
        }
      ]
    },
    {
      "name": "Promotion",
      "item": [
        {
          "id": "519df5f6-cd32-421a-a46e-bb3802dc0b59",
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
              "id": "1d14ee74-106b-4fa3-82e0-5af1cb0739ff"
            }
          ]
        }
      ]
    },
    {
      "name": "Rtb",
      "item": [
        {
          "id": "c7470b82-9173-4f5d-8305-dd48daf7435e",
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
              "id": "e3dc506d-515a-4aaf-83f7-646f60e93058"
            }
          ]
        }
      ]
    },
    {
      "name": "Request",
      "item": [
        {
          "id": "d1608082-9278-4cf0-9f79-4fe2db9bd58c",
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
              "id": "fad97b85-b18c-45af-a5e3-08fc8c815314"
            }
          ]
        },
        {
          "id": "f8376370-8ce5-4b02-92f9-b08e068f0134",
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
              "id": "bc9c1c8f-aaf4-40d7-ba50-dca6cca280b5"
            }
          ]
        }
      ]
    },
    {
      "name": "Sales",
      "item": [
        {
          "id": "fe8f0b36-cb42-46e1-9158-f35f55bf21a6",
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
              "id": "109d058f-7884-430c-b724-3484e15a9554"
            }
          ]
        }
      ]
    },
    {
      "name": "Saved",
      "item": [
        {
          "id": "a4bc76fb-18a8-4cf4-a103-aebbbb1eaf84",
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
              "id": "708bdb6a-9690-4040-949f-fde4dde297bb"
            }
          ]
        }
      ]
    },
    {
      "name": "Status",
      "item": [
        {
          "id": "f9dccfa0-435b-46cb-a1d4-fd499f269012",
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
              "id": "25ffd9d8-b916-4751-814a-bd7f35e7bd73"
            }
          ]
        }
      ]
    },
    {
      "name": "From.",
      "item": [
        {
          "id": "f1acd8d2-9337-400b-8388-24732bf064f3",
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
              "id": "2c1941d5-d0b4-4cfb-bf4f-b496af568e31"
            }
          ]
        },
        {
          "id": "fcb48a48-7901-44a7-adbf-73961e1c4faf",
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
              "id": "e73f530a-bee4-4f0b-87bf-dfc6dd357118"
            }
          ]
        }
      ]
    },
    {
      "name": "Test",
      "item": [
        {
          "id": "6fd1123b-e191-4883-aed0-54021f6d3f21",
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
              "id": "c1905623-c767-4b88-bc51-4c8317ee018f"
            }
          ]
        },
        {
          "id": "6a82cc69-341a-4c98-bd9d-8ba1a5e7b49c",
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
              "id": "3999aa6b-8f30-4af2-b5f6-85bc2c3af053"
            }
          ]
        },
        {
          "id": "e36f77a5-7359-4cad-ab4d-d788d95c2a53",
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
              "id": "e6776c1f-f2b7-42b4-ac48-4c09b2c32ced"
            }
          ]
        }
      ]
    },
    {
      "name": "Thread",
      "item": [
        {
          "id": "74b20c6a-f47a-498a-86b0-c11b01634b64",
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
              "id": "5c1df901-4306-4a90-8460-b144c288d278"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "d77b1741-cb4c-4d50-9cfd-c69e8985a96f",
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
              "id": "0ce9235a-2e2c-41ff-b853-97f7c5e1b6f2"
            }
          ]
        },
        {
          "id": "d5192965-22c0-4ecd-a39d-e473fc4a4808",
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
              "id": "aa188b2c-6533-4432-833c-adcf02419dd9"
            }
          ]
        },
        {
          "id": "af7bfa37-177a-4ecf-86d5-038d8125383f",
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
              "id": "22e975c0-1227-4894-93b8-6a567263761e"
            }
          ]
        },
        {
          "id": "680eca5f-0593-4bd1-b0c0-aca4df52a512",
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
              "id": "93e2e21b-9623-4a98-aea9-222db208adf5"
            }
          ]
        }
      ]
    },
    {
      "name": "Veo",
      "item": [
        {
          "id": "0e75bb6c-4575-4afe-abea-a294001c64fd",
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
              "id": "9a94eaa3-5b43-4135-b859-620450158c39"
            }
          ]
        },
        {
          "id": "c0c61cd0-f8fb-4c0f-8f3e-f3dc352e7854",
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
              "id": "4a35dff7-122b-4d70-8fa9-3bf8b33070fe"
            }
          ]
        },
        {
          "id": "80bfa290-69d8-4b05-b31a-43d3a5e2438a",
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
              "id": "c49ae1c2-040c-49bc-86a1-f9f75d12564d"
            }
          ]
        }
      ]
    },
    {
      "name": "Asset3d",
      "item": [
        {
          "id": "4fd2d5ee-de43-42fa-8350-b4ade975071f",
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
              "id": "1154b981-007b-4393-a9db-ed280b5c89c0"
            }
          ]
        }
      ]
    },
    {
      "name": "Work",
      "item": [
        {
          "id": "0e9246ae-ebd5-4917-bd09-b13df285a454",
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
              "id": "e45acd66-47a6-4043-a03e-00a2188134ee"
            }
          ]
        }
      ]
    },
    {
      "name": "App",
      "item": [
        {
          "id": "1869e0f6-6610-4c05-88cb-b55f91babc7b",
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
              "id": "180d3efc-33e0-42a1-8046-23f141852cc9"
            }
          ]
        }
      ]
    },
    {
      "name": "Async",
      "item": [
        {
          "id": "a088eaf9-5e02-4063-b84f-dbdcac1d1125",
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
              "id": "4001bc62-6cfa-4704-a07f-dc39dad1dbce"
            }
          ]
        }
      ]
    }
  ]
}