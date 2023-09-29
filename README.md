# **Link to Shrink API**
Published backend API app to reduce the length of links provided by user

**Common API usage:**
```
*Take short view of link by pushing original version*
- METHOD [POST] localhost:3000/shrinkUrl
- BODY x-www-urlencoded
- KEY url VALUE https://kinsta.com/blog/docker-compose-volumes/
```
```
*Take short view of link by pushing original version*
- METHOD [GET] localhost:3000/getLinkByUrl
- PARAMS
- KEY "url" VALUE "your-link"
```
```
*Take original view of link by pushing reduced version*
- METHOD [GET] localhost:3000/getLinkByShortUrl
- PARAMS
- KEY "shortUrl" VALUE "your-short-link"
```
```
Used:
- TS, JS
- Node.js, Express.js
- Sequelize, Redis(as cache for fast requests)
```
Example
![LinkToShrink](https://github.com/Javez/LinkToShrink/assets/66317972/cf2b854d-c713-47f6-a953-daa3eda06fff)
