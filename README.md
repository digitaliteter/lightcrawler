# lightcrawler
Crawl a website and run it through Google lighthouse


## Introduction
```

npm install --save lightcrawler --g

lightcrawler --url https://atom.io/ --config lightcrawler-config.json

```


## lightcrawler-config.json

```
{
  "extends": "lighthouse:default",
  "settings": {
    "crawler": {
      "maxDepth": 2,
      "maxChromeInstances": 5
    },
    "onlyCategories": [
      "Accessibility",
      "Performance",
      "Best Practices"
    ],
    "onlyAudits": [
      "accesskeys",
      "aria-allowed-attr",
      "external-anchors-use-rel-noopener",
      "geolocation-on-start",
      "no-document-write",
      "no-mutation-events",
      "no-old-flexbox",
      "time-to-interactive",
      "user-timings",
      "viewport",
      "without-javascript"
    ]
  }
}
```

## Remember

Enjoy!
