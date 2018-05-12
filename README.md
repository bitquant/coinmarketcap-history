# coinmarketcap-history
Cryptocurrency historical data download from CoinMarketCap

## Install
```
$ npm install coinmarketcap-history --save
```

## Usage
```javascript
var coinmarketcap = require("coinmarketcap-history");

coinmarketcap.getHistory("bitcoin")
  .then(data => console.log(JSON.stringify(data, null, 2)))
  .catch(err => console.error(err.stack ? err.stack : err));

/*
[
  [
    "May 11, 2018",
    "9,052.96",
    "9,052.96",
    "8,394.46",
    "8,441.49",
    "8,488,520,000",
    "154,142,000,000"
  ],
  [
    "May 10, 2018",
    "9,325.96",
    "9,396.04",
    "9,040.52",
    "9,043.94",
    "6,906,700,000",
    "158,772,000,000"
  ],
  ...
  [
    "Apr 28, 2013",
    "135.30",
    "135.98",
    "132.10",
    "134.21",
    "-",
    "1,500,520,000"
  ]
]  
*/
```

## License
MIT license; see [LICENSE](./LICENSE).
