## LiquidM Universal Pixel for Google Tag Manager

This Pixel allows you to attribute conversions to campaigns and ads, run CPC+ campaigns and build audiences for retargeting. 
  
### CPC+ campaigns

CPC+ campaigns are based on Complete View events. In order to track them add LiquidM Universal Pixel with the type `CPC+ Complete View Tracking` to all your landing pages. Please refer to LiquidM Platform Guide or https://liquidm.com/cpc-plus/ for further information.

### Conversion Tracking

Two attribution models are available for conversion tracking - one is based on campaign/account and the other is based on click token. 
- Campaign/account model uses 3rd-party cookie to attribute a conversion to the last ad (impression) which was shown to the user. For this option add LiquidM Universal Pixel with the type `Conversion Tracking` and set campaign or account ID to the pages where the conversion happens (e.g. checkout page).
- Click token model is more precise and requires two pixels to be implemented. For the first step add LiquidM Universal Pixel with the pixel type `Conversion Tracking` and attribution type `Deferred Tracking (1st party cookies)` to all your pages. Then add Pixel with the pixel type `Conversion Tracking` and attribution type `Click token` to the page where the conversion happens (e.g. checkout page). 

Please refer to the LiquidM Platform Guide in your account for further information, use case examples, the description of the attribution models and limitations of each attribution type.

### Retargeting segments

In order to retarget user who have visited your site or have converted (e.g. visited checkout page) add LiquidM Universal Pixel with the pixel type `Retargeting segments` and set Segment Token. Select the same segment in the Targeting section of your ad to retarget or exclude the audience. Please refer to the LiquidM Platform Guide for further information about retargeting.
