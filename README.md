# Schaliegasvrij

* [Status](#status)
* [Setting Up](#setting-up)
* [Data](#data)
  + [site.json](#site.json)
  + [Index.json](#index.json)
  + [Pages.json](#pages.json)
* [Forms](#forms)

## Status

| | |
| --- | --- |
| __Huidige versie__ | 1.0 |
| __Readme updated__ | 9 August 2019

## Setting Up

`npm install` 
`npm run start` 
or `npm run prod` if you have access to live data

## Data

### Site.json

``` json
{
  "title": "Schaliegasvrij",
  "description": "Voor een duurzame haven, zonder schaliegas, zonder wegwerpplastic, met een echte toekomst.",
  "url": "http://www.schaliegasvrij.be",
  "logo": "https://www.logo.be",
  "footerTitle": "Antwerpen Schaliegasvrij",
  "footerContent": "(cc)2018",
  "footerLinks": [
    {
      "type": "facebook",
      "content": "https://www.facebook.com/Antwerpen-Schaliegasvrij-346826892611242/"
    }
  ]
}
```

### Index.json

The home-page uses a slightly different layout than all other pages (layout/home.html), and gives the option to include an images-mosaic:

``` json
[
  {
    "content": "Homepage Content",
    "images": [
      {
        "url": "https://firstimage.be"
      }
    ]
  }
]
```

### Pages.json

Pages use the default layout, and need the following elements:

``` json
[
  {
    "file": "index",
    "category": "over-ons",
    "categoryName": "Over ons",
    "menuTitle": "Over Ons",
    "content": [
      {
        "text": "Over ons: eerste paragraaf",
        "textFirst": true,
        "image": "https://eerste_afbeelding.be",
        "imgAlt": "alt"
      },
      {
        "text": "Tweede paragraaf",
        "image": "https://tweede_afbeelding.be"
      }
    ]
  }
]
```

Content is a selection of paragraphs accompanied by an optional image. If no images are provided, the text will take up the full width of the container; otherwise it will take up half of its container, with the image filling the other half. The layout will automatically alternate the order of a paragraph-image pair.

### Forms

```json
```
