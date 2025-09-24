# adverts
tutorial
The main file where the data comes from is the index.json file here. The images must be located in the images/ folder, and they CANNOT be in subfolders. This structure must always be this way.

## the index.json file
Youll notice the file has this structure:
[
   {
      "id": 1,
      "image": "Checks- Small Cert.jpg",
      "title": "Build trust with certification",
      "description": "Become a certified partner, get free premium, and more.",
      "actionText": null,
      "url": "https://kitlegit.com/app-certification/",
      "forFreeUsersOnly": false,
      "disableDate": null,
      "promoCode": null,
      "type": "HOME_PAGE_SMALL",
      "actionType": "LINK_TO_WEBVIEW"
    },

    ..... 
]

If anything changes about the structure, nothing will load on the app.
You can add as many ADVERT objects as you want, or delete them. The Advert obj is each piece of data between {}, like this one:
 {
    "id": 1,
    "image": "Checks- Small Cert.jpg",
    "title": "Build trust with certification",
    "description": "Become a certified partner, get free premium, and more.",
    "actionText": null,
    "url": "https://kitlegit.com/app-certification/",
    "forFreeUsersOnly": false,
    "disableDate": null,
    "promoCode": null,
    "type": "HOME_PAGE_SMALL",
    "actionType": "LINK_TO_WEBVIEW"
}


These objects are separates by comma "," and the last one in the file CANNOT have a comma (as its the last one).

So the finla index.json file will be something like this: 
[  {ADV},  {ADV},  {ADV}, {ADV}, ....., {ADV}  ] 

### the index.json important attributes
This explains each attribut of the object ADVERT. Remeber: keep quote marks where they are at now, and dont put them where they are not. 

{
    "id": 14, // internal only, but each ADVERT obj must have a unique id (regardless of the order)
    "image": "Home + Result Large - BF.jpg", // reference to the added image. The must match the exact images name thats added in the images folder.
    "title": null, // you write, in quotes "Title of the image" or null with no quotes
    "description": null, // you write, in quotes "Description of the image" or null with no quotes
    "actionText": "Get Premium", // you write (the text of the button)
    "url": null, // if this leads to a webpage, the link goes here, in quotes
    "forFreeUsersOnly": true, // true or false, no quotes
    "disableDate": null, // not used anymore
    "promoCode": null, // not used anymore
    "type": "RESULTS_PAGE_LARGE", // format of the banner. The options are   HOME_PAGE_SMALL, HOME_PAGE_LARGE, MY_CHECKS_SMALL, RESULTS_PAGE_LARGE 
    "actionType": "LINK_TO_PLANS_PAGE" // what the buttons does, the options are   LINK_TO_WEBVIEW, TRIGGER_POP_UP_QUERY, LINK_TO_PLANS_PAGE, LINK_EXTERNAL 
  }

