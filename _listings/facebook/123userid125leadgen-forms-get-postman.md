{
  "info": {
    "name": "Facebook Get User Leadgen Forms",
    "_postman_id": "6d24dc58-a758-484c-8992-d4ae5e28da1f",
    "description": "User Leadgen Forms",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Object",
      "item": [
        {
          "id": "98545675-046c-43b4-b2ac-530ed6ab25ab",
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
              "id": "4a92a431-fb92-4782-ae96-a7e6fa1000ee"
            }
          ]
        },
        {
          "id": "cc589394-8d4e-4a0a-bf64-30414dfb710a",
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
              "id": "49cd290d-6c09-4b1e-9e3f-ec360c1bead6"
            }
          ]
        },
        {
          "id": "f129c0f6-76a2-45f1-b0e1-2644f5eda4c3",
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
              "id": "a5f98d2e-8754-4050-acad-ee201a058fd4"
            }
          ]
        },
        {
          "id": "aedbf641-cb52-477c-830f-f0b94c229924",
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
              "id": "9c2ea427-1048-4042-b4ee-25b804a2b41f"
            }
          ]
        },
        {
          "id": "a47ee7ce-f9fe-4be4-b356-13bc35201163",
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
              "id": "ef0b404f-8cba-4cc7-a216-f623a921970e"
            }
          ]
        },
        {
          "id": "9152c1c5-ad78-4385-b220-6f2a3d8d2229",
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
              "id": "9c989bf5-6e88-4078-a9ef-86490c4cb014"
            }
          ]
        },
        {
          "id": "82875d63-98db-41da-b179-f482ce9b03d5",
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
              "id": "b931901e-7f37-42ab-b8e5-d2dae637ad56"
            }
          ]
        }
      ]
    },
    {
      "name": "Achievement",
      "item": [
        {
          "id": "3127dc4d-6708-4833-806c-46385ee9474c",
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
              "id": "58b63352-b7ba-40e6-841c-265d89c0e4bc"
            }
          ]
        }
      ]
    },
    {
      "name": "Album",
      "item": [
        {
          "id": "eec6cb10-b465-4a28-8b2c-fe55d78ceb11",
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
              "id": "5508268c-0437-41c7-8c4b-4dd1d6ea076f"
            }
          ]
        },
        {
          "id": "58f2fe2e-2fbc-4a4d-b459-9b1aff016bb1",
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
              "id": "f63b087d-6276-464e-bb39-d423e68dfd3a"
            }
          ]
        },
        {
          "id": "1ca456d6-82d7-49d9-bb84-a1ff77d14c4a",
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
              "id": "ee1edc13-bb9c-420d-9ed7-808edd59a273"
            }
          ]
        }
      ]
    },
    {
      "name": "Canvas",
      "item": [
        {
          "id": "91bb17b9-dc74-4e32-bf87-3173b4fb4dcd",
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
              "id": "789c9597-cf38-4156-b2c5-241b57f458c4"
            }
          ]
        },
        {
          "id": "8e265744-3e4a-431c-b82e-aa0b0a617c63",
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
              "id": "afe8a99e-085f-425d-a4e9-a77b17fb212c"
            }
          ]
        },
        {
          "id": "fc0b7596-6361-4fc0-bb55-727f8a776d65",
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
              "id": "e1363c38-9c69-4739-84f7-9348b4848527"
            }
          ]
        },
        {
          "id": "e056fc51-8a13-46b2-ac94-8585f730c2c7",
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
              "id": "695f6c67-cfde-485d-9194-db52d70d5ba6"
            }
          ]
        },
        {
          "id": "930658ba-fb8b-43de-9eb3-30a725e2f7f3",
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
              "id": "659e8ce9-d172-4262-9be0-cbe4e400b79d"
            }
          ]
        },
        {
          "id": "9cd34240-90f5-40d6-a8f4-add6af34cfe9",
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
              "id": "bcfba7cc-1d67-4da6-8369-b782ff8cde28"
            }
          ]
        },
        {
          "id": "a8a5e238-8b8c-4142-935d-0afcd60739ce",
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
              "id": "f6189ae5-5150-4567-9dd5-a822423dc60d"
            }
          ]
        },
        {
          "id": "120026ff-0e7f-444a-bcd2-eead36073b7a",
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
              "id": "5dec95eb-065f-4c16-b46e-e39bca2b255c"
            }
          ]
        },
        {
          "id": "7303d07d-7cb4-4f84-a864-73cca1e62be8",
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
              "id": "738a0aa5-89f3-4bfc-ba5a-e097dbfbdac2"
            }
          ]
        },
        {
          "id": "e39ebb0e-8863-478c-b4df-289166c32abc",
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
              "id": "70e27469-6f47-48b8-ab61-5251374ac4c4"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "57fbe33e-501e-4937-bfba-0124f745672a",
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
              "id": "fffca298-0472-4cff-a975-d46f90132b76"
            }
          ]
        },
        {
          "id": "b905c3b2-22c1-46fa-a9fb-c3bbf39ee946",
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
              "id": "9683d0df-3379-41be-9699-39e39e064d38"
            }
          ]
        }
      ]
    },
    {
      "name": "Analytics",
      "item": [
        {
          "id": "9ada1e92-2b95-4f78-9c6f-ddc06ac25848",
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
              "id": "8676b3a0-b1a2-47d5-8ad0-3d16d4a7d0fb"
            }
          ]
        }
      ]
    },
    {
      "name": "Audience",
      "item": [
        {
          "id": "eaaca407-92df-4daa-bc57-485cc28883bd",
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
              "id": "f4344cce-7260-484a-8c30-01ca01fd0d3d"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "9c8d3b30-e379-4ee0-98c4-ab527e5b60df",
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
              "id": "04f8b933-9178-45cc-a863-130f216c107c"
            }
          ]
        },
        {
          "id": "6e3d4368-cc4a-4d9e-ad6e-952079d85398",
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
              "id": "963fe8cd-cf4e-4acf-a15d-0c2557a7db4f"
            }
          ]
        },
        {
          "id": "21e3341e-ff6e-4d5d-93ed-c074de250890",
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
              "id": "cb06686a-7649-42b1-b269-a3a78b905982"
            }
          ]
        }
      ]
    },
    {
      "name": "Conversation",
      "item": [
        {
          "id": "755390b2-abb8-4758-964f-c3f53d7a42b0",
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
              "id": "f56012c3-9ca9-424f-a66d-c57c2167b808"
            }
          ]
        },
        {
          "id": "9eb4ff4a-8a97-479e-aa50-624222236e33",
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
              "id": "24180534-51ff-407e-82bf-4045292c38c8"
            }
          ]
        },
        {
          "id": "64388ee3-0436-4cc7-8057-00b5346ace60",
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
              "id": "2a512d9f-6865-416d-964d-cd8fffa7bb54"
            }
          ]
        }
      ]
    },
    {
      "name": "Debug",
      "item": [
        {
          "id": "f2f41a91-16ec-410a-bcda-66db9f03e2ac",
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
              "id": "49638f13-d9ea-471a-9a85-ed06a4702afe"
            }
          ]
        }
      ]
    },
    {
      "name": "Doc",
      "item": [
        {
          "id": "2eed1abf-377d-41d8-89d3-e15e4d987182",
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
              "id": "1c66839e-58cf-47fb-ac94-a8e3b840ff7d"
            }
          ]
        }
      ]
    },
    {
      "name": "Domain",
      "item": [
        {
          "id": "7a40ad7f-efaf-402b-ac21-9ebe8d3de677",
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
              "id": "bc399ab3-d09b-486a-b086-078df8fadcb2"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "4c1a3fc7-bd28-45fa-9d2b-80026dc5a776",
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
              "id": "63240b3d-9f6a-431e-b032-73a4525aa9be"
            }
          ]
        }
      ]
    },
    {
      "name": "Friend",
      "item": [
        {
          "id": "74182743-286c-4a0a-8c1e-78bd365bb7f4",
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
              "id": "5c081678-8c31-46f2-bcf1-15faf91e26d0"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "cd87b916-65c4-4383-ba90-646b8d6e2114",
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
              "id": "a96677b6-0a01-4f2c-96ca-54b23178f757"
            }
          ]
        },
        {
          "id": "b899b1df-d990-4fc0-a007-21397b0b1605",
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
              "id": "436c3f3d-13a2-410a-a3db-27d545144328"
            }
          ]
        },
        {
          "id": "c4f3378c-8993-4ac5-a49f-fb38232b8389",
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
              "id": "c7e9a216-1a9e-49d7-b9ac-d73c46564da5"
            }
          ]
        },
        {
          "id": "dd257b05-d2ff-4001-9b79-391fa737fa8d",
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
              "id": "ec6cf2d9-2672-4096-b518-cde0cea16c8f"
            }
          ]
        },
        {
          "id": "6460c357-8ec2-428d-a4c3-d617aad6cf3f",
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
              "id": "6a355f83-f3cd-4c32-922a-a83accd19978"
            }
          ]
        },
        {
          "id": "63a8b71d-c43d-4e7c-bec5-8de46b4a44b8",
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
              "id": "302465fd-b939-4823-8333-dccb45ae870e"
            }
          ]
        },
        {
          "id": "b532dee4-1eb2-4451-b678-c192e3abc73b",
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
              "id": "53e585c2-803f-45dc-9a02-09bc7bd8cd91"
            }
          ]
        },
        {
          "id": "5c8fd899-33c6-4266-ac3a-4e07e45ecbe7",
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
              "id": "e3910cc3-3763-41ef-bcf3-39695ed6a3af"
            }
          ]
        },
        {
          "id": "aea1e9e2-3236-4f80-893b-07d9b3f60110",
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
              "id": "b236cc17-710d-44a3-b5c9-3d0c230bd423"
            }
          ]
        },
        {
          "id": "a0e7a44d-0103-46a6-a13c-ca72d3a9e63a",
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
              "id": "8c566c79-70d9-460c-9f43-c9d955f1278c"
            }
          ]
        }
      ]
    },
    {
      "name": "Me",
      "item": [
        {
          "id": "14b24ea5-0f25-4cc9-9412-4d03e73d7e82",
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
              "id": "ad94288c-b83c-4f09-bf39-3552b4f6c25a"
            }
          ]
        },
        {
          "id": "5ca5dec2-8b70-4418-98f1-787bd2e75326",
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
              "id": "523cd40d-4fcf-4b99-89e9-c31ffa1e077c"
            }
          ]
        },
        {
          "id": "e355dd04-54ed-4aa1-929f-c8b91c4c60a7",
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
              "id": "7b998ddf-0ac1-4e00-a73a-4101e00056d7"
            }
          ]
        },
        {
          "id": "fa318ced-f521-45a2-8bcb-c7011523d1bb",
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
              "id": "44763a50-a1ac-47ab-addc-fc365da8463a"
            }
          ]
        },
        {
          "id": "54c2c617-e409-4559-831a-2f3583cbbb94",
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
              "id": "74dd8a89-7137-4124-ae11-e5f9ddb2b43e"
            }
          ]
        },
        {
          "id": "4072582b-ed8c-4fa1-a61d-3e3e1648ba66",
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
              "id": "c10de79b-b801-4aa6-81d5-ddb078245ead"
            }
          ]
        }
      ]
    },
    {
      "name": "Life",
      "item": [
        {
          "id": "a0acf1f5-889c-4c74-8b36-eb72ac13909b",
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
              "id": "0e8a25e8-81b6-49a6-a069-ee87cacb3a55"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "3ea2c290-ecc7-4a2c-8a91-2e456420afd9",
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
              "id": "549ced07-9d43-4db3-84f0-8d5f78b3bcc3"
            }
          ]
        },
        {
          "id": "e6f43279-71ca-4eff-a46f-9ef7c765d253",
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
              "id": "2685826b-4e8c-4a20-9ec1-0cc01161cf78"
            }
          ]
        }
      ]
    },
    {
      "name": "Live",
      "item": [
        {
          "id": "968b36b3-bd49-43f5-8d95-abcc818f9f9a",
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
              "id": "dd6a4203-46a2-4511-aa17-141333076167"
            }
          ]
        }
      ]
    },
    {
      "name": "Mailing",
      "item": [
        {
          "id": "3e7deb5c-cc3e-406e-88d0-31a3f43a47d1",
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
              "id": "c5f95b69-25b1-4eaa-b5df-3e7e9964f6ea"
            }
          ]
        }
      ]
    },
    {
      "name": "Message",
      "item": [
        {
          "id": "b62d0cec-ea64-4c52-9474-33662b77188c",
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
              "id": "979adbc7-176b-429c-9710-32d06c39cdd1"
            }
          ]
        },
        {
          "id": "9cdc8572-e33f-4fd8-b177-c88e590a9357",
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
              "id": "cf3b9a6c-2d90-4719-a6c8-0698b26ca46f"
            }
          ]
        },
        {
          "id": "d5bacfd5-e4fb-42da-9b6d-d1999221f56b",
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
              "id": "24c26589-8977-41bd-b2ea-c5c17f74c9e6"
            }
          ]
        }
      ]
    },
    {
      "name": "Milestone",
      "item": [
        {
          "id": "7dc895d9-0280-434f-9dbf-b331c7124b68",
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
              "id": "8518dd7d-7171-48a0-b72f-9f567b6fa1c4"
            }
          ]
        }
      ]
    },
    {
      "name": "Notification",
      "item": [
        {
          "id": "682c4310-55b2-4dba-a809-438670e29e3c",
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
              "id": "8b948526-8cae-441c-93f1-ea08abb2135d"
            }
          ]
        }
      ]
    },
    {
      "name": "Open",
      "item": [
        {
          "id": "8d9b2be0-d21c-4da0-a569-2bfc777a85a5",
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
              "id": "e6d65903-4602-4ea1-abb3-90f021cab872"
            }
          ]
        },
        {
          "id": "e20ae3a8-e4b3-4977-9dbb-cbc61470470e",
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
              "id": "f0260ef4-6bff-488c-8133-ebcd7da1c212"
            }
          ]
        },
        {
          "id": "84ecbc9e-f269-4889-9275-c1de5b4baab6",
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
              "id": "1fb7dcac-a4b9-497a-995a-8910d6db46ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Page",
      "item": [
        {
          "id": "ffb4b42c-16d7-4d62-8443-3c359a5f628c",
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
              "id": "cd4129ac-55ed-4608-9006-125789d2b21d"
            }
          ]
        },
        {
          "id": "f88f2423-5558-4253-b196-cc64f3a4c68a",
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
              "id": "8afe0c17-3734-4d82-aaa4-c301ffd59eb9"
            }
          ]
        },
        {
          "id": "1e6dda14-2e4b-439d-8245-f86d6a4db61b",
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
              "id": "a1889962-420a-4c2c-967d-d16aba411b54"
            }
          ]
        }
      ]
    },
    {
      "name": "Pages",
      "item": [
        {
          "id": "8488ff86-2067-4c8a-8908-c3e208509863",
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
              "id": "50bd8e61-2cf6-45ce-b36c-4a525f495073"
            }
          ]
        }
      ]
    },
    {
      "name": "Pa