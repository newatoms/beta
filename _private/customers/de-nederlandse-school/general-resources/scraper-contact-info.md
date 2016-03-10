# Contact info scraper

This code will scrape all contact info from the /wie-zijn-wij/ url.

```javascript
var x = new require('x-ray')()

  x(
    'http://www.denederlandseschool.nl/wie-zijn-wij/',
    {
      contacts: x(
        '.item-inner',
        [ {
          category: '.category',
          name: '.title',
          occupation: '.occupation',
          moreInfo: 'a@href'
        } ]
      ),
    }
  ).write('results.json')
  ```
