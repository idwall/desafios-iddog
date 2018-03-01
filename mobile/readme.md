# IDdog Challenge for Frontend Developers

<img src="media/id-dog.gif" />

## ✍️ Instructions

* Create a `/signup` page with an email `input` to [signup a user](https://iddog-api.now.sh/signup) (only with email)
* Store the returned `token` (cookies / local storage)
* Redirect to `/feed`
* On `/feed` it should [`GET /feed`](https://iddog-api.now.sh/feed)
* Create a menu with 4 routes — `husky`, `labrador`, `hound` and `pug`
* Each route should fetch data on [`GET /feed`](https://iddog-api.now.sh/feed)
* After first fetch, cached the data so when you go back to the route you don't need to fetch it again
* When you click on a photo, it should open the photo as (https://your-website.com/feed?category=Xid=Y)
* When you refresh the page with a photo opened, it should remain on the photo screen
* Deploy your app ([now](https://zeit.co/now) / [heroku](https://www.heroku.com/) / [netlify](https://www.netlify.com/))

**Ps:** You don't need to apply the same styles (CSS and animations)

## 🙋‍ Help

* Use [media](https://github.com/idwall/iddog/tree/master/media) as reference ([GIF](media/id-dog.gif) and 01-07 flow)
* Use React and Redux
* Create tests (components, actions, reducers etc)

## 📃 API

All endpoints live under the URL [`https://iddog-api.now.sh`](https://iddog-api.now.sh) and then generally follow the REST architecture.

All requests must be encoded as JSON with the Content-Type: application/json header. Most responses, including errors, are encoded exclusively as JSON as well.

### POST /signup

#### Signup a user

```bash
POST /signup
```

```bash
curl "https://iddog-api.now.sh/signup" \
-H "Content-Type: application/json" \
-d '{ "email": "your@email.com" }'
```

### GET /feed

#### List of dogs

```bash
GET /feed
```

```bash
curl "https://iddog-api.now.sh/feed" \
-H "Authorization: $TOKEN" \
-H "Content-Type: application/json"
```

##### Queries

##### ?category

**Default**: `husky`<br/>
**Type**: `string`<br/>
**Options**: `husky`, `hound`, `pug`, `labrador`
