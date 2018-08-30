{
  "info": {
    "name": "Facebook Get Me Locations",
    "_postman_id": "47bd0aaa-94b9-40dd-9cd5-d5d1d92514bc",
    "description": "A feed of posts and photos that include location information and in which this person has been tagged. This is useful for constructing a chronology of places that the person has visited.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Object",
      "item": [
        {
          "id": "7306341e-6bb4-4e50-b5ff-34256133cd55",
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
              "id": "b60deaba-b979-4867-91dd-679accd6a7bd"
            }
          ]
        },
        {
          "id": "073ce9b2-394c-41a3-931d-8367d6a174fe",
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
              "id": "f96af056-b1ba-49f1-a523-eb68e550f873"
            }
          ]
        },
        {
          "id": "cb1e5b6f-ab62-4298-9b63-ef0ad2b3aba0",
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
              "id": "7967c0d9-4d0b-451f-9c0f-742c963a468a"
            }
          ]
        },
        {
          "id": "09b9a708-4b80-465b-8bee-c240f34b4859",
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
              "id": "d434210a-43e8-46ff-81e1-78d28eca6d1d"
            }
          ]
        },
        {
          "id": "a1a0e946-e830-464c-a826-0d251a189544",
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
              "id": "c113e3f2-e9b1-4a3d-923e-f5f1d25e5b8a"
            }
          ]
        },
        {
          "id": "68cdda1e-3028-4277-963c-d7e96db8122d",
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
              "id": "d74a27d1-2f36-42d3-a75b-00590c8ce1e8"
            }
          ]
        },
        {
          "id": "6857c521-587b-4bf1-a24a-a6ed12606b3a",
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
              "id": "c164d636-ed5a-44bb-af6f-7e8db296408d"
            }
          ]
        }
      ]
    },
    {
      "name": "Achievement",
      "item": [
        {
          "id": "a3873deb-108d-4c3d-8e9f-ead3e71506e4",
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
              "id": "caaa1e46-0cf9-4e9c-93af-1f02e8d7fbc7"
            }
          ]
        }
      ]
    },
    {
      "name": "Album",
      "item": [
        {
          "id": "f9786740-e648-4b55-bab0-e05fc2f6c020",
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
              "id": "a410cad9-34a4-4b67-a07b-33d7bece1abe"
            }
          ]
        },
        {
          "id": "00b57557-a5ae-401a-a521-56dbd2f298e3",
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
              "id": "4aa0da53-eb64-4d0e-af99-ad6f205b071a"
            }
          ]
        },
        {
          "id": "aa37da3c-f911-4768-8d99-fb5b51113d8f",
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
              "id": "7051087d-3fd1-42cf-9a3f-7f93f03e9a69"
            }
          ]
        }
      ]
    },
    {
      "name": "Canvas",
      "item": [
        {
          "id": "56ea6f50-7ec6-4bac-a56d-4b725b87164e",
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
              "id": "be021c93-1739-43f3-a1f7-37bdb67dc7f7"
            }
          ]
        },
        {
          "id": "6485fe1b-6b60-4747-a436-672faeddf35b",
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
              "id": "dde4b871-2166-446f-a9f2-ab3636dcf447"
            }
          ]
        },
        {
          "id": "7fa1bc09-c975-45d9-b3a8-e2f19f51fe0f",
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
              "id": "f2dc7e3e-43b1-4664-a90a-3bfc29b7eefd"
            }
          ]
        },
        {
          "id": "1948d86d-18d5-4bdd-9af1-f5a6f98cc356",
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
              "id": "bf24e582-20f6-49f2-b5a7-8129c5b26454"
            }
          ]
        },
        {
          "id": "22fd028d-7d2d-4b6b-a988-c017298f2ff8",
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
              "id": "2e5b267b-14ea-484c-b156-11bc09e0ab05"
            }
          ]
        },
        {
          "id": "29205d38-fb7e-42ef-af66-2eca05b2ce75",
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
              "id": "aec3e57b-d898-4290-a95e-9a762fba7a93"
            }
          ]
        },
        {
          "id": "b12b4992-83db-4b63-b344-e38ab3bbfda2",
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
              "id": "71aff185-521a-43c7-be67-adae4909fa01"
            }
          ]
        },
        {
          "id": "897b4ec4-be93-480a-8e30-7595f03456d1",
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
              "id": "b6343e4d-0077-4a7d-9548-c8dc6b586e87"
            }
          ]
        },
        {
          "id": "298e39e4-b3c1-48e9-a01a-7539d3a32350",
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
              "id": "43018b1c-a341-4679-86a3-5584281bd37e"
            }
          ]
        },
        {
          "id": "8620c7a5-9429-452c-831d-f91ba9253af7",
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
              "id": "d716ebe3-67ec-4f7e-86eb-5d5d5d0b709a"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "a736b930-1e8e-4c41-b0e6-e223734382a1",
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
              "id": "e501265a-958f-4898-8915-9fe9e281f10a"
            }
          ]
        },
        {
          "id": "ff6ee445-db6b-4ced-a30e-ce147fc96c3f",
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
              "id": "08941da7-dcae-4498-8e71-2d82fc94feee"
            }
          ]
        }
      ]
    },
    {
      "name": "Analytics",
      "item": [
        {
          "id": "07685c7b-c105-4fc6-8a20-140bf437df6d",
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
              "id": "ad32cdd0-24f7-4050-a86c-126af7f77e25"
            }
          ]
        }
      ]
    },
    {
      "name": "Audience",
      "item": [
        {
          "id": "75eafed1-7f9b-4001-a342-e4c37bff353f",
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
              "id": "27476533-c047-48b2-a500-dedd6d8294c1"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "e2603c02-0338-4eaf-a5bd-9c137926dcaf",
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
              "id": "7420fa08-7340-40d1-88fe-2063b0658981"
            }
          ]
        },
        {
          "id": "1b3505bc-2139-4897-8421-b44479a35fff",
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
              "id": "83d35a6e-f5be-4b62-83c7-233728c4b608"
            }
          ]
        },
        {
          "id": "dee03bd9-91a6-4b2d-a149-1280a9aaf78e",
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
              "id": "11400952-1d93-4133-9e9b-66787ef5b662"
            }
          ]
        }
      ]
    },
    {
      "name": "Conversation",
      "item": [
        {
          "id": "0166e126-a20b-4250-8ba7-a823992dd333",
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
              "id": "be88fab1-653b-4503-961d-f02167b46944"
            }
          ]
        },
        {
          "id": "0ead629d-9ecb-42f0-9064-b5f484c06475",
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
              "id": "447ca199-ff2a-430e-bcd5-9e09184140e8"
            }
          ]
        },
        {
          "id": "c2948cb9-193b-425d-bd6f-f6e293e26926",
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
              "id": "2e8522b2-d486-40e3-9af3-a032762b4b70"
            }
          ]
        }
      ]
    },
    {
      "name": "Debug",
      "item": [
        {
          "id": "07ea839f-69ea-43c2-a954-c254a930aebc",
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
              "id": "8e274942-4a1d-4866-8bc3-c6ac52f54b51"
            }
          ]
        }
      ]
    },
    {
      "name": "Doc",
      "item": [
        {
          "id": "7397d576-a6b5-4001-9a0f-4d7339474d7d",
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
              "id": "8a52bc82-3265-4129-9fc9-a6ea8e399206"
            }
          ]
        }
      ]
    },
    {
      "name": "Domain",
      "item": [
        {
          "id": "688f4176-3bea-4df6-9b54-da9b503e7a70",
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
              "id": "f89c94c8-3955-43eb-81b9-8a9db2d0d6a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "8f44bc8c-08c4-4688-b97e-c31be55d1840",
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
              "id": "9938d107-2fac-44ca-99bc-ecedf845c52c"
            }
          ]
        }
      ]
    },
    {
      "name": "Friend",
      "item": [
        {
          "id": "dc36e765-ed3c-48dc-9816-f80249c8bdad",
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
              "id": "5f1f7d2b-be3a-4bf0-91a1-a64d5aa2a749"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "27e94c99-02f1-4840-a726-a55a68df22f6",
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
              "id": "9755b739-c98d-4e5c-9e4e-8118a89ab2be"
            }
          ]
        },
        {
          "id": "eecc23da-cdfa-49b7-81d7-18d43211f606",
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
              "id": "71bcdba5-3a27-4229-af83-591963715ba1"
            }
          ]
        },
        {
          "id": "9e0fbc6f-b9ef-4e5d-9f77-4738aa80f65b",
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
              "id": "23675df6-9ef1-4c40-948f-d21766412394"
            }
          ]
        },
        {
          "id": "9dce1c85-89bf-4d09-b6c5-ba1eaf13bc46",
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
              "id": "274c6ba5-1d7d-418f-9f57-cf4ac967eeb9"
            }
          ]
        },
        {
          "id": "9065a41e-1af7-4bfa-94a4-9232f48b96b4",
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
              "id": "0cd25243-7f0b-4417-a712-3bd462a0cdfa"
            }
          ]
        },
        {
          "id": "e8cb0b7e-f1ab-4769-bc53-24fe27ed97b8",
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
              "id": "bb5bf194-1770-4942-84d4-60d5f957b318"
            }
          ]
        },
        {
          "id": "af8c0aec-93cc-42a7-98ea-f4beba4a4bb6",
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
              "id": "d9e75a3c-5bf3-4847-9c00-99d79e75be52"
            }
          ]
        },
        {
          "id": "80c3384d-5368-4e2a-93d1-77bbb8a00465",
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
              "id": "e605281c-4f6a-4d7b-bcb7-fb5861033e7b"
            }
          ]
        },
        {
          "id": "7fd52ba1-83d1-4cc4-84b8-86cf3fb2a853",
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
              "id": "3e246d7a-a322-4c5b-906b-640b6f85b6ae"
            }
          ]
        },
        {
          "id": "f55dc5b4-4548-4035-805b-4845a52f9347",
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
              "id": "55c97d94-768d-414f-82be-bcb9dd2e77a2"
            }
          ]
        }
      ]
    },
    {
      "name": "Me",
      "item": [
        {
          "id": "994a10a1-576e-4781-bdcd-71f4012a3b62",
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
              "id": "77f475f8-94cd-44a6-9805-2153af345f71"
            }
          ]
        },
        {
          "id": "eb788cca-3881-4dbb-9799-663104dbc61f",
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
              "id": "462fad75-6654-4a13-8c7f-0e9721cc8779"
            }
          ]
        },
        {
          "id": "ed3d4c02-ab66-43e9-b313-0ec6c6278ab3",
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
              "id": "eb440267-d92e-4116-b5b9-a51ab4459523"
            }
          ]
        },
        {
          "id": "5339c7bd-2549-4e75-a7d9-c6976c7d46c4",
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
              "id": "2609ef6e-79c3-472f-b89e-fda2499155bd"
            }
          ]
        },
        {
          "id": "fa2ff474-9ffa-46e7-9a60-00a925fcc37f",
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
              "id": "390fef45-cacb-4490-be9c-1987a3cb8d5d"
            }
          ]
        },
        {
          "id": "0142018f-e5ef-4112-baba-56dea155904b",
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
              "id": "cec950cd-80d7-4161-b2b1-bc689dfec4c9"
            }
          ]
        },
        {
          "id": "bcf6a09d-5eb9-4c88-8fd9-5c0cd041c3b4",
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
              "id": "e736ff81-028c-4154-a5a1-5eee81c035ff"
            }
          ]
        }
      ]
    },
    {
      "name": "Life",
      "item": [
        {
          "id": "e401d5c8-b3fd-4c22-98e0-d79276afaa35",
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
              "id": "f5e3f1e3-ae41-4204-a95e-b05b19221117"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "766b6763-ed44-403b-9917-15d898e7552f",
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
              "id": "e1462267-a9f9-4031-8dd4-d767de65c873"
            }
          ]
        },
        {
          "id": "ca650d0c-7d21-487d-b118-0ba22694d122",
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
              "id": "18cf5359-bba8-47dd-9506-9f290ec062b9"
            }
          ]
        }
      ]
    },
    {
      "name": "Live",
      "item": [
        {
          "id": "3b0f5fad-aac4-43e1-848c-ebd9ade0f4b3",
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
              "id": "887eb962-5288-45ab-89fd-68fc062c44c7"
            }
          ]
        }
      ]
    },
    {
      "name": "Mailing",
      "item": [
        {
          "id": "0d814241-7ade-4246-82b8-6137e0c36d13",
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
              "id": "500f0e2a-2b78-48b4-8daa-9ea09c6296e9"
            }
          ]
        }
      ]
    },
    {
      "name": "Message",
      "item": [
        {
          "id": "37859fd0-09d1-4a05-a7ec-37dca85fbd1e",
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
              "id": "0652c097-4872-4049-8965-b9b0bb72438c"
            }
          ]
        },
        {
          "id": "04065abd-b272-42b4-a4bc-d3d2edaa9c71",
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
              "id": "9e7cfbb7-00d6-4335-b768-e84cb6f1a8d3"
            }
          ]
        },
        {
          "id": "5f168ad6-40df-45e3-aa9b-65b2ca4b1ccf",
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
              "id": "d0daaeba-8582-4017-9a9f-170a45928f04"
            }
          ]
        }
      ]
    },
    {
      "name": "Milestone",
      "item": [
        {
          "id": "1bf43f74-835b-4e27-b109-2de2620422df",
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
              "id": "e2cce836-82ac-40b7-a1eb-5365d9df43c2"
            }
          ]
        }
      ]
    },
    {
      "name": "Notification",
      "item": [
        {
          "id": "c3bfd3b8-c0fc-48f6-a1e9-398b52a1af1e",
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
              "id": "47f88319-97f5-4a46-bef0-5f80cb148d2b"
            }
          ]
        }
      ]
    },
    {
      "name": "Open",
      "item": [
        {
          "id": "ff707af1-6103-44fa-adb1-f2189ab6c45a",
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
              "id": "8d10cfa7-fef5-48ab-aab2-71f3673f725f"
            }
          ]
        },
        {
          "id": "01cf842c-0f0c-4541-af21-3f4431e52f64",
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
              "id": "56900233-46d5-4475-9f2a-d05351596e17"
            }
          ]
        },
        {
          "id": "47cef14e-47f6-4e4c-8ae1-11f011d7eb5e",
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
              "id": "3c712887-9fe2-4a37-b8b9-ba5c29d347b7"
            }
          ]
        }
      ]
    },
    {
      "name": "Page",
      "item": [
        {
          "id": "accca20d-36d4-40f5-889d-bd85ec95f74c",
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
              "id": "7360572d-706b-41f3-a877-213fd6c933a0"
            }
          ]
        },
        {
          "id": "1d65a005-3c1c-4daa-b1dc-e8aaa95ea1d3",
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
              "id": "09783806-4d34-4c71-836d-ed72dab1f92b"
            }
          ]
        },
        {
          "id": "7775085e-64ba-4190-9865-c9836ad5a785",
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
              "id": "8eefac43-7ece-44ff-ae7d-5cac98799341"
            }
          ]
   