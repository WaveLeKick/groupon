[Groupon](https://apify.com/lexis-solutions/groupon?fpr=data)

# 📦 Groupon Scraper

![Groupon Scraper](https://images.apifyusercontent.com/bYF0C7eY43KU66BkzK71MO-l8KtjrnmSMyELsuAT2Es/w:1800/cb:1/aHR0cHM6Ly9pLmliYi5jby8zOU5OM1l6Mi9ncm91cG9uLWNvdmVyLnBuZw.webp)

This actor is designed to scrape deals, listings, and local offers from [Groupon.com](https://www.groupon.com/), one of the most popular discount marketplaces in the world. Whether you're interested in specific products, categories, or individual deal pages, this scraper helps you extract structured data for deeper analysis and integration.

---

## 🚀 Key Features

- ✅ Scrapes Groupon search results and local listings
- ✅ Supports full deal detail page scraping
- ✅ Simple input structure with customizable start URLs
- ✅ Optional limit on number of items to scrape
- ✅ Proxy support for geo-specific scraping

---

## 👤 Who Is This Actor For?

This actor is ideal for:

- **Market researchers** collecting price and offer data
- **Local business analysts** monitoring deals in specific categories or cities
- **Affiliate marketers** tracking current promotions
- **Developers** building applications using Groupon’s publicly available data
- **SEO professionals** analyzing content and deal visibility

---

## ❓ Why Is This Actor Important?

Groupon provides vast local and product-based deal information that is often only accessible via client-side rendering and complex navigation. This actor:

- Automates navigation and deal extraction across search, category, and individual pages.
- Helps you bypass manual data collection by scraping structured deal data.
- Is highly flexible — simply change the start URLs to target a different query or category.

---

## Input Schema

Here’s an example input:

```
{
  "startUrls": [
    {
      "url": "https://www.groupon.com/search?query=oil"
    },
    {
      "url": "https://www.groupon.com/local/beauty-and-spas"
    },
    {
      "url": "https://www.groupon.com/deals/n-blooms-today-25"
    }
  ],
  "maxItems": 10,
  "proxyConfiguration": {
    "useApifyProxy": false
  }
}
```

## Output Schema

```
{
  "id": "sev-laser-chicago",
  "uuid": "181994d1-1adc-425a-85c9-e4801308fbde",
  "title": "Say Goodbye to Unwanted Hair! 6 Laser Sessions at SEV Laser Chicago (Up to 56% Off)",
  "subtitle": "",
  "seoTitle": "SEV Laser Chicago - From $97.20 - Chicago | Groupon",
  "url": "https://www.groupon.com/deals/sev-laser-chicago",
  "status": "BUY",
  "mainDealType": "local",
  "overlayDetails": {
    // null in most cases
    "title": "Valid Treatment Areas",
    // null in most cases
    "detailsHtml": "<h5>Small Treatment Areas</h5>\n<ul>\n<li>Unibrow</li>\n<li>Upper lip</li>\n<li>Ears</li>\n<li>Chin</li>\n<li>Nose/Nostrils</li>\n</ul>\n<h5>Medium Treatment Areas</h5>\n<ul>\n<li>Bikini Line</li>\n<li>Underarms</li>\n<li>Neck (front or back)</li>\n</ul>\n<h5>Large Treatment Areas:</h5>\n<ul>\n<li>Full Bikini (Brazilian)</li>\n<li>Half Back (upper or lower)</li>\n<li>Chest</li>\n<li>Half Legs (upper or lower)</li>\n</ul>\n<h5>Extra Large Treatment Areas:</h5>\n<ul>\n<li>Full Bikini (Brazilian) and Underarms</li>\n<li>Face and Neck (front or back)</li>\n<li>Full Arms</li>\n</ul>"
  },
  "flags": {
    "__typename": "DealFlags",
    "isGoodsDeal": false,
    "isGiftable": true,
    "isTravelDeal": false,
    "isGetawaysDeal": false,
    "isGetawaysBookableDeal": false,
    "isCoupon": false,
    "isClo": false,
    "isG1G2": true,
    "isGlive": false,
    "is3Pip": false,
    "isHotelDeal": false,
    "isGrouponGiftCard": false,
    "isUITreatmentEmpty": false,
    "isMerchantNameInTitle": false,
    "isBookable": false,
    "hasPromotion": true,
    "hidePrice": false,
    "hideReviews": false,
    "hasTimer": false,
    "discountEnabled": true,
    "showRedemptionLocations": true,
    "showPrice": true
  },
  "aboutDealHtml": "<p><br><center><img loading=\"lazy\" src=\"https://sdn.signalhire.co/storage/company/0910/c815/e70d/914f/94d8/b6ac/8318/e948.webp\" alt=\"\" width=\"200\" style=\"max-width: 100%\"></center><br></p>\n<p>Are you tired of the constant hassle of shaving or waxing? Say goodbye to unwanted hair and hello to smooth, silky skin with this exclusive laser hair removal offer!</p>\n<h4><p style=\"color:#A69788\">About Laser Hair Removal</p></h4>    \n<p>Embark on a journey towards flawless skin with laser hair removal sessions. Experience the power of Candela and Cynosure lasers, meticulously designed for optimal hair removal results. </p>\n<p>Learn more about the type of lasers used:</p>\n<ul>\n<li>\n<p>Candela lasers combine the Yag 1064 and Alexandrite 755nm wavelengths for optimal hair removal results.</p>\n</li>\n<li>\n<p>Cynosure combines the laser technology of Alexandrite and the Yag; the dual laser application allows for more precision when targeting the bulge, bulb, and papilla of the hair follicle for more effective hair removal on most skin types, including light, dark, and most hair colors. For additional information <a href=\"https://candelamedical.com/na/science/gentle-laser-technology\">click here</a>. </p>\n</li>\n</ul>\n<h4><p style=\"color:#A69788\">Valid Treatment Areas</p></h4>\n<ul>\n<li>\n<p><strong>Small Treatment Areas</strong>: Unibrow | Upper lip | Ears | Chin | Nose/Nostrils<br></p>\n</li>\n<li>\n<p><strong>Medium Treatment Areas</strong>: Bikini Line | Underarms | Neck (front or back) <br></p>\n</li>\n<li>\n<p><strong>Large Treatment Areas</strong>: Full Bikini (Brazilian) | Half Back (upper or lower) | Chest | Half Legs (upper or lower) <br></p>\n</li>\n<li>\n<p><strong>Extra - Large Treatment Areas</strong>: Full Bikini (Brazilian) and Underarms | Face and Neck (front or back) | Full Arms <br></p>\n</li>\n<li>\n<p><strong><a href=\"#details\">View All Valid Treatment Areas</a></strong></p>\n</li>\n</ul>\n<h4><p style=\"color:#A69788\">Before You Go</p></h4>   \n<ul>\n<li>\n<p>Treatment areas cannot be altered or substituted under any circumstances</p>\n</li>\n<li>\n<p>This offer is only valid for listed location</p>\n</li>\n</ul>\n<center><br><img loading=\"lazy\" src=\"https://sevlaser.com/wp-content/uploads/2023/07/polaroid-location-lhr.avif\" alt=\"\" width=\"250\" style=\"max-width: 100%\"><br></center>\n<h4><p style=\"color:#A69788\">Discover the SEV Difference</p></h4>         \n<p><strong>Celebrity-Favorite Spa Salon:</strong> Step into the realm of Hollywood's elite and indulge in treatments favored by your favorite stars.<br></p>\n<p><strong>Safe for All Skin Tones:</strong> Whether your skin tone is light or dark, the laser technologies cater to all, delivering effective treatments with unmatched precision. Also, the inclusive approach ensures that everyone feels valued and receives great care. </p>\n<p>Don't let unwanted hair hold you back. Visit SEV Laser and embrace a future of smooth, hair-free skin.    </p>\n<p>SEV Laser <strong>prioritizes your safety and satisfaction</strong> above all else. Their medical accreditation provides adherence to stringent quality and safety standards, offering you peace of mind during your treatments. With a stellar <strong>5-star rating on Groupon</strong>, their commitment to excellence speaks volumes. </p>\n<p>Beyond just treatments, they provide <strong>comprehensive aftercare guidance</strong> to ensure your comfort and maximize results. With SEV, you're not merely undergoing a procedure—you're investing in confidence and liberation from unwanted hair.</p>\n<p>Don't let unwanted hair hold you back. Visit SEV Laser and embrace a future of smooth, hair-free skin.</p>",
  "finePrintHtml": "\n    Promotional value expires 120 days after purchase. Amount paid never expires.    \n    <br>\n<p><b>Booking:</b></p>\n<li>Appointment Required. </li>\n<li>A credit card is required at the time of booking the first appointment. </li>\n<li>Valid only at listed location.</li>\n\n<p><b>Eligibility Requirements:</b></p>\n<li>All clients are required to complete a consultation (if applicable) and paperwork provided by SEV prior to treatment. </li>\n<li>Must be 14 years and older to receive treatment. </li>\n<li>Younger than 18 years of age, must have guardian-signed waivers and guardian must accompany to first appointment. </li>\n\n<p><b>Restrictions: </b></p>\n<li>Limit 1 Groupon redemption per person, across all SEV locations.</li>\n<li>Additional vouchers will not be honored, including vouchers received as a gift. </li>\n<li>You may purchase up to 3 additional vouchers as gift(s) only, however if the gift receiver has already used a voucher, the gifted voucher will not be honored. </li>\n<li><a href=\"https://www.groupon.com/deals/sev-laser-chicago/special_content?redirect=false\">Treatment areas</a> cannot be altered or substituted under any circumstances. </li>\n<li>All treatment areas must be booked and treated together during all sessions.</li>\n<li>Transferring sessions to another individual is not permitted.</li>\n\n<p><b>Cancellation & Refund Policy: </b></p>\n<li>First appointment must be booked within 60 days of purchase date.</li>\n<li>Treatment packages expire 1 year from the activation date.</li>\n<li>48 hours. All SEV cancellations and policies</a> apply. </li>\n<li>Refund requests will only be honored prior to any treatment received. </li>\n<li>Refunds will be processed by Groupon directly. </li>\n<li>Consultation required, non candidates and other refund requests will be honored before the service provided.</li>\n<br> \n    Merchant is solely responsible to purchasers for the care and quality of the advertised goods and services.\n    Learn about <a href=\"https://www.groupon.com/legal/pricing-transparency\">Strike-Through Pricing and Savings</a>\n  ",
  "highlightsHtml": "<p>Qualified and skilled technician uses the Candela and Cynosure laser to gently remove unwanted hair from the chosen body area</p>",
  "categorizations": [
    {
      "__typename": "Categorizations",
      "id": "local",
      "children": [
        {
          "__typename": "Categorizations",
          "id": "beauty-and-spas",
          "children": [
            {
              "__typename": "Categorizations",
              "id": "hair-removal",
              "children": [
                {
                  "__typename": "Categorizations",
                  "id": "laser-hair-removal",
                  "children": []
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "merchant": {
    "__typename": "Merchant",
    "id": "sev-laser-chicago",
    "uuid": "6ba100e6-44e3-4745-875a-1c06b5bb44b5",
    "aboutHtml": "<p>SEV Laser is a celebrity-favorited medical spa specialized in laser hair removal. Notable customers are, among others, the Kardashian sisters, Vanessa Hudgens, Golden Barbie, and Ashley Tisdale. The clinic's effects are also thoroughly admired on the internet—SEV is followed by over 250,000 Instagramers. High-quality lasers are used not only for permanent hair removal, but also for skin rejuvenation and tightening. Other services, such as non-invasive face and body sculpting, eyelash extensions, or eyebrow shaping are also on offer.</p>",
    "brandSlug": "sev-laser",
    "name": "SEV Laser Chicago",
    "recommendations": [
      {
        "__typename": "MerchantRecommendation",
        "rating": 4.89,
        "totalMessage": "379",
        "total": 379
      }
    ],
    "websiteUrl": "https://sevlaser.com/chicago/"
  },
  "grouponRating": "4.9",
  "soldQuantityMessage": "5,000+",
  "endsIn": "2046-02-05T05:59:59Z",
  "division": {
    "__typename": "Division",
    "id": "chicago",
    "timezoneIdentifier": "America/Chicago",
    "timezoneOffsetInSeconds": -18000
  },
  "primaryImageUrl": "https://img.grouponcdn.com/deal/qYAv6HJxJ6msmA6vqfnsasatUTg/qY-700x420/v1/t600x362.webp",
  "images": [
    "https://img.grouponcdn.com/deal/qYAv6HJxJ6msmA6vqfnsasatUTg/qY-700x420/v1/t600x362.webp",
    "https://img.grouponcdn.com/deal/3QFqeoL98s2wZ6nUXep6La7hNVcb/3Q-700x420/v1/t600x362.webp",
    "https://img.grouponcdn.com/deal/3zwK2dtCERoeja7Yvy1Umhw7F3wN/3z-700x420/v1/t600x362.webp",
    "https://img.grouponcdn.com/deal/1RrenY7HaYfBypEshXiPdNKfXPF/1R-700x420/v1/t600x362.webp",
    "https://img.grouponcdn.com/deal/3PPsXb5F2ZeyPqsptZeGDRUpKLCa/3P-700x420/v1/t600x362.webp",
    "https://img.grouponcdn.com/deal/JNz1zUWRAfmBVeiEVj5PiWUQnYq/JN-700x420/v1/t600x362.webp",
    "https://img.grouponcdn.com/deal/3X521oGsj2f2WgK8bpJt27f2eYqc/3X-700x420/v1/t600x362.webp",
    "https://img.grouponcdn.com/deal/3HFRzGC3gbrjofZKzg3g8CaoM197/3H-700x420/v1/t600x362.webp"
  ],
  "videos": [
    {
      "__typename": "DealVideo",
      "youtubeId": "XtjhDVChiUw",
      "thumbnailUrl": "https://img.youtube.com/vi/XtjhDVChiUw/hqdefault.jpg",
      "url": "https://www.youtube.com/embed/XtjhDVChiUw"
    }
  ],
  "reels": [],
  "badges": [
    {
      "__typename": "Badge",
      "badgeType": "BEST_RATED",
      "text": "Best Rated",
      "iconUrl": null
    },
    {
      "__typename": "Badge",
      "badgeType": "BOUGHT_5000",
      "text": "5,000+ Bought",
      "iconUrl": null
    },
    {
      "__typename": "Badge",
      "badgeType": "URGENCY_MESSAGE",
      "text": "Selling fast!",
      "iconUrl": "https://img.grouponcdn.com/ums/4YgzH3Csf5WxLLjeijjsvN4zrkyx/icon-fire-54x54-54x54"
    }
  ],
  "options": [
    {
      "__typename": "DealOption",
      "id": "9ae55d64-04f7-4e62-9ebc-8443a35dcb88",
      "uuid": "9ae55d64-04f7-4e62-9ebc-8443a35dcb88",
      "title": "Six Laser Hair-Removal Sessions on One Small Area - Valid Only at Chicago",
      "expiresAt": "2025-10-03T00:00:00Z",
      "optionStatus": "BUY",
      "isSoldOut": false,
      "soldQuantityMessage": "720+",
      "discount": "-46%",
      "discountExperiment": "46",
      "includedFees": null,
      "specialMessageOption": {
        "__typename": "SpecialMessageOption",
        "message": null,
        "isNegative": false,
        "isPositive": false
      },
      "booking": {
        "__typename": "DealOptionBooking",
        "isPrePurchaseBookable": false,
        "agendas": [],
        "bookingType": null,
        "componentFlow": null
      },
      "buyUrl": "https://www.groupon.com/deals/sev-laser-chicago/confirmation?pledge_id=9ae55d64-04f7-4e62-9ebc-8443a35dcb88",
      "maximumPurchaseQuantity": 4,
      "minimumPurchaseQuantity": 1,
      "allowedQuantities": [1, 2, 3, 4],
      "actions": [
        {
          "__typename": "Action",
          "actionType": "BUY_NOW",
          "status": "BUY",
          "url": "https://www.groupon.com/deals/sev-laser-chicago/confirmation?pledge_id=9ae55d64-04f7-4e62-9ebc-8443a35dcb88"
        },
        {
          "__typename": "Action",
          "actionType": "ADD_TO_CART",
          "status": "BUY",
          "url": "https://www.groupon.com/deals/sev-laser-chicago/confirmation?pledge_id=9ae55d64-04f7-4e62-9ebc-8443a35dcb88"
        }
      ],
      "consumerContractTerms": [
        {
          "__ref": "ConsumerContractTerms:additional-info"
        }
      ],
      "isStartingPrice": false,
      "strikeThroughPrice": [
        {
          "__typename": "FormattedPriceItem",
          "alignTop": false,
          "value": "$",
          "strikeThrough": true,
          "small": false,
          "bold": false,
          "hideable": false
        },
        {
          "__typename": "FormattedPriceItem",
          "alignTop": false,
          "value": "180",
          "strikeThrough": true,
          "small": false,
          "bold": false,
          "hideable": false
        }
      ],
      "price": [
        {
          "__typename": "FormattedPriceItem",
          "alignTop": false,
          "value": "$",
          "strikeThrough": true,
          "small": false,
          "bold": true,
          "hideable": false
        },
        {
          "__typename": "FormattedPriceItem",
          "alignTop": false,
          "value": "108",
          "strikeThrough": true,
          "small": false,
          "bold": true,
          "hideable": false
        }
      ],
      "unformattedPrice": {
        "__typename": "Price",
        "amount": 10800,
        "currencyCode": "USD",
        "currencyExponent": 2,
        "suffix": null
      },
      "limitedSale": {
        "__typename": "LimitedSale",
        "isLimitedSale": true,
        "endsAt": "2025-06-07T06:59:10Z",
        "limitedSaleOffer": {
          "__typename": "LimitedSaleOffer",
          "relativeOfferLabel": "Extra $10.80 off, ends tomorrow",
          "offerLabel": "Extra $10.80 Off Ends 6/6",
          "rawOfferPrice": 9720,
          "offerPrice": [
            {
              "__typename": "FormattedPriceItem",
              "alignTop": false,
              "value": "$",
              "strikeThrough": false,
              "small": false,
              "bold": true,
              "hideable": false
            },
            {
              "__typename": "FormattedPriceItem",
              "alignTop": false,
              "value": "97",
              "strikeThrough": false,
              "small": false,
              "bold": true,
              "hideable": false
            },
            {
              "__typename": "FormattedPriceItem",
              "alignTop": false,
              "value": ".",
              "strikeThrough": false,
              "small": false,
              "bold": true,
              "hideable": false
            },
            {
              "__typename": "FormattedPriceItem",
              "alignTop": false,
              "value": "20",
              "strikeThrough": false,
              "small": false,
              "bold": true,
              "hideable": false
            }
          ]
        }
      },
      "promotion": {
        "__typename": "Promotion",
        "message": "Extra $9.72 off",
        "endsAt": "6/6",
        "promoEndTimeStamp": "2025-06-06T23:59:00-07:00",
        "event": "referenceId:145678,eventName:,dealId:181994d1-1adc-425a-85c9-e4801308fbde,inventoryProductId:43350d2b-9811-4eff-ad84-d3bba9685c66,discountAmount:9,discountCeiling:",
        "promocode": "DAD25",
        "formattedFinalPrice": [
          {
            "__typename": "FormattedPriceItem",
            "alignTop": false,
            "value": "$",
            "strikeThrough": false,
            "small": false,
            "bold": true,
            "hideable": false
          },
          {
            "__typename": "FormattedPriceItem",
            "alignTop": false,
            "value": "87",
            "strikeThrough": false,
            "small": false,
            "bold": true,
            "hideable": false
          },
          {
            "__typename": "FormattedPriceItem",
            "alignTop": false,
            "value": ".",
            "strikeThrough": false,
            "small": false,
            "bold": true,
            "hideable": false
          },
          {
            "__typename": "FormattedPriceItem",
            "alignTop": false,
            "value": "48",
            "strikeThrough": false,
            "small": false,
            "bold": true,
            "hideable": false
          }
        ],
        "price": {
          "__typename": "Price",
          "amount": 8748,
          "currencyCode": "USD",
          "currencyExponent": 2,
          "suffix": null
        }
      },
      "traits": [],
      "gallery": null,
      "warranties": [],
      "redemptionLocations": [
        {
          "__typename": "DealRedemptionLocation",
          "uuid": "c8dee5c1-2a2e-b1fa-d5e8-017c27a7e253",
          "city": "Chicago",
          "country": "US",
          "state": "IL",
          "streetAddress1": "2320 North Lincoln Avenue"
        }
      ],
      "specificAttributes": {
        "__typename": "DealOptionSpecificAttributes",
        "description": null,
        "priceQualifier": null
      },
      "shippingCharge": null,
      "shippingOptions": [],
      "inventoryProductId": "43350d2b-9811-4eff-ad84-d3bba9685c66",
      "images": [],
      "encodedDealOptionPromoData": "eyJpZCI6IjQzMzUwZDJiLTk4MTEtNGVmZi1hZDg0LWQzYmJhOTY4NWM2NiIsImlzaWQiOiJ2aXMiLCJidXllck1pblF1YW50aXR5IjoxLCJwcm9ncmFtVHlwZSI6IlNBTEUiLCJwcmljZVN1bW1hcnkiOnsicHJpY2UiOnsiYW1vdW50IjoxMDgwMCwiY3VycmVuY3lDb2RlIjoiVVNEIn19LCJyZWZlcmVuY2VQcmljZSI6eyJhbW91bnQiOjk3MjAsImN1cnJlbmN5Q29kZSI6IlVTRCJ9fQ=="
    },
    {
      "__typename": "DealOption",
      "id": "586e89fa-0da2-4adc-abf1-fc72a4c67148",
      "uuid": "586e89fa-0da2-4adc-abf1-fc72a4c67148",
      "title": "Six Laser Hair-Removal Sessions on One Medium Area - Valid Only at Chicago",
      "expiresAt": "2025-10-03T00:00:00Z",
      "optionStatus": "BUY",
      "isSoldOut": false,
      "soldQuantityMessage": "1,000+",
      "discount": "-42%",
      "discountExperiment": "42",
      "includedFees": null,
      "specialMessageOption": {
        "__typename": "SpecialMessageOption",
        "message": null,
        "isNegative": false,
        "isPositive": false
      },
      "booking": {
        "__typename": "DealOptionBooking",
        "isPrePurchaseBookable": false,
        "agendas": [],
        "bookingType": null,
        "componentFlow": null
      },
      "buyUrl": "https://www.groupon.com/deals/sev-laser-chicago/confirmation?pledge_id=586e89fa-0da2-4adc-abf1-fc72a4c67148",
      "maximumPurchaseQuantity": 4,
      "minimumPurchaseQuantity": 1,
      "allowedQuantities": [1, 2, 3, 4],
      "actions": [
        {
          "__typename": "Action",
          "actionType": "BUY_NOW",
          "status": "BUY",
          "url": "https://www.groupon.com/deals/sev-laser-chicago/confirmation?pledge_id=586e89fa-0da2-4adc-abf1-fc72a4c67148"
        },
        {
          "__typename": "Action",
          "actionType": "ADD_TO_CART",
          "status": "BUY",
          "url": "https://www.groupon.com/deals/sev-laser-chicago/confirmation?pledge_id=586e89fa-0da2-4adc-abf1-fc72a4c67148"
        }
      ],
      "consumerContractTerms": [
        {
          "__ref": "ConsumerContractTerms:additional-info"
        }
      ],
      "isStartingPrice": false,
      "strikeThroughPrice": [
        {
          "__typename": "FormattedPriceItem",
          "alignTop": false,
          "value": "$",
          "strikeThrough": true,
          "small": false,
          "bold": false,
          "hideable": false
        },
        {
          "__typename": "FormattedPriceItem",
          "alignTop": false,
          "value": "300",
          "strikeThrough": true,
          "small": false,
          "bold": false,
          "hideable": false
        }
      ],
      "price": [
        {
          "__typename": "FormattedPriceItem",
          "alignTop": false,
          "value": "$",
          "strikeThrough": false,
          "small": false,
          "bold": true,
          "hideable": false
        },
        {
          "__typename": "FormattedPriceItem",
          "alignTop": false,
          "value": "174",
          "strikeThrough": false,
          "small": false,
          "bold": true,
          "hideable": false
        },
        {
          "__typename": "FormattedPriceItem",
          "alignTop": false,
          "value": ".",
          "strikeThrough": false,
          "small": false,
          "bold": true,
          "hideable": false
        },
        {
          "__typename": "FormattedPriceItem",
          "alignTop": false,
          "value": "99",
          "strikeThrough": false,
          "small": false,
          "bold": true,
          "hideable": false
        }
      ],
      "unformattedPrice": {
        "__typename": "Price",
        "amount": 17499,
        "currencyCode": "USD",
        "currencyExponent": 2,
        "suffix": null
      },
      "limitedSale": {
        "__typename": "LimitedSale",
        "isLimitedSale": false,
        "endsAt": null,
        "limitedSaleOffer": null
      },
      "promotion": {
        "__typename": "Promotion",
        "message": "Extra $29 off",
        "endsAt": "6/6",
        "promoEndTimeStamp": "2025-06-06T23:59:00-07:00",
        "event": "referenceId:145697,eventName:,dealId:181994d1-1adc-425a-85c9-e4801308fbde,inventoryProductId:d26063d0-3291-469b-afd9-49b408a16d0e,discountAmount:29,discountCeiling:",
        "promocode": "DAD25",
        "formattedFinalPrice": [
          {
            "__typename": "FormattedPriceItem",
            "alignTop": false,
            "value": "$",
            "strikeThrough": false,
            "small": false,
            "bold": true,
            "hideable": false
          },
          {
            "__typename": "FormattedPriceItem",
            "alignTop": false,
            "value": "145",
            "strikeThrough": false,
            "small": false,
            "bold": true,
            "hideable": false
          },
          {
            "__typename": "FormattedPriceItem",
            "alignTop": false,
            "value": ".",
            "strikeThrough": false,
            "small": false,
            "bold": true,
            "hideable": false
          },
          {
            "__typename": "FormattedPriceItem",
            "alignTop": false,
            "value": "99",
            "strikeThrough": false,
            "small": false,
            "bold": true,
            "hideable": false
          }
        ],
        "price": {
          "__typename": "Price",
          "amount": 14599,
          "currencyCode": "USD",
          "currencyExponent": 2,
          "suffix": null
        }
      },
      "traits": [],
      "gallery": null,
      "warranties": [],
      "redemptionLocations": [
        {
          "__typename": "DealRedemptionLocation",
          "uuid": "c8dee5c1-2a2e-b1fa-d5e8-017c27a7e253",
          "city": "Chicago",
          "country": "US",
          "state": "IL",
          "streetAddress1": "2320 North Lincoln Avenue"
        }
      ],
      "specificAttributes": {
        "__typename": "DealOptionSpecificAttributes",
        "description": null,
        "priceQualifier": null
      },
      "shippingCharge": null,
      "shippingOptions": [],
      "inventoryProductId": "d26063d0-3291-469b-afd9-49b408a16d0e",
      "images": [],
      "encodedDealOptionPromoData": "eyJpZCI6ImQyNjA2M2QwLTMyOTEtNDY5Yi1hZmQ5LTQ5YjQwOGExNmQwZSIsImlzaWQiOiJ2aXMiLCJidXllck1pblF1YW50aXR5IjoxLCJwcm9ncmFtVHlwZSI6IkRFRkFVTFQiLCJwcmljZVN1bW1hcnkiOnsicHJpY2UiOnsiYW1vdW50IjoxNzQ5OSwiY3VycmVuY3lDb2RlIjoiVVNEIn19LCJyZWZlcmVuY2VQcmljZSI6e319"
    }
  ],
  "customerReviews": [
    {
      "id": "d47d31f2-3981-11f0-abd8-42010ab7ca86",
      "user": {
        "__typename": "CustomerReviewUser",
        "id": "d47a686e-3981-11f0-8cac-42010ab7ca86",
        "name": "Guest",
        "badges": [],
        "ratingCount": 1,
        "reviewCount": 1
      },
      "text": "The service is very professional and the results are guaranteed. Additionally, the attention from all the staff is incredible.",
      "rating": 5,
      "icons": ["Star", "Star", "Star", "Star", "Star"]
    },
    {
      "id": "432bcbca-956a-11ef-bd2a-42010ab7c6ab",
      "user": {
        "__typename": "CustomerReviewUser",
        "id": "dff828a6-22b1-11e9-af0c-a0369f472020",
        "name": "Mandy",
        "badges": ["TOP REVIEWER", "HELPFUL REVIEWER"],
        "ratingCount": 23,
        "reviewCount": 14
      },
      "text": "Very friendly clean place! My laser tech was very nice and explained everything thoroughly!! Laser was quick and painless!",
      "rating": 5,
      "icons": ["Star", "Star", "Star", "Star", "Star"]
    },
    {
      "id": "daed9b64-852a-11ef-ae3a-42010ab7c6a8",
      "user": {
        "__typename": "CustomerReviewUser",
        "id": "dae313f6-852a-11ef-9168-42010ab7c6a8",
        "name": "Alma",
        "badges": [],
        "ratingCount": 1,
        "reviewCount": 1
      },
      "text": "Amazing customer service. The staff was always friendly and made me feel comfortable!",
      "rating": 5,
      "icons": ["Star", "Star", "Star", "Star", "Star"]
    },
    {
      "id": "8db71d46-3bf3-11ef-8190-0200fc3c8c29",
      "user": {
        "__typename": "CustomerReviewUser",
        "id": "e2be61b6-fc0a-11ed-9b23-0200fc3c8c29",
        "name": "Maria",
        "badges": [],
        "ratingCount": 2,
        "reviewCount": 2
      },
      "text": "Amazing experience! It's only my first time, but so far, so good.",
      "rating": 5,
      "icons": ["Star", "Star", "Star", "Star", "Star"]
    },
    {
      "id": "a92a1ef8-1456-11ef-af57-0200fc3c8c29",
      "user": {
        "__typename": "CustomerReviewUser",
        "id": "94f60a0b-1dbd-11e9-af0b-a0369f472020",
        "name": "Danelle",
        "badges": [],
        "ratingCount": 5,
        "reviewCount": 2
      },
      "text": "Excellent place. The staff are very courteous, especially when I need to reschedule when running a little late. Every nurse is professional during each visit. Can't recommend Sev enough!",
      "rating": 5,
      "icons": ["Star", "Star", "Star", "Star", "Star"]
    },
    {
      "id": "adcc634a-11d5-11ef-8590-0200fc3c8c29",
      "user": {
        "__typename": "CustomerReviewUser",
        "id": "521a4188-43d1-11ec-af0e-a0369f472020",
        "name": "Maggie",
        "badges": [],
        "ratingCount": 9,
        "reviewCount": 1
      },
      "text": "Literally amazing !! Took 5 minutes and didn’t even hurt! They even called me a day after to make sure I had a good experience and if I had any questions. 100000% worth",
      "rating": 5,
      "icons": ["Star", "Star", "Star", "Star", "Star"]
    }
  ],
  "shareLinks": [
    {
      "title": "Facebook",
      "url": "https://www.facebook.com/sharer/sharer.php?u=https://www.groupon.com/deals/sev-laser-chicago?utm_campaign=UserReferral&utm_medium=facebook&utm_source=deal_ita"
    },
    {
      "title": "Pinterest",
      "url": "https://www.pinterest.com/pin/create/button/?url=https%3A%2F%2Fwww.groupon.com%2Fdeals%2Fsev-laser-chicago%3Futm_campaign%3DUserReferral%26utm_medium%3Dpinterest%26utm_source%3Ddeal_ita&media=https://img.grouponcdn.com/deal/qYAv6HJxJ6msmA6vqfnsasatUTg/qY-700x420/v1/t600x362.webp&description=Say%20Goodbye%20to%20Unwanted%20Hair!%206%20Laser%20Sessions%20at%20SEV%20Laser%20Chicago%20(Up%20to%2056%25%20Off)"
    },
    {
      "title": "X",
      "url": "https://twitter.com/intent/tweet?url=https%3A%2F%2Fwww.groupon.com%2Fdeals%2Fsev-laser-chicago%3Futm_campaign%3DUserReferral%26utm_medium%3Dtwitter%26utm_source%3Ddeal_ita&text=Say%20Goodbye%20to%20Unwanted%20Hair!%206%20Laser%20Sessions%20at%20SEV%20Laser%20Chicago%20%20-%20Up%20to%2056%25%20Off%20-%20"
    },
    {
      "title": "Email",
      "url": "mailto:?subject=I%20think%20you'd%20like%20this%20deal%3A%20Say%20Goodbye%20to%20Unwanted%20Hair!%206%20Laser%20Sessions%20at%20SEV%20Laser%20Chicago%20(Up%20to%2056%25%20Off)&body=Say%20Goodbye%20to%20Unwanted%20Hair!%206%20Laser%20Sessions%20at%20SEV%20Laser%20Chicago%20(Up%20to%2056%25%20Off)%20https%3A%2F%2Fwww.groupon.com%2Fdeals%2Fsev-laser-chicago%3Futm_campaign%3DUserReferral%26utm_medium%3Demail%26utm_source%3Ddeal_ita"
    }
  ],
  "locations": [
    {
      "__typename": "RedemptionLocation",
      "id": "24290827",
      "lat": 41.924085,
      "lng": -87.647251,
      "state": "IL",
      "country": "US",
      "uuid": "c8dee5c1-2a2e-b1fa-d5e8-017c27a7e253",
      "address": "2320 North Lincoln Avenue, Chicago",
      "streetAddress1": "2320 North Lincoln Avenue",
      "name": "The Lincoln Common",
      "websiteUrl": "https://sevlaser.com/chicago/",
      "directionsUrl": "https://www.google.com/maps/dir/?api=1&destination=41.924085,-87.647251",
      "distance": null,
      "phoneNumber": null,
      "openHours": null,
      "amenities": []
    }
  ],
  "amenities": [
    {
      "__typename": "Amenity",
      "iconUrl": "https://img.grouponcdn.com/sparta/32Sj46mg7VNV5JzPqKn6PEuZLpiY/32-32x32.webp",
      "name": "Good for Groups",
      "available": true
    },
    {
      "__typename": "Amenity",
      "iconUrl": "https://img.grouponcdn.com/sparta/ULgqscfy4yxfsEQYe3CnobL3xyt/UL-32x32.webp",
      "name": "Parking",
      "available": true
    }
  ],
  "traits": [],
  "categoryShortcuts": [
    "Nearby",
    "Beauty & Spas",
    "Waxing",
    "Upper Lip Wax",
    "Bikini Wax",
    "Upper Lip Threading",
    "Electrolysis Hair Removal",
    "Laser Hair Removal",
    "Brazilian Wax",
    "Underarm Wax"
  ],
  "currentCategory": {
    "__typename": "DealCurrentCategory",
    "id": "laser-hair-removal",
    "type": "subcategory2",
    "title": "Laser Hair Removal",
    "url": "/local/laser-hair-removal",
    "topcategory": "local"
  }
}
```

👀 p.s.

Got feedback or need an extension?

Lexis Solutions is a [certified Apify Partner](https://apify.com/partners/find). We can help you with custom solutions or data extraction projects.

Contact us over [Email](mailto:scraping@lexis.solutions) or [LinkedIn](https://www.linkedin.com/company/lexis-solutions)

## Support Our Work 💝

If you're happy with our work and scrapers, you're welcome to leave us a company review [here](https://apify.com/partners/find/lexis-solutions/review) and leave a review for the scrapers you're subscribed to. It will take you less than a minute but it will mean a lot to us!

Image Credit: [https://www.groupon.com](https://www.groupon.com)