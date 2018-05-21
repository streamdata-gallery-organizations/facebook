{
  "info": {
    "name": "Facebook Post Me Scores",
    "_postman_id": "86fea478-b080-4bcc-b311-932541846e83",
    "description": "As of April 4, 2018, this endpoint only returns an empty data set. Please see the changelog for more information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Object",
      "item": [
        {
          "id": "595315d0-124f-4e8a-a554-e3d32a3db4e2",
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
              "id": "604aded4-cd7c-4d0d-a5eb-e68e24dee19e"
            }
          ]
        },
        {
          "id": "18f9e49c-3cc1-4980-b6ba-a9c0fbb6f109",
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
              "id": "10a461ae-e0be-44a1-8c4d-a2d81e11d9c9"
            }
          ]
        },
        {
          "id": "ba83b59a-34a1-4e0f-b90a-70ac23b5a892",
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
              "id": "dd04be2a-9946-4b6e-9cc2-57123333da79"
            }
          ]
        },
        {
          "id": "1063d2a5-1fb9-4854-bc87-c0ea86355a31",
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
              "id": "02d44b04-e0f9-496e-a359-d7faa3641e41"
            }
          ]
        },
        {
          "id": "770d06ca-9fc9-454f-8408-a23e6617d49e",
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
              "id": "afcc35bc-b069-40c0-a9d1-52bfc5742b27"
            }
          ]
        },
        {
          "id": "7e3fb700-5c93-4d87-a6ba-d130198789dc",
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
              "id": "84fdff47-c9cd-4312-9671-bd8866f98872"
            }
          ]
        },
        {
          "id": "66758f30-3f16-413a-b7da-ff69f7e27eed",
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
              "id": "e4fe0ca0-9317-47e8-a130-80844835b6e8"
            }
          ]
        }
      ]
    },
    {
      "name": "Achievement",
      "item": [
        {
          "id": "78df52ba-3add-4fef-a60f-c2101eb8b0e2",
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
              "id": "b361de8d-2b19-48e6-bf8c-0491d977571c"
            }
          ]
        }
      ]
    },
    {
      "name": "Album",
      "item": [
        {
          "id": "cbf49e72-e0c5-4099-9dcb-fa2f6e361d59",
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
              "id": "2cecbfab-879b-40f6-9aec-c79f44548d01"
            }
          ]
        },
        {
          "id": "39272398-bc5f-4890-9e6c-c848b0edd7e5",
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
              "id": "69fa0a32-e700-4cdb-9733-e52703237e98"
            }
          ]
        },
        {
          "id": "cfb58cba-4114-431d-9356-84ffbb6f05ad",
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
              "id": "02b92127-aa47-4269-8c89-11069d5ecc71"
            }
          ]
        }
      ]
    },
    {
      "name": "Canvas",
      "item": [
        {
          "id": "c6fae5c7-6366-492c-a001-a2999481382a",
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
              "id": "6ab2f7e4-2a35-470f-9736-b0ba886ad794"
            }
          ]
        },
        {
          "id": "c1b9dbed-2135-4fd2-b1c6-55a6479ee045",
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
              "id": "87b0dedd-ed6d-49d8-8dcb-42bff5a24bc6"
            }
          ]
        },
        {
          "id": "15dba138-532f-47ba-a707-ec113432b073",
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
              "id": "1296bd24-c68f-42ae-9949-aef36c57dac5"
            }
          ]
        },
        {
          "id": "b03f6023-1ef0-4ef4-9355-703254997a7c",
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
              "id": "a5e6fe2c-1ba2-4640-8700-9349f94f8fa9"
            }
          ]
        },
        {
          "id": "b8317739-9dfd-4f09-9655-18817c693444",
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
              "id": "540b5e1a-7e52-47e4-8336-db6a61f54739"
            }
          ]
        },
        {
          "id": "13955838-dc6e-4e0c-8f68-b0fb07860b7f",
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
              "id": "f2cace8d-b37c-4e44-b06e-911fb70f3801"
            }
          ]
        },
        {
          "id": "075d510c-7c00-4bd8-99d6-d3c39360eec5",
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
              "id": "c71f0e09-8682-4c5e-8325-a1f46fe74d9d"
            }
          ]
        },
        {
          "id": "cbd15ddc-356f-4922-9944-a083ebcd34ce",
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
              "id": "8b0db374-fccd-47e0-8f9c-a6e464a1a891"
            }
          ]
        },
        {
          "id": "59e5e32d-7d19-44ad-b351-394897353746",
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
              "id": "b381bb36-ff79-4929-a451-314e549fa9f8"
            }
          ]
        },
        {
          "id": "bb0bed31-8a19-4140-a428-cfa8a155535e",
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
              "id": "78eadbf7-2d31-4c0e-9533-fd21245d4a79"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "f51a240f-4e41-478e-978f-9eb94a2ec4ef",
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
              "id": "72310779-660e-4c58-a2dc-4a115d23d520"
            }
          ]
        },
        {
          "id": "1baa97fe-a2cf-4274-8a0f-552bf4c5e61e",
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
              "id": "68d12a2e-3fc4-412e-acc1-84c2a9028e18"
            }
          ]
        }
      ]
    },
    {
      "name": "Analytics",
      "item": [
        {
          "id": "cb28661b-f29c-4ec1-a8f6-4a43669de897",
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
              "id": "86f787cb-66d8-4184-ab6a-6b0bbea73ded"
            }
          ]
        }
      ]
    },
    {
      "name": "Audience",
      "item": [
        {
          "id": "a0f2d9e1-4d17-4970-91ef-e82d48377d85",
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
              "id": "541051cb-15ff-422e-b91a-5d9c56d8ce5e"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "6d36ff84-dd46-40d9-95b8-9549582f2f93",
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
              "id": "0570bfaa-3958-4d8a-8720-20b7fec6c92e"
            }
          ]
        },
        {
          "id": "887ede51-51ce-4d46-87e0-c3ffe6c35c5a",
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
              "id": "864b1ae6-c61a-4a7e-a01c-1fba2ae04879"
            }
          ]
        },
        {
          "id": "314595d2-4997-4b47-8f7e-462263a4d394",
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
              "id": "e3a745bb-e2a3-4d66-a84e-42e69d520f01"
            }
          ]
        }
      ]
    },
    {
      "name": "Conversation",
      "item": [
        {
          "id": "dbf344c7-fa7d-4bfc-b434-fbed8e57e26f",
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
              "id": "14b41b60-2e60-4bf5-b095-c073d74bb5fb"
            }
          ]
        },
        {
          "id": "f74daae4-8b62-413f-af23-8cd2509a14bb",
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
              "id": "07e7789d-689b-4343-aef5-341749b72e9b"
            }
          ]
        },
        {
          "id": "a7f1e5c5-b8dc-409c-b586-46cc66cd3452",
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
              "id": "f9c5c6a5-498b-4cd4-913c-e52a6b45701c"
            }
          ]
        }
      ]
    },
    {
      "name": "Debug",
      "item": [
        {
          "id": "25727758-610e-40de-845c-030487850100",
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
              "id": "318ab12f-8c9f-4ef7-9192-4ca48a72bca2"
            }
          ]
        }
      ]
    },
    {
      "name": "Doc",
      "item": [
        {
          "id": "f1126cd6-1c68-40f2-a2e3-823fc7e373eb",
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
              "id": "fc82c7d1-fa3e-4ada-a626-8d5e81dbf1b4"
            }
          ]
        }
      ]
    },
    {
      "name": "Domain",
      "item": [
        {
          "id": "38f7813d-9df5-4cd5-81c9-37a5f59967f0",
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
              "id": "64b0f2a0-2f68-4172-a3b3-b4c833d4422b"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "2bc3e052-205f-420e-bf07-b8f361fc7c2d",
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
              "id": "1522f911-d4ca-49e4-821f-68244c333647"
            }
          ]
        }
      ]
    },
    {
      "name": "Friend",
      "item": [
        {
          "id": "c25f9fb0-9517-457a-9808-1ec59761d471",
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
              "id": "b64a266f-f6f2-4738-b698-11fce2ef96da"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "25faa6c9-9eae-4803-b9f2-b60526558276",
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
              "id": "5d4bca25-1d2d-46b8-9ecd-5d925d16230b"
            }
          ]
        },
        {
          "id": "60161bf0-fd46-425e-b126-ae5087bbd7dc",
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
              "id": "b66159e8-19de-4fcb-b44b-10befe79cecb"
            }
          ]
        },
        {
          "id": "06117e9e-82b2-4f65-9767-0d31907ee06d",
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
              "id": "f1257c95-e8a5-43a8-ba51-34d9a9bdd565"
            }
          ]
        },
        {
          "id": "fcc2f19a-c1c7-482b-90bd-6f2b0fec2e69",
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
              "id": "8a94df30-9a83-41f6-ab83-49171c7d1320"
            }
          ]
        },
        {
          "id": "dfc2721e-b9ed-4be9-ad01-60c0ca9b45cb",
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
              "id": "5db597d2-a312-41ea-86b7-e8b8ae173a7e"
            }
          ]
        },
        {
          "id": "d4f2324c-e7d9-41e6-82ab-d85867ae0e7b",
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
              "id": "55897923-7654-47d2-9a94-a1b229b26652"
            }
          ]
        },
        {
          "id": "bf34ce6d-7f4f-4465-802c-b5da0cd1fcf7",
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
              "id": "37e7c641-d39f-4641-8748-8556d2e35095"
            }
          ]
        },
        {
          "id": "78ccbf42-1509-4365-96c1-8fa69a4fb21a",
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
              "id": "8eebb734-5c4b-4b97-a250-209bf0d2b854"
            }
          ]
        },
        {
          "id": "629a7b49-0b19-4d4f-844a-7d56fb7700c5",
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
              "id": "4dd24c60-8e76-4173-a6b5-f4373e24ae3f"
            }
          ]
        },
        {
          "id": "786cbbce-a340-4e5e-9c19-8c7df0cccebf",
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
              "id": "962840fd-7b71-42c1-ad51-98c633c9051e"
            }
          ]
        }
      ]
    },
    {
      "name": "Me",
      "item": [
        {
          "id": "0807e65b-0a99-49e1-a6ff-7e962e4f7d5d",
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
              "id": "ca542610-6e28-44af-89bd-91cca1df2e33"
            }
          ]
        },
        {
          "id": "78415fe6-50cd-46ee-bb4e-336fe3cdf3ea",
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
              "id": "1a78196f-2306-46d8-b6b2-055bd63c9426"
            }
          ]
        },
        {
          "id": "ad30ccc9-ea77-4bc5-ad1a-7983d1f46ee5",
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
              "id": "83bd4424-b945-427d-adea-2bc9e1ba94bf"
            }
          ]
        },
        {
          "id": "5e4e028e-b75c-4496-9558-7dbcf172de57",
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
              "id": "a9440f58-fc43-4efe-8c7a-09cdec015ad1"
            }
          ]
        },
        {
          "id": "55a1b687-5258-4c41-92cc-e84ee116bd1c",
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
              "id": "95ff5cb8-d6f7-4372-a168-ff35becbe12a"
            }
          ]
        },
        {
          "id": "87e2d697-46e1-4d3c-b7ff-37db3f5d9dae",
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
              "id": "d3a34984-3dd0-460a-b563-b48baa42c801"
            }
          ]
        },
        {
          "id": "3c678b86-2c52-4f7d-b5cd-600703862b71",
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
              "id": "dd6d5a79-c1c3-4571-b907-7d86388d9d60"
            }
          ]
        },
        {
          "id": "f25a3b9c-625f-4ac8-ab8b-9408f7e4b110",
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
              "id": "2d8a934b-772e-4718-bdbc-b800e5911da5"
            }
          ]
        },
        {
          "id": "f18e6a69-e351-4b7e-a3fa-6b77b53a6eeb",
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
              "id": "ab6c1948-af37-4e43-a182-2ac52ab4e15f"
            }
          ]
        },
        {
          "id": "efa49be4-23ff-416a-b06c-6316f11ffd66",
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
              "id": "3c30b1f1-cf18-4fe4-8a49-04a3ea19b25e"
            }
          ]
        }
      ]
    },
    {
      "name": "Life",
      "item": [
        {
          "id": "e99bb224-235f-4480-8b3c-5c4bc5cd6b77",
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
              "id": "88caca23-0d34-490d-82be-b6ced9cd6d35"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "d379866b-b2dd-4e96-9844-9e5f8ca43aa5",
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
              "id": "4fb849f8-8b9c-4d12-aff8-7c23158d9b14"
            }
          ]
        },
        {
          "id": "11f81e98-b13a-45a2-8628-35bd317fc227",
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
              "id": "6bf86fa8-d7d8-407c-9f65-05e6782a08f7"
            }
          ]
        }
      ]
    },
    {
      "name": "Live",
      "item": [
        {
          "id": "a397b23d-7be5-4065-965b-8434b38c2161",
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
              "id": "94189e65-46c6-45c3-b316-1b4f6e1d4c40"
            }
          ]
        }
      ]
    },
    {
      "name": "Mailing",
      "item": [
        {
          "id": "5cd7ca64-9c64-48d4-8042-7cfbe8205f31",
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
              "id": "bbd29fc0-080f-4ef0-bdc6-bb12b5e3190e"
            }
          ]
        }
      ]
    },
    {
      "name": "Message",
      "item": [
        {
          "id": "c41a1558-2ed7-4124-83de-d625aa55f4d4",
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
              "id": "470b7e53-3741-49e7-ae98-252ec0dea7eb"
            }
          ]
        },
        {
          "id": "79fd2ce8-3786-448e-94ce-fe810cea507c",
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
              "id": "148346a4-142a-401f-823f-8deac89a5738"
            }
          ]
        },
        {
          "id": "7572ac4f-8c74-46b4-8b11-c88be904b064",
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
              "id": "a6a5848f-2a1e-43b3-a8b2-b490657a8ab3"
            }
          ]
        }
      ]
    },
    {
      "name": "Milestone",
      "item": [
        {
          "id": "370a5d1f-1ee3-4963-b0ed-2c990cf5002e",
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
              "id": "dae6049e-aaf0-4e86-8a9d-2c5ff44fe4fb"
            }
          ]
        }
      ]
    },
    {
      "name": "Notification",
      "item": [
        {
          "id": "4cb1f9eb-1717-409d-a64b-94cd40a59fb4",
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
              "id": "edd4192b-605c-4a9f-86fe-7ed0fb09b7c4"
            }
          ]
        }
      ]
    },
    {
      "name": "Open",
      "item": [
        {
          "id": "500a145e-024a-4549-94ae-de3b4cae59cf",
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
              "id": "7973cf33-0258-4262-8579-532f0e58eb9e"
            }
          ]
        },
        {
          "id": "a88ccca9-1cc6-4e01-9d34-19382a23ab3e",
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
              "id": "5c678ec6-5115-4e78-ad6b-b43d451f9b3d"
            }
          ]
        },
        {
          "id": "00c14dc9-5076-42fc-ac8b-e61416d2756e",
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
              "id": "4add39f8-4488-40ce-8f13-c1ffff4d6fdc"
            }
          ]
        }
      ]
    },
    {
      "name": "Page",
      "item": [
        {
          "id": "f4c8b56c-1720-46b3-9d27-36dadf46a541",
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
              "id": "0fc5de72-36ff-44c3-8798-fdbc1608be99"
            }
          ]
        },
        {
          "id": "3e5d5100-bc27-4bca-95fc-a7e97651b751",
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
              "id": "3df8278c-fbc8-4ff3-a874-63f2f7286fb9"
            }
          ]
        },
        {
          "id": "7469fd30-b469-4a79-b32d-d258a70e9fc0",
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
              "id": "01330596-ad6c-4b42-925c-9982fbda83f3"
            }
          ]
        }
      ]
    },
    {
      "name": "Pages",
      "item": [
        {
          "id": "aada6e4d-bb6e-4734-86f1-1a53e85b42aa",
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
              "id": "8d52a2e4-1e2d-43ac-b43d-5bf6636dd544"
            }
          ]
        }
      ]
    },
    {
      "name": "Payment",
      "item": [
        {
          "id": "41fd6998-d9d6-491a-aef4-b09aad91ac35",
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
              "id": "ef7cf9ec-b2ed-443a-aef6-31f1a31beeb2"
            }
          ]
        },
        {
          "id": "54207659-ed96-4e0e-b52a-12fdce45ab5d",
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
              "id": "51076a40-d934-4c6a-bc4b-5fa7c5ad236a"
            }
          ]
        },
        {
          "id": "9c7e9360-34b6-4858-bcd7-283472505b7e",
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
              "id": "30c1cf1e-c4bb-4a07-a71c-150bccafa8cd"
            }
          ]
        }
      ]
    },
    {
      "name": "Place",
      "item": [
        {
          "id": "8be921ce-b2a3-4596-9ea5-8035687387f7",
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
              "id": "df8c0bc5-606a-49ba-9686-343c131c0576"
            }
          ]
        },
        {
          "id": "5facbd8a-eadc-42d1-ba90-35c3882d854c",
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
              "id": "097c3e72-e223-41e5-a432-8e40b643d759"
            }
          ]
        }
      ]
    },
    {
      "name": "Posts",
      "item": [
        {
          "id": "a0e64371-188a-49ad-8517-eaeea8834873",
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
              "id": "bd5e0982-86d0-4e65-996f-388c43b44080"
            }
          ]
        },
        {
          "id": "d16304e5-6f96-4af9-8d80-55e116e70927",
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
              "id": "b3c38270-1dc1-4bb2-a3f1-04688dbdaf04"
            }
          ]
        },
        {
          "id": "88d58d0e-1c1e-4850-bd41-4ee969744426",
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
              "id": "2b197534-533d-469f-8319-f3db05d056bb"
            }
          ]
        }
      ]
    },
    {
      "name": "Attachments",
      "item": [
        {
          "id": "8703b5b1-caab-44b8-afdc-a57afae8626c",
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
              "id": "aee80870-1fb2-4790-b1fb-cf5bfd61fef7"
            }
          ]
        }
      ]
    },
    {
      "name": "Promotion",
      "item": [
        {
          "id": "d67fd3b9-a819-4d69-afdc-42927c11370b",
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
              "id": "67d16448-32c0-4c54-8d88-fd9a10751ecf"
            }
          ]
        }
      ]
    },
    {
      "name": "Rtb",
      "item": [
        {
          "id": "fa519520-d6b8-4ed1-ac34-db1c3ead3c93",
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
              "id": "a8fc65fc-ae85-453e-8b4f-823bda939121"
            }
          ]
        }
      ]
    },
    {
      "name": "Request",
      "item": [
        {
          "id": "22afec78-0821-4629-a3b6-37df56d64d93",
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
              "id": "5a61000e-44f6-4a5b-b22b-5756604a4c25"
            }
          ]
        },
        {
          "id": "8e852df2-86ae-45de-9620-00b70826c2bb",
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
              "id": "ac477050-2438-4bdd-9239-26a36a3cf019"
            }
          ]
        }
      ]
    },
    {
      "name": "Sales",
      "item": [
        {
          "id": "fb8dc861-c17e-4ed2-abb6-10ee55799b2f",
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
              "id": "9d9830db-515a-480d-8c20-ee85f97aff98"
            }
          ]
        }
      ]
    },
    {
      "name": "Saved",
      "item": [
        {
          "id": "c538c9ae-cebe-4bf0-bedc-c0f66406c366",
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
              "id": "35f2e1ec-5496-4e5e-93c4-18f61ef0feeb"
            }
          ]
        }
      ]
    },
    {
      "name": "Status",
      "item": [
        {
          "id": "35767a1d-dcfb-4371-a9d2-80fde79e16d1",
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
              "id": "708e583b-9c7f-4fbe-8652-5d54a2837e3b"
            }
          ]
        }
      ]
    },
    {
      "name": "From.",
      "item": [
        {
          "id": "47c2a14f-cd27-4437-90dd-c6788a483214",
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
              "id": "0bf0e082-9eed-4920-9d2c-3739d9cb26a1"
            }
          ]
        },
        {
          "id": "51f9d229-c03f-4f80-a6bb-f765e17a45f9",
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
              "id": "be9bb211-c209-40bd-878d-5548a45196a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Test",
      "item": [
        {
          "id": "638d8390-d7fc-4d4c-b8cc-d4f5bc93ede3",
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
              "id": "7f8d0cf3-7325-4cb0-b831-aff501a5cf0b"
            }
          ]
        },
        {
          "id": "106f9ce6-e697-473f-8b72-473aac6015aa",
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
              "id": "efd96794-99c1-4e0c-98cd-3cfe8bead9b1"
            }
          ]
        },
        {
          "id": "2b899657-9ba1-46dc-b623-bbb4dab919d5",
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
              "id": "dfbb96db-4c3d-48fa-bd30-5cf2eca279fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Thread",
      "item": [
        {
          "id": "ce15e419-80c9-429d-9135-e3c88d0a9cae",
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
              "id": "1d09fdfb-2808-42ba-a206-b8966443f059"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "8365f701-5946-4ee3-b7c0-0edcde569cdb",
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
              "id": "83608828-54aa-4041-b4e8-e4a67d943b97"
            }
          ]
        },
        {
          "id": "b931354e-0498-4c1b-8caa-fd62a03baf7c",
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
              "id": "e5827721-ada5-4103-bdbd-8486e13ae5bb"
            }
          ]
        },
        {
          "id": "22774df1-a224-45f1-a0f3-d37a4a8403d1",
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
              "id": "e9f3b624-9733-4aa0-a93f-067a30cd90c5"
            }
          ]
        },
        {
          "id": "d792c8e4-6fbe-4485-a6eb-2fd6156f4ba4",
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
              "id": "144ab68f-b5c2-4986-95c6-c2c929970c9c"
            }
          ]
        },
        {
          "id": "2e0f81ef-5418-49fd-bd32-74640c37b997",
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
              "id": "a48dec72-6eb6-44d8-b385-607269e95372"
            }
          ]
        },
        {
          "id": "543f2587-7794-4feb-9603-2972fb1f1e29",
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
              "id": "d43538bb-6f98-4a82-9655-bc84001a8ffe"
            }
          ]
        },
        {
          "id": "4557c3f4-1575-4d6a-beb2-c798fecc9baa",
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
              "id": "2a59623b-a159-4194-8ea6-40a3663bed29"
            }
          ]
        },
        {
          "id": "bdb7aead-db07-405c-af7a-1471143c660f",
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
              "id": "32d58478-5ec7-46d1-8f7c-75e4f97298af"
            }
          ]
        },
        {
          "id": "cab6c98f-f4fc-4926-a543-fca367e6f818",
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
              "id": "ae85bcac-01e9-46e5-bfac-aa6b36ad4601"
            }
          ]
        },
        {
          "id": "68c91203-15ee-4839-9df7-0e385dc5aebd",
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
              "id": "20d4416f-5f0e-41c1-990a-25b855fc4bd7"
            }
          ]
        },
        {
          "id": "66824b6d-178e-440d-bc90-879777c9c5f9",
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
              "id": "79d02070-b9ae-4d10-99bc-1febbede4bdf"
            }
          ]
        },
        {
          "id": "7c8989fe-dd0f-4be1-814f-2a4642434770",
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
              "id": "a59dc05c-a2fc-46ed-9015-78292f95416e"
            }
          ]
        },
        {
          "id": "30bb922d-65ea-4d40-8c4c-fccbca50de1c",
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
              "id": "98b9558c-f4f8-4d1b-bc45-9f8514556d54"
            }
          ]
        },
        {
          "id": "61528a5b-50ea-4544-8f74-b72136c1f46c",
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
              "id": "975cab8d-a859-4802-b62e-382afebf22ee"
            }
          ]
        },
        {
          "id": "4f729237-db23-465b-8453-593836c70403",
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
              "id": "c5ae04bc-854b-4ef6-b345-492529b8c6f9"
            }
          ]
        },
        {
          "id": "80d18d28-4721-4aa2-afe2-f212098fc0a6",
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
              "id": "7e0c3786-f4f3-4880-8a1e-28eb0d960a11"
            }
          ]
        },
        {
          "id": "298ae036-a5c1-4ecd-96bd-4348aedb4063",
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
              "id": "5be75e0b-c53f-45d7-8554-37767b3738af"
            }
          ]
        },
        {
          "id": "c9a88b51-0556-46f8-b2db-d0304069b359",
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
              "id": "40e5eda6-ac9c-425f-9109-acf2c6932a99"
            }
          ]
        },
        {
          "id": "0c6f3f52-5f4a-444b-af5e-2b394156f9f0",
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
              "id": "8d343ebc-5359-4a92-a1cb-4db1bdbe2935"
            }
          ]
        },
        {
          "id": "58f45f67-049e-42f2-a010-f89aa6f238fe",
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
              "id": "77a95432-9b2d-4f0e-a507-c6674106ff4d"
            }
          ]
        },
        {
          "id": "55dd44c7-9e2d-4654-91c1-751bd6835e58",
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
              "id": "12870292-efa4-4f7e-804a-12a2f4a6d51b"
            }
          ]
        },
        {
          "id": "744c4a03-cf02-47e6-88ff-a7b62763e461",
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
              "id": "e72882e7-d7f0-442d-94a5-05a40e2dd7b8"
            }
          ]
        },
        {
          "id": "5721f8b0-861e-4a1d-8a69-855f81bd1b37",
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
              "id": "d9ab7168-4282-467e-89d8-298245738f02"
            }
          ]
        },
        {
          "id": "8d448bd4-4aab-4aef-8f3a-66f2a4551577",
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
              "id": "ebb6086b-48cc-4d90-9e50-5f37d8dff802"
            }
          ]
        },
        {
          "id": "4ad99740-e8cb-4784-a1ed-ec02a68a8b47",
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
              "id": "d7ec67bc-bcbb-4036-84ca-2c86b28ef693"
            }
          ]
        },
        {
          "id": "3aeff25a-9f90-45d1-89c1-f35ec80b708f",
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
              "id": "93b622ac-3751-4ac9-a34e-1c47c6970073"
            }
          ]
        },
        {
          "id": "e9f141a5-34d4-40b9-ba5c-1e59b2db4807",
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
              "id": "e92550a4-583f-4f80-96fd-1c7cd3ca8efc"
            }
          ]
        },
        {
          "id": "ae93ffea-02c7-4611-9f2e-12172a4123cb",
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
              "id": "68871cf9-564d-417f-92b7-d13df6bee65a"
            }
          ]
        },
        {
          "id": "290f0c7a-1ae2-48e8-9d40-e7b14e8fcc40",
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
              "id": "82eebf46-15e4-4ccb-bedb-f9388611fc13"
            }
          ]
        },
        {
          "id": "02d5ad1f-3dbc-407f-b826-70554ee91007",
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
              "id": "26be12cc-3811-42b3-bccd-d94f75d6b543"
            }
          ]
        },
        {
          "id": "2eec2d24-272d-4bee-9703-d1bbd4faa441",
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
              "id": "67ce132b-f518-4768-9e0c-485aeee75b90"
            }
          ]
        },
        {
          "id": "abe4e928-23ed-4e48-8307-d67dddb5984d",
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
              "id": "fde9004a-0661-40b6-baf1-483dbddd9fb3"
            }
          ]
        },
        {
          "id": "83230853-67f2-43d4-98f3-cc065c8c57dc",
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
              "id": "fb4af007-88cb-4425-88b9-e46c108f5d96"
            }
          ]
        },
        {
          "id": "3ea1bdf3-3d63-41ae-9a28-f8593b7afcac",
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
              "id": "d0d97b39-a172-43c7-a24c-988f9fefeede"
            }
          ]
        },
        {
          "id": "177d5f68-32cd-45c9-95f6-b38c517eacbe",
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
              "id": "e27c1d07-a83a-4bc5-a8c0-a675291fd06d"
            }
          ]
        },
        {
          "id": "507a6074-8b26-4179-a8ae-48eab7a074e6",
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
              "id": "d2e72b11-400f-4d39-8ab2-7af2016f137f"
            }
          ]
        },
        {
          "id": "b45971cb-9731-416e-820a-501c2093d7ce",
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
              "id": "8d50a913-ff82-4bbf-825b-8a360a38e503"
            }
          ]
        },
        {
          "id": "7328d714-f0d5-4db7-b410-8792aeda10a5",
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
              "id": "3430c021-7bc7-450a-b063-9cf873eefb00"
            }
          ]
        },
        {
          "id": "21f30dcc-6ba3-467a-89fe-15afc9251f17",
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
              "id": "01482bc7-b9cf-4b70-95ea-4e36176a59e8"
            }
          ]
        },
        {
          "id": "32577ee5-4d8c-4762-ba00-40dcc3d3f483",
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
              "id": "68b7b5d2-1bb4-475e-8acd-4154b99adcfe"
            }
          ]
        },
        {
          "id": "9931a6cd-a454-4a6d-8ae5-f8b3f4a55665",
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
              "id": "03c2cccd-35e1-452e-bb06-c6d78312c3ca"
            }
          ]
        },
        {
          "id": "940d92e1-e42e-4bbe-9c53-6d94193d0e30",
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
              "id": "b186161e-db35-4695-993e-4a6137b16919"
            }
          ]
        },
        {
          "id": "cbb72539-a215-4b66-92d0-5b93ebfecf60",
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
              "id": "97362429-d8d7-4b37-bd6b-f915c1a9db76"
            }
          ]
        }
      ]
    },
    {
      "name": "Veo",
      "item": [
        {
          "id": "50a9fd76-d845-49b0-9db5-741b6fa11397",
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
              "id": "f1ed2ac8-5581-4782-97c5-828f10fee126"
            }
          ]
        },
        {
          "id": "6d49b012-c011-4073-b005-4d0a1be25356",
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
              "id": "4034637f-ab7c-44ee-9c01-a8b9392ffb64"
            }
          ]
        },
        {
          "id": "5eae4ab9-2c98-4549-a5bd-3fbecc372f3c",
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
              "id": "86b4735e-f3c6-4de1-8379-a01e0e4febb4"
            }
          ]
        }
      ]
    },
    {
      "name": "Asset3d",
      "item": [
        {
          "id": "7e401c76-980c-4074-b6e0-ed272504f5fa",
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
              "id": "daf60412-30f4-4cdf-b2fa-bb9b663ca9f4"
            }
          ]
        }
      ]
    },
    {
      "name": "Work",
      "item": [
        {
          "id": "e82d7a7c-6277-4ecd-abb4-1971a8d48e0d",
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
              "id": "8dce25ea-3d9d-480e-80f7-166de0e47f09"
            }
          ]
        }
      ]
    },
    {
      "name": "App",
      "item": [
        {
          "id": "d7c24165-6fff-4c9c-ab34-b75452d46617",
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
              "id": "9c73ab6f-087b-42f8-8a85-0c1578b4dc65"
            }
          ]
        }
      ]
    },
    {
      "name": "Async",
      "item": [
        {
          "id": "26ee8918-c35d-489a-a46e-b95ec4a90d7f",
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
              "id": "e9cda839-a036-40b6-8f9f-07cecb1ab659"
            }
          ]
        }
      ]
    }
  ]
}