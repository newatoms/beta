# Web scraper

This scraper can extract information from multiple targeted linkedIn profiles.
Want to know how to use it and how it works? Go to the [Web Scraping guide](../guides/web-scraping/readme.md).

```javascript
var profiles = [
    'https://nl.linkedin.com/in/sam-prinssen-6a101522',
    'https://nl.linkedin.com/in/thomas-de-beus-a76184b0',
    'https://nl.linkedin.com/in/matthijs-mentink-1ba4651a'
  ]

var x = new require('x-ray')()

for (var i = 0; i < profiles.length; i++) {
  var profile = profiles[i]

x(
  profile,
    {
      work: x(
        '.position',
        [ {
          title: '.item-title',
          organisation: '.item-subtitle',
          time: '.date-range'
        } ]
      ),
      school: x(
        '.school',
        [ {
          school: '.item-title',
          type: '.item-subtitle',
          time: '.date-range'
        } ]
      )
    }
  ).write(profile.replace(/\//gi, '-') + '.json')
}
```
