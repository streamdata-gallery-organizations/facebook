{
  "info": {
    "name": "Facebook Get Me Home",
    "_postman_id": "b027ddf9-a26c-4269-8f37-1e8cdecbee53",
    "description": "As of October 6th, 2015, this endpoint is no longer available.  Please consider using the /user-id/feed edge instead.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Object",
      "item": [
        {
          "id": "5a4ecbeb-ab21-4a7d-ad59-e36cd711bc85",
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
              "id": "760e6da1-9356-4181-81f8-1ee0f9ed3a8e"
            }
          ]
        },
        {
          "id": "1aee3ca2-4d8f-4296-bfe5-23442483ca8c",
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
              "id": "cd8a4194-a5a0-4492-8c8f-9b08e6b273ee"
            }
          ]
        },
        {
          "id": "36101b73-e997-4d29-ad50-5472de2226eb",
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
              "id": "166df62d-a6f9-4172-b3ed-a6eb6564df45"
            }
          ]
        },
        {
          "id": "07523f10-c87b-475c-ad50-eca6297bc48f",
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
              "id": "20200961-cb82-4ec7-b6c2-3568a313fb28"
            }
          ]
        },
        {
          "id": "1e99da78-f0c5-41b1-9eb6-63185866d7d9",
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
              "id": "9ab7ab61-8c66-4cc7-98da-26855e2c51aa"
            }
          ]
        },
        {
          "id": "69babbac-9e3d-4672-9ce3-05117f1cdb6c",
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
              "id": "a56dda84-966d-403c-a11e-c58ccf780f1f"
            }
          ]
        },
        {
          "id": "03a55240-3c30-45cf-bd99-99f1987428f4",
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
              "id": "0ad32a2c-75a4-4b83-aff5-205882a58bbe"
            }
          ]
        }
      ]
    },
    {
      "name": "Achievement",
      "item": [
        {
          "id": "58b5648a-a2ee-47c3-9874-27664b4d6652",
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
              "id": "43f0d7d5-db8b-4aca-9c96-2a369af52ebc"
            }
          ]
        }
      ]
    },
    {
      "name": "Album",
      "item": [
        {
          "id": "36569440-2a66-4541-8a99-d0a7fbbd59d5",
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
              "id": "f3f1278e-d227-4f2f-80ab-72c711116d50"
            }
          ]
        },
        {
          "id": "a86a3f30-a409-4a6c-b5a8-edac98002488",
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
              "id": "d5d40a32-63ad-4deb-be47-f3cbf358052e"
            }
          ]
        },
        {
          "id": "b0d33e29-9ca2-479b-88b2-66099cb2c0f5",
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
              "id": "74ec2d11-baeb-4696-a93f-dc5fcb2949bf"
            }
          ]
        }
      ]
    },
    {
      "name": "Canvas",
      "item": [
        {
          "id": "f31cac0f-5f52-4bb5-a0d3-867c6f134de2",
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
              "id": "ea844a11-e255-48b4-8f7c-7acad464188d"
            }
          ]
        },
        {
          "id": "ea342e55-4fe6-4e2d-9c53-324297d155e3",
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
              "id": "c3355c73-af88-4824-add3-08a530a2dd1c"
            }
          ]
        },
        {
          "id": "334d4e85-4043-4048-8196-2f12d6fbc55e",
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
              "id": "d3079ea8-81ba-4e5e-b7f2-4313b9010b3a"
            }
          ]
        },
        {
          "id": "b1462ba0-6268-4d54-af8e-0e55eca58b6f",
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
              "id": "554ce455-ca0b-49f9-86e1-033edc6ed113"
            }
          ]
        },
        {
          "id": "936d6913-c46d-4e0f-96b3-c52ef8220c21",
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
              "id": "ef150fcd-1ac1-4d8d-808b-9abc98434762"
            }
          ]
        },
        {
          "id": "780e90bb-50f2-4912-b518-55c529059c79",
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
              "id": "0655dac5-3e7f-45b7-b96f-bb0e81d49fbe"
            }
          ]
        },
        {
          "id": "ff799091-a48a-4f55-bdd6-40c92b0096cd",
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
              "id": "03aeb70c-3d10-471d-9523-818c27ef3b69"
            }
          ]
        },
        {
          "id": "28367d01-3e60-4a1a-bc5a-3e60e01db925",
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
              "id": "ae304050-f5a2-412a-9d15-a2f38e56eee2"
            }
          ]
        },
        {
          "id": "ad73b2ea-3f29-4730-9ee8-3c555ccb1118",
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
              "id": "ece614b0-10b9-4048-8dba-d4bc9117468a"
            }
          ]
        },
        {
          "id": "1c591ba9-e93d-48ae-b568-0935c9ddbe18",
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
              "id": "537273c5-36dd-4bcf-9c2e-ef09b08b280e"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "077868fb-fb0e-4fc6-b011-4f66a4bc8436",
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
              "id": "b402a71e-d0b0-40e7-82b4-cf075d49525b"
            }
          ]
        },
        {
          "id": "da1cd1c7-8a62-44b2-a3ac-832955c9a0dc",
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
              "id": "0eaaba34-09ff-4372-84e5-a0054e2b2787"
            }
          ]
        }
      ]
    },
    {
      "name": "Analytics",
      "item": [
        {
          "id": "4896a5e5-f227-4406-8ca3-c85dbc31e8f9",
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
              "id": "945a90a7-4107-430e-a2bd-ab266cc5d9bf"
            }
          ]
        }
      ]
    },
    {
      "name": "Audience",
      "item": [
        {
          "id": "c52cbc85-f84c-44fb-84bf-51bb5db14d88",
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
              "id": "873eb87e-bf30-4226-b2f1-222da0796a7c"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "28d24e9b-1b16-4739-a201-69e71794d0aa",
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
              "id": "2cca394c-68a4-4eed-b606-8d033b7b10e0"
            }
          ]
        },
        {
          "id": "e9662d0b-b3da-4539-9abe-69fedebb80d8",
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
              "id": "9b19009b-d24b-4fbb-8746-46205e1ef776"
            }
          ]
        },
        {
          "id": "9daa9b4e-a6de-459d-9ef7-315783915cc7",
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
              "id": "2a4eeef2-a153-4548-9489-f245789b6cde"
            }
          ]
        }
      ]
    },
    {
      "name": "Conversation",
      "item": [
        {
          "id": "22c0bc2f-1c13-4892-805d-dc545785b7d5",
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
              "id": "7a3aa336-434a-4d0e-914e-b55158ca472e"
            }
          ]
        },
        {
          "id": "018fb92b-e832-4cc0-bbeb-82c7f246ff2d",
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
              "id": "f26cbe9b-8f64-4449-a8cf-5f6615148db9"
            }
          ]
        },
        {
          "id": "e0c6abcb-6d66-4bf2-8db2-e52c1a9b6fe0",
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
              "id": "105110a3-b08b-4667-8c74-9d1cead41825"
            }
          ]
        }
      ]
    },
    {
      "name": "Debug",
      "item": [
        {
          "id": "d76bb3ad-8368-4b7b-a80f-2694d06ab725",
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
              "id": "743b9c82-8d38-4f06-87da-2d4ef5a31e4c"
            }
          ]
        }
      ]
    },
    {
      "name": "Doc",
      "item": [
        {
          "id": "6daf4140-a69f-4fc6-8a8d-f724ee160be6",
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
              "id": "c1c2f113-6097-4863-a591-f039fcd0be35"
            }
          ]
        }
      ]
    },
    {
      "name": "Domain",
      "item": [
        {
          "id": "d85853f4-7a0f-438c-b60a-5c1e07237def",
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
              "id": "5259c9a6-89ab-4c52-b691-8f3cac7c342e"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "dd5ebb88-e6e9-4d69-bb5d-33ceb5114126",
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
              "id": "e85cdbb1-1085-4c31-83ba-7fcd12c38ab3"
            }
          ]
        }
      ]
    },
    {
      "name": "Friend",
      "item": [
        {
          "id": "62d65fcf-fd56-4c89-b0d7-cf348b366e89",
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
              "id": "dde696b6-16ed-4004-badf-27badf72ea09"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "14e9c308-2737-472c-97dd-78edbc45572c",
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
              "id": "8002ac0b-1c3c-4575-a8e9-38fdc3b72b85"
            }
          ]
        },
        {
          "id": "6d79a022-ca8d-4526-8d4b-c01a77c38b96",
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
              "id": "c7778bd3-5098-43d0-bb20-c52bab3eccc0"
            }
          ]
        },
        {
          "id": "9cc63282-fca9-47f4-9d0e-9efc1bcbf78e",
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
              "id": "ad4954f0-5603-455d-89a1-624dc365709d"
            }
          ]
        },
        {
          "id": "603c0dbd-9fef-498c-9393-8f07fba35c68",
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
              "id": "3330a421-86e0-4a24-995e-219b144c3bba"
            }
          ]
        },
        {
          "id": "00f1d668-29a8-497e-bab7-d03e993a38b8",
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
              "id": "bb680f4f-859a-4ea3-944b-130bd4f06cfa"
            }
          ]
        },
        {
          "id": "dbf258c5-65cc-4a44-96bd-b20b97d83698",
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
              "id": "a3af38f3-d75e-46a2-b91c-e55db16be693"
            }
          ]
        },
        {
          "id": "3e1c9211-778c-43b0-ac5d-0a798c4be6d8",
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
              "id": "ed06b0a8-b2ab-4dfc-872f-098ab28b5ca3"
            }
          ]
        },
        {
          "id": "28ef32a8-1699-4ff3-8292-265cfb858df5",
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
              "id": "8fc8bf4d-a506-4eae-8f5a-9e309138d56d"
            }
          ]
        },
        {
          "id": "31ee7aae-1e28-40fc-a092-3213d2e7dbc3",
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
              "id": "7d237de0-e5bd-4698-b661-84d7ee28db1c"
            }
          ]
        },
        {
          "id": "afad5d2c-f186-4554-8ff7-ecd6bfaff914",
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
              "id": "59099ef6-4194-4832-a301-bfc90f33ba82"
            }
          ]
        }
      ]
    },
    {
      "name": "Me",
      "item": [
        {
          "id": "789e5f48-ef28-479e-9af3-d6750c254dcc",
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
              "id": "0cf4b47b-d50a-481a-b223-02fd3dfabf3a"
            }
          ]
        },
        {
          "id": "fa01ef3e-dcbd-4c85-ac1b-d61a96c85aac",
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
              "id": "5d2659af-3946-4a9e-919f-c8fefc14f311"
            }
          ]
        },
        {
          "id": "d06f872e-9af9-444c-9a65-93eb06e471f3",
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
              "id": "60e0b89a-443a-4db9-af4e-c5c75a98eb06"
            }
          ]
        },
        {
          "id": "dd9af819-5986-4f79-ad87-289711e36f32",
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
              "id": "70ffd097-30f1-4f25-8667-d600d6207400"
            }
          ]
        },
        {
          "id": "e939a51e-f5f3-41f0-8996-47ce0293d6b5",
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
              "id": "265dc2bf-f3eb-4557-a7f0-a25afaa4ad7e"
            }
          ]
        }
      ]
    },
    {
      "name": "Life",
      "item": [
        {
          "id": "1dddd9b5-fee7-4f70-a3aa-566e73636a2d",
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
              "id": "d45955f5-0edd-464d-a8f0-d36aa675d681"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "e95efb7a-f1e1-4bb8-98e6-adde4025573d",
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
              "id": "0df0d5d8-220f-4a9d-852b-21fe805d1c40"
            }
          ]
        },
        {
          "id": "38b0d747-0a7b-4674-bee5-8bca5afc06a4",
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
              "id": "75986e94-d68d-4528-85e8-3970709d0140"
            }
          ]
        }
      ]
    },
    {
      "name": "Live",
      "item": [
        {
          "id": "89165a8e-ed94-40c1-b53e-3b4f8a0360de",
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
              "id": "2d3e1eea-ec8b-49be-8b91-7c8c379718ae"
            }
          ]
        }
      ]
    },
    {
      "name": "Mailing",
      "item": [
        {
          "id": "fd63338b-8e84-4cf3-8f8e-5442eb7c50c4",
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
              "id": "f34ddf5a-67e1-4eff-9749-acc8bda37348"
            }
          ]
        }
      ]
    },
    {
      "name": "Message",
      "item": [
        {
          "id": "bf48cfd3-61d1-4ff5-a9b1-c7d64320d9c1",
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
              "id": "f4d73bc2-4987-422c-a3e1-b5f6011cad44"
            }
          ]
        },
        {
          "id": "9dfa3109-9954-4830-9f06-7c0f2241e541",
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
              "id": "85cf454f-40bd-417a-a0fa-1b6430dc3584"
            }
          ]
        },
        {
          "id": "e50f070f-6335-457a-ba84-01a674223a74",
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
              "id": "6fc5e641-8dc0-4d92-95ef-dc3afb9dee98"
            }
          ]
        }
      ]
    },
    {
      "name": "Milestone",
      "item": [
        {
          "id": "02bc12f9-df3e-4a1a-9114-111961f74dae",
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
              "id": "de53a64b-1bbd-4e8e-a9b6-f1c3859f1379"
            }
          ]
        }
      ]
    },
    {
      "name": "Notification",
      "item": [
        {
          "id": "bbd4b82f-887e-43ca-9f50-25f8d28c2a94",
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
              "id": "f0ffe41a-7e9a-41e4-bf80-d357e24302bd"
            }
          ]
        }
      ]
    },
    {
      "name": "Open",
      "item": [
        {
          "id": "7e8140a6-7dc4-4456-97e9-091021168d30",
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
              "id": "213e9539-58bf-4315-bfb5-0a2084a50aab"
            }
          ]
        },
        {
          "id": "3250c188-4beb-4c46-a361-a0b9960b17d2",
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
              "id": "d6c9ad09-77b3-4db3-bcfa-ded041b39355"
            }
          ]
        },
        {
          "id": "596c9259-b8b0-4af2-950a-a0ecaaa07499",
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
              "id": "de0a8099-ce92-465a-9b89-3417f42f3537"
            }
          ]
        }
      ]
    },
    {
      "name": "Page",
      "item": [
        {
          "id": "e2e4b70d-6f13-43f1-85dd-da46c2b57d24",
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
              "id": "a5bb742f-2e43-4852-947e-db7fabe4e0e5"
            }
          ]
        },
        {
          "id": "00e6c3ed-9622-4a41-9120-6c1d2c92e166",
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
              "id": "c3ed26ec-aa0c-4de4-86d4-4f390e39034d"
            }
          ]
        },
        {
          "id": "3990d65e-5fe4-401e-9219-2ac4881ef895",
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
              "id": "98d2d5d4-8478-425a-9b52-21c3f19b7491"
            }
          ]
        }
      ]
    },
    {
      "name": "Pages",
      "item": [
        {
          "id": "5822d7bb-5c37-4a9a-b91d-121b0319b85a",
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
              "id": "70ef01d4-b0ab-4cb6-9d2b-76622e931cb0"
            }
          ]
        }
      ]
    },
    {
      "name": "Payment",
      "item": [
        {
          "id": "4482b6f4-0bf6-4a71-9ec1-07cb35d9593c",
          "name": "getPayment",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;payment-id&#125;?actions=actions&amount=amount&application=application&country=country&created_time=created_time&currency=currency&disputes=disputes&id=id&items=items&payout_foreign_exchange_rate=payout_foreign_exchange_rate&product=product&quantity=quantity&reason=reason&request_id=request_id&status=status&tax=