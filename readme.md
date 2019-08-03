# FortniteAPI.com Node.js wrapper.

Fortnite API for Node.js. Get access to the daily store, the items list, battle pass items, user stats and more.

## Getting Started

How can I use this package?

### Installing

Install our NPM package.

```
npm i fortnite-api-js
```

### Set up

This API requires an API key, which you can get at [www.fortniteapi.com](https://fortniteapi.com)

```
const fortniteapi = require('fortnite-api-js');

fortniteapi.configuration({
  key: 'PUT_YOUR_TOKEN_HERE'
});
```

You're good to go!

### Available functions

| Function             | Input         |
| --------------------|:-------------:|
| getShop             | en, fr or de  |
| getStore            | en, fr or de  |
| getUpcoming         | -             |
| getItemsList        | -             |
| getItem             | the item ID   |
| getPopularItems     | -             |
| getRandomItems      | -             |
| getNews             | br of stw     |
| getCreativeList     | order (popular, views, newest, oldest or rating) |
| getCreativeTags     | -             |
| getCreativeIsland   | island ID     |
| fetchCreativeIsland | island ID     |
| addCreativeIsland   | island ID     |
| creativeSearch      | search input  |
| searchUserId        | username	  |
| getUserStatsV2      | user id	  	  |
| getUserStatsV1      | user id & platform	  |

### Examples

```
fortniteapi.getShop('en').then(data => {
  console.log(data)
})
```

```
fortniteapi.getItem('208f8a9-35aff6e-b1ae608-1cb4c7b').then(data => {
  console.log(data)
})
```

```
fortniteapi.getCreativeIsland('6697-1781-1082').then(data => {
  console.log(data)
})
```


## Built With

* [Axios](https://www.npmjs.com/package/axios) - GET requests to fortniteapi.com
* [foreach](https://www.npmjs.com/package/foreach) - For the configuration :)

## Authors

* **Sam Hoog Antink** - *Initial work* - [samhoogantink](https://github.com/samhoogantink)
