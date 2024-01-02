# Tokopedia API

🌐 **Unleash the Future of E-Commerce with Tokopedia API!**

Are you ready to revolutionize your online business? Dive into the power of Tokopedia API – your key to seamless integration with Indonesia's premier e-commerce platform. Elevate your digital storefront with these incredible features:

### 📂 **List Categories:**
Effortlessly organize and display a comprehensive list of product categories. Navigate through the diverse offerings on Tokopedia seamlessly, enhancing user experience and encouraging exploration.
```
curl --request GET \
	--url https://tokopedia7.p.rapidapi.com/categories \
	--header 'X-RapidAPI-Host: tokopedia7.p.rapidapi.com' \
	--header 'X-RapidAPI-Key: SIGN-UP-FOR-KEY'
```
```json
{
  "success": true,
  "message": "success",
  "results": [
    {
      "identifier": "",
      "name": "Pilihan Untukmu",
      "id": "0",
      "child": [
        {
          "id": "1889",
          "template": "",
          "name": "Gamis Wanita",
          "url": "https://www.tokopedia.com/p/fashion-muslim/dress-muslim-wanita/gamis-wanita",
          "iconImageUrl": "https://images.tokopedia.net/img/cache/300/attachment/2019/12/30/50439068/50439068_ffcb7af5-ff46-4b34-b8be-8524f50328bf.png",
          "child": [],
          "__typename": "AllCategoryResp"
        },
        ...
      ],
      "__typename": "AllCategoryResp"
    },
    ...
  ]
}
```

### 🔍 **Autocomplete:**
Deliver an intuitive and user-friendly search experience. Enable autocomplete functionality to assist users in finding their desired products quickly, making the shopping journey smoother than ever.
```
curl --request GET \
	--url 'https://tokopedia7.p.rapidapi.com/autocomplete?q=iphone' \
	--header 'X-RapidAPI-Host: tokopedia7.p.rapidapi.com' \
	--header 'X-RapidAPI-Key: SIGN-UP-FOR-KEY'
```
```json
{
  "success": true,
  "message": "success",
  "results": [
    {
      "template": "list_single_line",
      "type": "curated",
      "applink": "tokopedia://discovery/deals-c-search?q=Iphone&source=search-autocomplete.04.01.01",
      "url": "https://tokopedia.com/discovery/deals-c-search?q=Iphone&source=search-autocomplete.04.01.01",
      "title": "Iphone di Promo Hari Ini",
      "subtitle": "",
      "icon_title": "",
      "icon_subtitle": "",
      "shortcut_image": "",
      "image_url": "https://images.tokopedia.net/img/blog/promo/2022/10/Deals-dynamic_icon_promo.png",
      "url_tracker": "/tracker/v1?id=434367&user_id=&device=default_v3&unique_id=&type=curated",
      "label": "",
      "label_type": "",
      "tracking": {
        "code": ""
      },
      "discount_percentage": "",
      "original_price": "",
      "tracking_option": 3,
      "component_id": "02.04.01.01",
      "child_items": [],
      "suggestion_id": ""
    },
    ...
  ]
}
```

### ⚡ **Flash Sale:**
Stay ahead of the game with real-time access to flash sales. Integrate Tokopedia's dynamic flash sale data directly into your application, ensuring your users never miss out on exciting deals.
```
curl --request GET \
	--url https://tokopedia7.p.rapidapi.com/flash-sale \
	--header 'X-RapidAPI-Host: tokopedia7.p.rapidapi.com' \
	--header 'X-RapidAPI-Key: SIGN-UP-FOR-KEY'
```
```json
{
  "success": true,
  "message": "success",
  "results": {
    "additional_info": {
      "next_page": "p",
      "redirection": {},
      "total_product": {
        "product_count": 1492,
        "product_count_text": "1.492",
        "product_count_wording": "Tampilkan 1.492 produk"
      }
    },
    "creative_name": "ongoing",
    "data": [
      {
        "active_product_card": true,
        "applink": "tokopedia://product/558841547?extParam=src%3Dmultiloc%26whid%3D13355454",
        "atc_button_cta": "general_atc",
        "badges": [
          {
            "image_url": "https://images.tokopedia.net/img/official_store/badge_os.png",
            "title": "Official Store"
          }
        ],
        "campaign_code": "PG_01 January 24_Harga spesial_2980595",
        "campaign_id": 2980595,
        "campaign_sold_count": 34,
        "custom_stock": 1,
        "department_id": 0,
        "discount_percentage": 30,
        "discounted_price": "Rp145.000",
        "free_ongkir": {
          "img_url": "https://images.tokopedia.net/img/restriction-engine/bebas-ongkir/BO_reguler.png"
        },
        "gold_merchant": false,
        "gtm_item_name": "/discovery/kejar diskon - sprint_sale - #POSITION - nonlogin - product_card_revamp - - non topads - ongoing -  - #MEGA_TAB_VALUE",
        "hasAddToCartButton": false,
        "image_url_desktop": "https://images.tokopedia.net/img/cache/200-square/VqbcmM/2023/8/2/a6d4fe46-1940-4609-bb85-06e1aae4ea13.png",
        "image_url_mobile": "https://images.tokopedia.net/img/cache/200-square/VqbcmM/2023/8/2/a6d4fe46-1940-4609-bb85-06e1aae4ea13.png",
        "is_official": true,
        "is_topads": false,
        "labels": [],
        "max_order": 3,
        "min_order": 1,
        "name": "Nestlé DANCOW 1+ Madu Susu Anak 1-3 Tahun Box 1Kg",
        "parent_id": 0,
        "pdp_view": 0,
        "preorder": false,
        "price": "Rp101.758",
        "product_id": 558841547,
        "shop_applink": "tokopedia://shop/6673792",
        "shop_id": 6673792,
        "shop_location": "Kota Surabaya",
        "shop_logo": "",
        "shop_name": "Dancow Official Store",
        "shop_reputation": "",
        "shop_url_desktop": "https://www.tokopedia.com/dancowofficial",
        "shop_url_mobile": "https://www.tokopedia.com/dancowofficial",
        "show_three_dots_button": true,
        "status": 1,
        "stock": 1,
        "stock_sold_percentage": 97,
        "stock_wording": {
          "color": "#ef144a",
          "title": "Segera Habis"
        },
        "threshold": 7,
        "title": "",
        "topads_click_url": "",
        "topads_view_url": "",
        "url_desktop": "https://www.tokopedia.com/dancowofficial/nestl-dancow-1-madu-susu-anak-1-3-tahun-box-1kg?extParam=src%3Dmultiloc%26whid%3D13355454",
        "url_mobile": "https://www.tokopedia.com/dancowofficial/nestl-dancow-1-madu-susu-anak-1-3-tahun-box-1kg?extParam=src%3Dmultiloc%26whid%3D13355454",
        "warehouse_id": 13355454
      },
      ...
    ],
    "id": 5,
    "name": "product_card_revamp",
    "properties": {
      "active_cart_type": "general_cart",
      "mix_left": {},
      "progress_bar": "dynamic",
      "template": "grid",
      "tokonow_add_to_cart_active": false,
      "tracker_type": "default",
      "type": ""
    },
    "render_by_default": true,
    "skiprender": false
  }
}
```

### 🏬 **Shop Info:**
Provide users with detailed information about their favorite shops. From basic details to special promotions, display everything users need to know to build trust and loyalty.
```
curl --request GET \
	--url https://tokopedia7.p.rapidapi.com/shop/r2hcover \
	--header 'X-RapidAPI-Host: tokopedia7.p.rapidapi.com' \
	--header 'X-RapidAPI-Key: SIGN-UP-FOR-KEY'
```
```json
{
  "success": true,
  "message": "success",
  "results": {
    "shopCore": {
      "description": "mengutamakan kepuasan pelanggan siap bertanggung jawab dalam penjualan kami, Claim Garansi Wajib Vidio Unboxing,",
      "domain": "r2hcover",
      "shopID": "3768133",
      "name": "R2H COVER",
      "tagLine": "cepat amanah dan bertanggung jawab",
      "defaultSort": 2,
      "__typename": "shopCoreData"
    },
    "createInfo": {
      "openSince": "July 2018",
      "__typename": "createData"
    },
    "favoriteData": {
      "totalFavorite": 1104,
      "alreadyFavorited": 0,
      "__typename": "favData"
    },
    "activeProduct": 88,
    "shopAssets": {
      "avatar": "https://images.tokopedia.net/img/cache/215-square/GAnVPX/2021/6/27/d3a32c50-484b-478f-a74a-cb56a36a266d.jpg",
      "cover": "https://images.tokopedia.net/img/cache/1334/BpoSLE/seller_no_cover_1.png",
      "__typename": "imageData"
    },
    "location": "Kota Bandung",
    "isAllowManage": 0,
    "branchLinkDomain": "",
    "isOpen": 1,
    "shipmentInfo": [
      {
        "isAvailable": 1,
        "image": "https://images.tokopedia.net/img/kurir-sicepat.png",
        "name": "SiCepat",
        "product": [
          {
            "isAvailable": 1,
            "productName": "Regular Package",
            "uiHidden": false,
            "__typename": "shipmentProductData"
          },
          {
            "isAvailable": 1,
            "productName": "Regular Package",
            "uiHidden": true,
            "__typename": "shipmentProductData"
          },
          {
            "isAvailable": 1,
            "productName": "BEST",
            "uiHidden": false,
            "__typename": "shipmentProductData"
          },
          {
            "isAvailable": 1,
            "productName": "GOKIL",
            "uiHidden": false,
            "__typename": "shipmentProductData"
          }
        ],
        "__typename": "shipmentData"
      },
      {
        "isAvailable": 1,
        "image": "https://images.tokopedia.net/img/kurir-grab.png",
        "name": "GrabExpress",
        "product": [
          {
            "isAvailable": 1,
            "productName": "Instant 3 Jam",
            "uiHidden": false,
            "__typename": "shipmentProductData"
          }
        ],
        "__typename": "shipmentData"
      },
      {
        "isAvailable": 1,
        "image": "https://images.tokopedia.net/img/kurir-jnt.png",
        "name": "J&T",
        "product": [
          {
            "isAvailable": 1,
            "productName": "Reguler",
            "uiHidden": false,
            "__typename": "shipmentProductData"
          }
        ],
        "__typename": "shipmentData"
      },
      {
        "isAvailable": 1,
        "image": "https://images.tokopedia.net/img/kurir-jne.png",
        "name": "JNE",
        "product": [
          {
            "isAvailable": 1,
            "productName": "Reguler",
            "uiHidden": false,
            "__typename": "shipmentProductData"
          },
          {
            "isAvailable": 1,
            "productName": "OKE",
            "uiHidden": false,
            "__typename": "shipmentProductData"
          }
        ],
        "__typename": "shipmentData"
      },
      {
        "isAvailable": 1,
        "image": "https://images.tokopedia.net/img/kurir-gosend.png",
        "name": "GoSend",
        "product": [
          {
            "isAvailable": 1,
            "productName": "Instant 3 Jam",
            "uiHidden": false,
            "__typename": "shipmentProductData"
          },
          {
            "isAvailable": 1,
            "productName": "Instant 3 Jam",
            "uiHidden": true,
            "__typename": "shipmentProductData"
          }
        ],
        "__typename": "shipmentData"
      },
      {
        "isAvailable": 1,
        "image": "https://images.tokopedia.net/img/kurir-anteraja.png",
        "name": "AnterAja",
        "product": [
          {
            "isAvailable": 1,
            "productName": "Reguler",
            "uiHidden": false,
            "__typename": "shipmentProductData"
          },
          {
            "isAvailable": 1,
            "productName": "Same Day",
            "uiHidden": false,
            "__typename": "shipmentProductData"
          },
          {
            "isAvailable": 1,
            "productName": "Next Day",
            "uiHidden": false,
            "__typename": "shipmentProductData"
          },
          {
            "isAvailable": 1,
            "productName": "Economy",
            "uiHidden": false,
            "__typename": "shipmentProductData"
          },
          {
            "isAvailable": 1,
            "productName": "Cargo",
            "uiHidden": false,
            "__typename": "shipmentProductData"
          }
        ],
        "__typename": "shipmentData"
      }
    ],
    "shippingLoc": {
      "districtName": "Bandung Kulon",
      "cityName": "Kota Bandung",
      "__typename": "shippingLocData"
    },
    "shopStats": {
      "productSold": "18675",
      "totalTxSuccess": "17746",
      "totalShowcase": "10",
      "__typename": "statsData"
    },
    "statusInfo": {
      "shopStatus": 1,
      "statusMessage": "",
      "statusTitle": "",
      "tickerType": "warning",
      "__typename": "statusData"
    },
    "closedInfo": {
      "closedNote": "",
      "until": "",
      "reason": "",
      "detail": {
        "status": 0,
        "__typename": "closedInfoDetail"
      },
      "__typename": "closedInfoData"
    },
    "bbInfo": [],
    "goldOS": {
      "isGold": 1,
      "isGoldBadge": 1,
      "isOfficial": 0,
      "badge": "https://images.tokopedia.net/img/goldmerchant/pm_activation/badge/Power%20Merchant%20Pro.png",
      "shopTier": 3,
      "__typename": "goldOSData"
    },
    "shopSnippetURL": "https://seller.tokopedia.com/imgshare/shop_snippet/ZGVmZ2hpamtsbW5v0LQFVwP4foauxrFdwb9GzjO8hPZlRWGTLjRG6TZx3Q==.png",
    "customSEO": {
      "title": "Toko R2H COVER Online - Produk Lengkap & Harga Terbaik",
      "description": "Beli produk R2H COVER online, produk terlengkap dan harga terbaik. Dapatkan berbagai promo menarik. Belanja aman dan nyaman hanya di Tokopedia.",
      "bottomContent": "<h2><strong>Beli Aneka Produk Online dari Toko R2H COVER di Tokopedia</strong></h2><p><span style=\"font-weight: 400;\">Beli aneka produk di Toko R2H COVER secara online sekarang. Kamu bisa beli produk dari Toko R2H COVER dengan aman & mudah dari Kota Bandung. Ingin belanja lebih hemat & terjangkau di Toko R2H COVER? Kamu bisa gunakan fitur Cicilan 0% dari berbagai bank dan fitur Bebas Ongkir di Toko R2H COVER sehingga kamu bisa belanja online dengan nyaman di Tokopedia. Beli aneka produk terbaru di Toko R2H COVER dengan mudah dari genggaman tangan kamu menggunakan Aplikasi Tokopedia. Cek terus juga Toko R2H COVER untuk update Produk, Kode Voucher hingga Promo Terbaru dari Toko R2H COVER Terbaru secara online di Tokopedia!</span></p>",
      "__typename": "customSEOData"
    },
    "isQA": false,
    "isGoApotik": false,
    "partnerInfo": [
      {
        "fsType": 0,
        "__typename": "partnerInfoData"
      }
    ],
    "__typename": "TokoShopInfoData"
  }
}
```

### 🛍️ **Shop Product:**
Access and showcase a shop's entire product catalog seamlessly. Empower your users to explore a shop's offerings effortlessly, creating a captivating shopping experience.
```
curl --request GET \
	--url https://tokopedia7.p.rapidapi.com/shop/3768133/products \
	--header 'X-RapidAPI-Host: tokopedia7.p.rapidapi.com' \
	--header 'X-RapidAPI-Key: SIGN-UP-FOR-KEY'
```
```json
{
  "success": true,
  "message": "success",
  "results": [
    {
      "name": "Cover Mobil Rush, Konde. Sarung Mobil Rush Konde, Polyester Premium",
      "product_url": "https://www.tokopedia.com/r2hcover/cover-mobil-rush-konde-sarung-mobil-rush-konde-polyester-premium-abumuda-rush-lama-konde-eab50?extParam=src%3Dshop%26whid%3D2871280",
      "product_id": "9593871664",
      "price": {
        "text_idr": "Rp275.000",
        "__typename": "ProductListPrice"
      },
      "primary_image": {
        "original": "https://images.tokopedia.net/img/cache/300-square/VqbcmM/2023/5/19/52b15ac7-651e-43cf-a84f-c56bfe05f868.jpg",
        "thumbnail": "https://images.tokopedia.net/img/cache/200-square/VqbcmM/2023/5/19/52b15ac7-651e-43cf-a84f-c56bfe05f868.jpg",
        "resize300": "https://images.tokopedia.net/img/cache/300-square/VqbcmM/2023/5/19/52b15ac7-651e-43cf-a84f-c56bfe05f868.jpg",
        "__typename": "ProductListPrimaryImage"
      },
      "flags": {
        "isSold": false,
        "isPreorder": false,
        "isWholesale": false,
        "isWishlist": false,
        "__typename": "ProductListFlagNew"
      },
      "campaign": {
        "discounted_percentage": "0",
        "original_price_fmt": "",
        "start_date": "",
        "end_date": "",
        "__typename": "ProductDetailCampaignType"
      },
      "label": [],
      "label_groups": [
        {
          "position": "price",
          "title": "Cashback 16,5rb",
          "type": "lightGreen",
          "url": "",
          "__typename": "tomeLabelGroup"
        },
        {
          "position": "integrity",
          "title": "13 terjual",
          "type": "textDarkGrey",
          "url": "",
          "__typename": "tomeLabelGroup"
        }
      ],
      "badge": [
        {
          "title": "Power Merchant Pro Badge",
          "image_url": "https://images.tokopedia.net/img/goldmerchant/pm_activation/badge/PM%20Pro%20Small.png",
          "__typename": "ShopBadge"
        }
      ],
      "stats": {
        "reviewCount": 10,
        "rating": 98,
        "averageRating": "4.9",
        "__typename": "ProductListStats"
      },
      "category": {
        "id": "0",
        "__typename": "ProductListCategory"
      },
      "__typename": "ShopProductListDetail"
    },
    ...
  ]
}
```

### 🔍 **Product Search:**
Enable users to find products quickly and accurately. Leverage Tokopedia's powerful search capabilities to deliver precise search results, making it easy for users to discover what they need.
```
curl --request GET \
	--url 'https://tokopedia7.p.rapidapi.com/product/search?q=iphone' \
	--header 'X-RapidAPI-Host: tokopedia7.p.rapidapi.com' \
	--header 'X-RapidAPI-Key: SIGN-UP-FOR-KEY'
```
```json
{
  "success": true,
  "message": "success",
  "results": {
    "header": {
      "totalData": 196238,
      "totalDataText": "196rb+",
      "processTime": 0.060709716,
      "responseCode": 0,
      "errorMessage": "",
      "additionalParams": "",
      "keywordProcess": "6",
      "componentId": "04.06.00.00",
      "__typename": "AceSearchUnifyHeader"
    },
    "data": {
      "banner": {
        "position": 0,
        "text": "",
        "imageUrl": "",
        "url": "",
        "componentId": "",
        "trackingOption": 0,
        "__typename": "AceSearchUnifyBanner"
      },
      "backendFilters": "&ob=2",
      "isQuerySafe": true,
      "ticker": {
        "text": "",
        "query": "",
        "typeId": 0,
        "componentId": "",
        "trackingOption": 0,
        "__typename": "AceSearchUnifyTicker"
      },
      "redirection": {
        "redirectUrl": "",
        "departmentId": 0,
        "__typename": "AceSearchUnifyRedirection"
      },
      "related": {
        "position": 0,
        "trackingOption": 0,
        "relatedKeyword": "",
        "otherRelated": [],
        "__typename": "AceSearchUnifyRelated"
      },
      "suggestion": {
        "currentKeyword": "iphone",
        "suggestion": "",
        "suggestionCount": 0,
        "instead": "",
        "insteadCount": 0,
        "query": "",
        "text": "",
        "componentId": "",
        "trackingOption": 0,
        "__typename": "AceSearchUnifySuggestion"
      },
      "products": [
        {
          "id": 2783580239,
          "name": "NEW Apple iPhone 11 64GB 128GB 256GB Garansi Resmi iBox TAM GDN",
          "ads": {
            "adsId": "",
            "productClickUrl": "",
            "productWishlistUrl": "",
            "productViewUrl": "",
            "__typename": "AceSearchUnifyAds"
          },
          "badges": [
            {
              "title": "Official Store",
              "imageUrl": "https://images.tokopedia.net/img/official_store_badge.png",
              "show": true,
              "__typename": "AceSearchUnifyBadge"
            }
          ],
          "category": 3055,
          "categoryBreadcrumb": "handphone-tablet/handphone/ios",
          "categoryId": 65,
          "categoryName": "Handphone & Tablet",
          "countReview": 97,
          "customVideoURL": "",
          "discountPercentage": 8,
          "gaKey": "/searchproduct/handphone-tablet/handphone/ios/iphone/goodponsel/new-apple-iphone-11-64gb-128gb-256gb-garansi-resmi-ibox-tam-gdn-11-ibox-64gb-5ec72",
          "imageUrl": "https://images.tokopedia.net/img/cache/250-square/VqbcmM/2023/10/5/033a9323-910a-42b1-b3ef-cb15dbe28dce.png",
          "labelGroups": [
            {
              "position": "price",
              "title": "Cashback 139,9rb",
              "type": "lightGreen",
              "url": "",
              "__typename": "AceSearchUnifyLabelGroup"
            },
            {
              "position": "integrity",
              "title": "100+ terjual",
              "type": "textDarkGrey",
              "url": "",
              "__typename": "AceSearchUnifyLabelGroup"
            },
            {
              "position": "eta",
              "title": "Tiba 3 - 7 Jan",
              "type": "textDarkGrey",
              "url": "",
              "__typename": "AceSearchUnifyLabelGroup"
            }
          ],
          "originalPrice": "Rp7,59jt",
          "price": "Rp6.999.000",
          "priceRange": "Rp6,99jt - Rp8,49jt",
          "rating": 5,
          "ratingAverage": "5.0",
          "shop": {
            "shopId": 1086539,
            "name": "GoodPonsel",
            "url": "https://www.tokopedia.com/goodponsel",
            "city": "Surabaya",
            "isOfficial": true,
            "isPowerBadge": true,
            "__typename": "AceSearchUnifyShop"
          },
          "url": "https://www.tokopedia.com/goodponsel/new-apple-iphone-11-64gb-128gb-256gb-garansi-resmi-ibox-tam-gdn-11-ibox-64gb-5ec72?extParam=ivf%3Dfalse%26src%3Dsearch%26whid%3D16574388",
          "wishlist": false,
          "sourceEngine": "0",
          "warehouseIdDefault": 16574388,
          "__typename": "AceSearchUnifyProduct"
        },
        ...
      ],
      "violation": {
        "headerText": "",
        "descriptionText": "",
        "imageURL": "",
        "ctaURL": "",
        "ctaApplink": "",
        "buttonText": "",
        "buttonType": "",
        "__typename": "AceSearchUnifyViolation"
      },
      "__typename": "AceSearchUnifyData"
    },
    "__typename": "AceSearchUnifyResponse"
  }
}
```

### 📦 **Product Detail:**
Present users with rich and detailed product information. Showcase product specifications, images, and pricing, ensuring users have all the details they need to make informed decisions.
```
curl --request GET \
	--url 'https://tokopedia7.p.rapidapi.com/product/detail?shopDomain=etawalinofficial&productKey=etawalin-susu-etawa-original-atasi-nyeri-sendi-dan-asam-urat-1-box' \
	--header 'X-RapidAPI-Host: tokopedia7.p.rapidapi.com' \
	--header 'X-RapidAPI-Key: SIGN-UP-FOR-KEY'
```
```json
{
  "success": true,
  "message": "success",
  "results": {
    "basicInfo": {
      "alias": "etawalin-susu-etawa-original-atasi-nyeri-sendi-dan-asam-urat-1-box",
      "createdAt": "2022-09-20T20:57:12+07:00",
      "isQA": false,
      "id": "6301766083",
      "shopID": "14212194",
      "shopName": "Etawalin",
      "minOrder": 1,
      "maxOrder": 23846,
      "weight": 250,
      "weightUnit": "GRAM",
      "condition": "NEW",
      "status": "ACTIVE",
      "url": "https://www.tokopedia.com/etawalinofficial/etawalin-susu-etawa-original-atasi-nyeri-sendi-dan-asam-urat-1-box",
      "needPrescription": false,
      "catalogID": "0",
      "isLeasing": false,
      "isBlacklisted": false,
      "isTokoNow": false,
      "menu": {
        "id": "35010653",
        "name": "Produk Terlaris",
        "url": "https://www.tokopedia.com/etawalinofficial/etalase/produk-terlaris",
        "__typename": "pdpMenu"
      },
      "category": {
        "id": "2717",
        "name": "Susu Bubuk Dewasa",
        "title": "Susu Bubuk Dewasa",
        "breadcrumbURL": "https://www.tokopedia.com/p/makanan-minuman/susu-olahan-susu/susu-bubuk-dewasa",
        "isAdult": false,
        "isKyc": false,
        "minAge": 0,
        "detail": [
          {
            "id": "35",
            "name": "Makanan & Minuman",
            "breadcrumbURL": "https://www.tokopedia.com/p/makanan-minuman",
            "isAdult": false,
            "__typename": "pdpCategoryDetail"
          },
          {
            "id": "2690",
            "name": "Susu & Olahan Susu",
            "breadcrumbURL": "https://www.tokopedia.com/p/makanan-minuman/susu-olahan-susu",
            "isAdult": false,
            "__typename": "pdpCategoryDetail"
          },
          {
            "id": "2717",
            "name": "Susu Bubuk Dewasa",
            "breadcrumbURL": "https://www.tokopedia.com/p/makanan-minuman/susu-olahan-susu/susu-bubuk-dewasa",
            "isAdult": false,
            "__typename": "pdpCategoryDetail"
          }
        ],
        "__typename": "pdpCategory"
      },
      "txStats": {
        "transactionSuccess": "5571",
        "transactionReject": "21",
        "countSold": "8327",
        "paymentVerified": "5701",
        "itemSoldFmt": "11,4 rb",
        "__typename": "pdpTxStats"
      },
      "stats": {
        "countView": "32843",
        "countReview": "2973",
        "countTalk": "51",
        "rating": 4.9,
        "__typename": "pdpStats"
      },
      "__typename": "pdpBasicInfo"
    },
    "components": [
      {
        "name": "product_snapshot",
        "type": "product_snapshot",
        "position": "[0,0,1,1]",
        "data": [
          {
            "__typename": "pdpDataProductSnapshot"
          }
        ],
        "__typename": "pdpComponent"
      },
      {
        "name": "product_media",
        "type": "product_media",
        "position": "[0,1,1,1]",
        "data": [
          {
            "media": [
              {
                "type": "video",
                "urlOriginal": "https://images.tokopedia.net/img/cache/700/VqbcmM/2023/4/18/ba13ed2b-484f-4df6-a763-331c7bc77e1d.png",
                "urlThumbnail": "https://images.tokopedia.net/img/cache/200-square/VqbcmM/2023/4/18/ba13ed2b-484f-4df6-a763-331c7bc77e1d.png",
                "urlMaxRes": "https://images.tokopedia.net/img/cache/700/VqbcmM/2023/4/18/ba13ed2b-484f-4df6-a763-331c7bc77e1d.png",
                "videoUrl": "https://vod.tokopedia.com/view/adaptive.m3u8?id=247d1670507471ee9f3687c7361c0102",
                "prefix": "https://images.tokopedia.net/img/cache/",
                "suffix": "/VqbcmM/2023/4/18/ba13ed2b-484f-4df6-a763-331c7bc77e1d.png",
                "description": "",
                "variantOptionID": "0",
                "__typename": "pdpContentSnapshotMedia"
              },
              {
                "type": "image",
                "urlOriginal": "https://images.tokopedia.net/img/cache/700/VqbcmM/2023/4/18/ba13ed2b-484f-4df6-a763-331c7bc77e1d.png",
                "urlThumbnail": "https://images.tokopedia.net/img/cache/200-square/VqbcmM/2023/4/18/ba13ed2b-484f-4df6-a763-331c7bc77e1d.png",
                "urlMaxRes": "https://images.tokopedia.net/img/cache/700/VqbcmM/2023/4/18/ba13ed2b-484f-4df6-a763-331c7bc77e1d.png",
                "videoUrl": "",
                "prefix": "",
                "suffix": "",
                "description": "",
                "variantOptionID": "0",
                "__typename": "pdpContentSnapshotMedia"
              },
              {
                "type": "image",
                "urlOriginal": "https://images.tokopedia.net/img/cache/700/VqbcmM/2023/3/9/bc3b13d0-42f1-45c3-9aba-fe720bc09e1b.jpg",
                "urlThumbnail": "https://images.tokopedia.net/img/cache/200-square/VqbcmM/2023/3/9/bc3b13d0-42f1-45c3-9aba-fe720bc09e1b.jpg",
                "urlMaxRes": "https://images.tokopedia.net/img/cache/700/VqbcmM/2023/3/9/bc3b13d0-42f1-45c3-9aba-fe720bc09e1b.jpg",
                "videoUrl": "",
                "prefix": "",
                "suffix": "",
                "description": "",
                "variantOptionID": "0",
                "__typename": "pdpContentSnapshotMedia"
              },
              {
                "type": "image",
                "urlOriginal": "https://images.tokopedia.net/img/cache/700/VqbcmM/2023/3/9/addb7851-a9fe-4faa-a00f-c008b0a4e553.jpg",
                "urlThumbnail": "https://images.tokopedia.net/img/cache/200-square/VqbcmM/2023/3/9/addb7851-a9fe-4faa-a00f-c008b0a4e553.jpg",
                "urlMaxRes": "https://images.tokopedia.net/img/cache/700/VqbcmM/2023/3/9/addb7851-a9fe-4faa-a00f-c008b0a4e553.jpg",
                "videoUrl": "",
                "prefix": "",
                "suffix": "",
                "description": "",
                "variantOptionID": "0",
                "__typename": "pdpContentSnapshotMedia"
              },
              {
                "type": "image",
                "urlOriginal": "https://images.tokopedia.net/img/cache/700/VqbcmM/2023/3/9/99d1b559-f605-4e47-9885-841b382529a5.jpg",
                "urlThumbnail": "https://images.tokopedia.net/img/cache/200-square/VqbcmM/2023/3/9/99d1b559-f605-4e47-9885-841b382529a5.jpg",
                "urlMaxRes": "https://images.tokopedia.net/img/cache/700/VqbcmM/2023/3/9/99d1b559-f605-4e47-9885-841b382529a5.jpg",
                "videoUrl": "",
                "prefix": "",
                "suffix": "",
                "description": "",
                "variantOptionID": "0",
                "__typename": "pdpContentSnapshotMedia"
              },
              {
                "type": "image",
                "urlOriginal": "https://images.tokopedia.net/img/cache/700/VqbcmM/2023/3/9/f52d8497-1357-4589-a925-fb12ab52b43a.jpg",
                "urlThumbnail": "https://images.tokopedia.net/img/cache/200-square/VqbcmM/2023/3/9/f52d8497-1357-4589-a925-fb12ab52b43a.jpg",
                "urlMaxRes": "https://images.tokopedia.net/img/cache/700/VqbcmM/2023/3/9/f52d8497-1357-4589-a925-fb12ab52b43a.jpg",
                "videoUrl": "",
                "prefix": "",
                "suffix": "",
                "description": "",
                "variantOptionID": "0",
                "__typename": "pdpContentSnapshotMedia"
              }
            ],
            "videos": [
              {
                "source": "youtube",
                "url": "BB2IkXmvHdE",
                "__typename": "pdpContentSnapshotVideos"
              }
            ],
            "__typename": "pdpDataProductMedia"
          }
        ],
        "__typename": "pdpComponent"
      },
      {
        "name": "ticker_info",
        "type": "ticker_info",
        "position": "[0,2,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "button_ar",
        "type": "button_ar",
        "position": "[0,3,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "ongoing_campaign",
        "type": "ongoing_campaign",
        "position": "[0,4,1,1]",
        "data": [
          {
            "__typename": "pdpDataOnGoingCampaign"
          }
        ],
        "__typename": "pdpComponent"
      },
      {
        "name": "product_content",
        "type": "product_content",
        "position": "[0,7,1,1]",
        "data": [
          {
            "name": "Etawalin Susu Etawa Original Atasi Nyeri Sendi dan Asam Urat 1 Box",
            "price": {
              "value": 90000,
              "currency": "IDR",
              "priceFmt": "Rp90.000",
              "slashPriceFmt": "",
              "discPercentage": "",
              "__typename": "pdpContentSnapshotPrice"
            },
            "campaign": {
              "campaignID": "0",
              "campaignType": "0",
              "campaignTypeName": "",
              "campaignIdentifier": 0,
              "background": "",
              "percentageAmount": 0,
              "originalPrice": 0,
              "discountedPrice": 0,
              "originalStock": 0,
              "stock": 0,
              "stockSoldPercentage": 0,
              "threshold": 0,
              "startDate": "",
              "endDate": "",
              "endDateUnix": "0",
              "appLinks": "",
              "isAppsOnly": false,
              "isActive": false,
              "hideGimmick": false,
              "__typename": "pdpContentSnapshotCampaign"
            },
            "thematicCampaign": {
              "additionalInfo": "",
              "background": "",
              "campaignName": "",
              "icon": "",
              "__typename": "pdpContentSnapshotThematicCampaign"
            },
            "stock": {
              "useStock": true,
              "value": "23846",
              "stockWording": "",
              "__typename": "pdpContentSnapshotStock"
            },
            "variant": {
              "isVariant": false,
              "parentID": "0",
              "__typename": "pdpContentSnapshotVariant"
            },
            "wholesale": [
              {
                "minQty": 3,
                "price": {
                  "value": 87000,
                  "currency": "IDR",
                  "__typename": "pdpContentSnapshotPrice"
                },
                "__typename": "pdpContentSnapshotWholesale"
              },
              {
                "minQty": 12,
                "price": {
                  "value": 85000,
                  "currency": "IDR",
                  "__typename": "pdpContentSnapshotPrice"
                },
                "__typename": "pdpContentSnapshotWholesale"
              },
              {
                "minQty": 25,
                "price": {
                  "value": 82500,
                  "currency": "IDR",
                  "__typename": "pdpContentSnapshotPrice"
                },
                "__typename": "pdpContentSnapshotWholesale"
              }
            ],
            "isCashback": {
              "percentage": 0,
              "__typename": "pdpContentSnapshotIsCashback"
            },
            "isTradeIn": false,
            "isOS": false,
            "isPowerMerchant": true,
            "isWishlist": false,
            "isCOD": false,
            "preorder": {
              "duration": 0,
              "timeUnit": "UNKNOWN",
              "isActive": false,
              "preorderInDays": 0,
              "__typename": "pdpContentSnapshotPreorder"
            },
            "__typename": "pdpDataProductContent"
          }
        ],
        "__typename": "pdpComponent"
      },
      {
        "name": "social_proof_mini",
        "type": "social_proof_mini",
        "position": "[0,11,1,1]",
        "data": [
          {
            "__typename": "pdpDataComponentSocialProofV2"
          }
        ],
        "__typename": "pdpComponent"
      },
      {
        "name": "mini_variant_options",
        "type": "variant",
        "position": "[0,16,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "bmgm_sneak_peek",
        "type": "bmgm",
        "position": "[0,19,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "product_detail_media",
        "type": "product_detail_media",
        "position": "[0,21,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "product_detail",
        "type": "product_detail",
        "position": "[0,22,1,1]",
        "data": [
          {
            "content": [
              {
                "title": "Kondisi",
                "subtitle": "Baru",
                "applink": "",
                "showAtFront": true,
                "isAnnotation": false,
                "__typename": "pdpContentProductDetail"
              },
              {
                "title": "Berat Satuan",
                "subtitle": "250 g",
                "applink": "",
                "showAtFront": false,
                "isAnnotation": false,
                "__typename": "pdpContentProductDetail"
              },
              {
                "title": "Min. Pemesanan",
                "subtitle": "1 Buah",
                "applink": "",
                "showAtFront": true,
                "isAnnotation": false,
                "__typename": "pdpContentProductDetail"
              },
              {
                "title": "Kategori",
                "subtitle": "Susu Bubuk Dewasa",
                "applink": "https://www.tokopedia.com/p/makanan-minuman/susu-olahan-susu/susu-bubuk-dewasa",
                "showAtFront": false,
                "isAnnotation": false,
                "__typename": "pdpContentProductDetail"
              },
              {
                "title": "Etalase",
                "subtitle": "Produk Terlaris",
                "applink": "https://www.tokopedia.com/etawalinofficial/etalase/produk-terlaris",
                "showAtFront": true,
                "isAnnotation": false,
                "__typename": "pdpContentProductDetail"
              },
              {
                "title": "Deskripsi",
                "subtitle": "🚛 𝐏𝐄𝐍𝐆𝐈𝐑𝐈𝐌𝐀𝐍 𝐒𝐄𝐍𝐈𝐍 - 𝐒𝐀𝐁𝐓𝐔 🚛\nPengiriman Instan - Sameday Ready!!!\n\nSTOK READY 100 %\n✅𝐃𝐞𝐭𝐚𝐢𝐥 𝐏𝐫𝐨𝐝𝐮𝐜𝐭✅\nNama product : Etawalin\nBerat Bersih : 200gr\nBPOM : POM TR232052411\n\nEtawalin - Susu Kambing Etawa 100% Original Solusi Atasi Nyeri Sendi\n\nApakah Anda sering mengalami nyeri sendi❓\n👉🏻 Asam urat sering kambuh❓\n👉🏻 Badan nyeri karena rematik ❓\n👉🏻 Khawatir tulang tak lagi padat❓\n\nAWASS❗❗\nJangan anggap remeh, itu adalah ciri-ciri kesehatan tulang anda menurun\nApa yang terjadi bila Reumatik dan nyeri sendi tidak diobati?\n👉🏻 Osteoartritis (Radang Sendi)\n👉🏻 Osteoporosis (Pengapuran Tulang)\n👉🏻 Tulang Melemah\n\nJangan khawatir!\nKami merekomendasikan Etawalin\nEtawalin adalah minuman susu yang terbuat dari susu kambing etawa asli yang dipadukan dengan 5 herbal alami yang diciptakan khusus untuk penderita reumatik, nyeri sendi, hingga asam urat dan sangat berguna untuk meningkatkan kesehatan dan kepadatan tulang.\n\n🟠Kelebihan Produk :\n✅100% Original\n✅Bahan berkualitas\n✅Sudah terdaftar di BPOM\n✅Terbukti berkhasiat\n\n🟠Aturan minum :\n⏰ 2 x 1 sendok makan/hari\n\nHarga 1 Box Etawalin @90.0000/Box\nHarga 3 Box Etawalin @87.000/Box\nPaket 12 Box Etawalin Harga Spesial @85.000 (𝐋𝐞𝐛𝐢𝐡 𝐇𝐞𝐦𝐚𝐭).\nBeli 25 Box Etawalin Harga Spesial @82.500 ((𝐒𝐚𝐧𝐠𝐚𝐭 𝐋𝐞𝐛𝐢𝐡 𝐇𝐞𝐦𝐚𝐭)\n\n#SusuKambingEtawa #MeredakanNyeriSendi #NyeriSendi #ObatNyeriSendi #ObatNyeriSendi #SusuKesehatan #Etawalin #SusuNyeriSendi #SusuAsamUrat\n#SusuEtawalin #EtawalinOriginal",
                "applink": "",
                "showAtFront": true,
                "isAnnotation": false,
                "__typename": "pdpContentProductDetail"
              },
              {
                "title": "Alergen",
                "subtitle": "Mengandung Laktosa",
                "applink": "",
                "showAtFront": false,
                "isAnnotation": true,
                "__typename": "pdpContentProductDetail"
              },
              {
                "title": "Komposisi",
                "subtitle": "Pemanis",
                "applink": "",
                "showAtFront": false,
                "isAnnotation": true,
                "__typename": "pdpContentProductDetail"
              },
              {
                "title": "Konsumsi Dalam",
                "subtitle": "90 Hari",
                "applink": "",
                "showAtFront": false,
                "isAnnotation": true,
                "__typename": "pdpContentProductDetail"
              },
              {
                "title": "Merek",
                "subtitle": "Etawa",
                "applink": "",
                "showAtFront": false,
                "isAnnotation": true,
                "__typename": "pdpContentProductDetail"
              },
              {
                "title": "Preferensi Diet",
                "subtitle": "Produk Bebas Gluten",
                "applink": "",
                "showAtFront": false,
                "isAnnotation": true,
                "__typename": "pdpContentProductDetail"
              }
            ],
            "__typename": "pdpDataProductDetail"
          }
        ],
        "__typename": "pdpComponent"
      },
      {
        "name": "imei",
        "type": "custom_info",
        "position": "[0,24,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "separator",
        "type": "separator",
        "position": "[0,29,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "shop_credibility",
        "type": "shop_credibility",
        "position": "[0,31,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "review_list",
        "type": "review_list",
        "position": "[0,32,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "other_offers",
        "type": "custom_info_title",
        "position": "[0,37,1,1]",
        "data": [
          {
            "__typename": "pdpDataCustomInfoTitle"
          }
        ],
        "__typename": "pdpComponent"
      },
      {
        "name": "tradein",
        "type": "info",
        "position": "[0,40,1,1]",
        "data": [
          {
            "icon": "https://images.tokopedia.net/pdp/info/icon/Tradein@3x.png",
            "title": "Beli dengan Tukar Tambah",
            "isApplink": true,
            "applink": "",
            "content": [],
            "__typename": "pdpDataInfo"
          }
        ],
        "__typename": "pdpComponent"
      },
      {
        "name": "wholesale",
        "type": "info",
        "position": "[0,44,1,1]",
        "data": [
          {
            "icon": "",
            "title": "Harga Grosir",
            "isApplink": true,
            "applink": "",
            "content": [],
            "__typename": "pdpDataInfo"
          }
        ],
        "__typename": "pdpComponent"
      },
      {
        "name": "palugada",
        "type": "custom_info",
        "position": "[0,45,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "order_prio",
        "type": "info",
        "position": "[0,47,1,1]",
        "data": [
          {
            "icon": "https://images.tokopedia.net/pdp/info/icon/pdp-orderprio@3x.png",
            "title": "Order Prioritas",
            "isApplink": false,
            "applink": "",
            "content": [],
            "__typename": "pdpDataInfo"
          }
        ],
        "__typename": "pdpComponent"
      },
      {
        "name": "separator",
        "type": "separator",
        "position": "[0,48,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "separator",
        "type": "separator",
        "position": "[0,49,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "pdp_1",
        "type": "product_list",
        "position": "[0,50,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "pdp_fbt_hatc",
        "type": "product_list",
        "position": "[0,51,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "separator",
        "type": "separator",
        "position": "[0,52,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "review",
        "type": "review",
        "position": "[0,53,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "separator",
        "type": "separator",
        "position": "[0,55,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "kg_bestseller",
        "type": "product_list",
        "position": "[0,56,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "pdp_2",
        "type": "product_list",
        "position": "[0,57,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "discussion",
        "type": "discussion",
        "position": "[0,58,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "comparison_bpc",
        "type": "product_list",
        "position": "[0,60,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "report",
        "type": "report",
        "position": "[0,62,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "tdn_topads",
        "type": "banner_ads",
        "position": "[0,63,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "pdp_3",
        "type": "product_list",
        "position": "[0,65,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "kg_instant",
        "type": "product_list",
        "position": "[0,66,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "comparison",
        "type": "product_list",
        "position": "[0,67,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "view-to-view",
        "type": "view-to-view",
        "position": "[0,68,1,1]",
        "data": [
          {
            "__typename": "pdpDataProductListComponent"
          }
        ],
        "__typename": "pdpComponent"
      },
      {
        "name": "pdp_7",
        "type": "product_list",
        "position": "[0,69,1,1]",
        "data": [
          {
            "__typename": "pdpDataProductListComponent"
          }
        ],
        "__typename": "pdpComponent"
      },
      {
        "name": "pdp_4",
        "type": "product_list",
        "position": "[0,70,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "shopads_carousel",
        "type": "product_list",
        "position": "[0,71,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "pdp_9_tokonow",
        "type": "product_list",
        "position": "[0,72,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "_204",
        "type": "post_atc_layout",
        "position": "[0,74,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      },
      {
        "name": "_205",
        "type": "post_atc_layout_variant",
        "position": "[0,75,1,1]",
        "data": [],
        "__typename": "pdpComponent"
      }
    ]
  }
}
```

### ⭐ **Product Rating:**
Integrate product ratings into your application to build trust. Let users see what others think about a product at a glance, enhancing the credibility of your platform.
```
curl --request GET \
	--url https://tokopedia7.p.rapidapi.com/product/rating/459906908 \
	--header 'X-RapidAPI-Host: tokopedia7.p.rapidapi.com' \
	--header 'X-RapidAPI-Key: SIGN-UP-FOR-KEY'
```
```json
{
  "success": true,
  "message": "success",
  "results": {
    "productID": "459906903",
    "rating": {
      "positivePercentageFmt": "86% pembeli merasa puas",
      "ratingScore": "4.5",
      "totalRating": 1820,
      "totalRatingWithImage": 193,
      "totalRatingTextAndImage": 766,
      "detail": [
        {
          "rate": 5,
          "totalReviews": 1294,
          "formattedTotalReviews": "1.294",
          "percentageFloat": 71.1,
          "__typename": "productrevRatingDetail"
        },
        {
          "rate": 4,
          "totalReviews": 280,
          "formattedTotalReviews": "280",
          "percentageFloat": 15.38,
          "__typename": "productrevRatingDetail"
        },
        {
          "rate": 3,
          "totalReviews": 137,
          "formattedTotalReviews": "137",
          "percentageFloat": 7.53,
          "__typename": "productrevRatingDetail"
        },
        {
          "rate": 2,
          "totalReviews": 47,
          "formattedTotalReviews": "47",
          "percentageFloat": 2.58,
          "__typename": "productrevRatingDetail"
        },
        {
          "rate": 1,
          "totalReviews": 62,
          "formattedTotalReviews": "62",
          "percentageFloat": 3.41,
          "__typename": "productrevRatingDetail"
        }
      ],
      "__typename": "productrevProductRating"
    },
    "topics": [
      {
        "rating": 4.150000095367432,
        "ratingFmt": "4,0",
        "formatted": "Kualitas Barang",
        "key": "kualitas",
        "reviewCount": 422,
        "reviewCountFmt": "422",
        "show": false,
        "__typename": "topicAggs"
      },
      {
        "rating": 4.300000190734863,
        "ratingFmt": "4,0",
        "formatted": "Harga Barang",
        "key": "harga",
        "reviewCount": 128,
        "reviewCountFmt": "128",
        "show": false,
        "__typename": "topicAggs"
      },
      {
        "rating": 4.349999904632568,
        "ratingFmt": "4,0",
        "formatted": "Pengiriman",
        "key": "pengiriman",
        "reviewCount": 87,
        "reviewCountFmt": "87",
        "show": false,
        "__typename": "topicAggs"
      },
      {
        "rating": 4,
        "ratingFmt": "4,0",
        "formatted": "Pelayanan Penjual",
        "key": "pelayanan",
        "reviewCount": 79,
        "reviewCountFmt": "79",
        "show": false,
        "__typename": "topicAggs"
      },
      {
        "rating": 4.199999809265137,
        "ratingFmt": "4,0",
        "formatted": "Sesuai Deskripsi",
        "key": "sesuai deskripsi",
        "reviewCount": 69,
        "reviewCountFmt": "69",
        "show": false,
        "__typename": "topicAggs"
      },
      {
        "rating": 4.300000190734863,
        "ratingFmt": "4,0",
        "formatted": "Kemasan Barang",
        "key": "kemasan",
        "reviewCount": 47,
        "reviewCountFmt": "47",
        "show": false,
        "__typename": "topicAggs"
      }
    ],
    "availableFilters": {
      "withAttachment": true,
      "rating": true,
      "topics": true,
      "helpfulness": true,
      "__typename": "availableFiltersHeader"
    },
    "__typename": "productrevRatingAndTopics"
  }
}
```

### 📝 **Product Reviews:**
Foster a community by incorporating product reviews. Allow users to share their experiences and insights, creating a vibrant and engaged user base.
```
curl --request GET \
	--url https://tokopedia7.p.rapidapi.com/product/reviews/459906908 \
	--header 'X-RapidAPI-Host: tokopedia7.p.rapidapi.com' \
	--header 'X-RapidAPI-Key: SIGN-UP-FOR-KEY'
```
```json
{
  "success": true,
  "message": "success",
  "results": {
    "productID": "459906903",
    "list": [
      {
        "id": "981956664",
        "variantName": "Merah",
        "message": "oke kak",
        "productRating": 4,
        "reviewCreateTime": "1703769969",
        "reviewCreateTimestamp": "4 hari lalu",
        "isReportable": false,
        "isAnonymous": true,
        "imageAttachments": [],
        "videoAttachments": [],
        "reviewResponse": {
          "message": "Terima kasih telah berbelanja di LIGER OFFICIAL STORE. Bagikan link toko kami https://www.tokopedia.com/liger-official kepada teman-teman Anda dan favoritkan Toko kami untuk terus update mengenai stok dan produk terbaru",
          "createTime": "4 hari lalu",
          "__typename": "reviewReviewResponsePDPType"
        },
        "user": {
          "userID": "0",
          "fullName": "R***t",
          "image": "https://images.tokopedia.net/img/cache/100-square/default_v3-usrnophoto.png",
          "url": "",
          "__typename": "reviewReviewUserPDPType"
        },
        "likeDislike": {
          "totalLike": 0,
          "likeStatus": 0,
          "__typename": "reviewLikeDislikePDPType"
        },
        "stats": [],
        "badRatingReasonFmt": "",
        "__typename": "reviewListPDPType"
      },
      ...
    ],
    "shop": {
      "shopID": "5463752",
      "name": "LIGER OFFICIAL STORE",
      "url": "https://www.tokopedia.com/liger-official",
      "image": "https://images.tokopedia.net/img/cache/215-square/shops-1/2019/2/28/5463752/5463752_6db9c54d-440e-4a10-a916-268f6a16d120.png",
      "__typename": "reviewShopPDPType"
    },
    "hasNext": true,
    "totalReviews": 766,
    "__typename": "productrevGetProductReviewListType"
  }
}
```

### 🚀 **Why Choose Tokopedia API?**
- **Cutting-Edge Technology:** Stay ahead with the latest e-commerce innovations.
- **User-Centric Design:** Enhance user experience with seamless and intuitive features.
- **Reliable Data:** Access real-time, accurate, and reliable data from Tokopedia's extensive marketplace.

### 🌟 **Get Started Today!**
Transform your digital storefront with the power of Tokopedia API. Join the e-commerce revolution and provide your users with an unparalleled shopping experience.

Get Your API key here: [TOKOPEDIA API](https://rapidapi.com/ptwebsolution/api/tokopedia7)
