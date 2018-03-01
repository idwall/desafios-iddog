# IDdog Challenge for Mobile (Android and iOS) Developers

Gif bellow is just for reference.

<img src="https://github.com/idwall/desafios-iddog/blob/master/frontend/media/id-dog.gif?raw=true" />

## ✍️ Instructions

* Create a `/signup` page with an email `input` to [signup a user](https://iddog-api.now.sh/signup) (only with email)
* Store the returned `token` (local storage)
* Redirect to `/feed`
* On `/feed` it should [`GET /feed`](https://iddog-api.now.sh/feed)
* Create a menu with 4 routes — `husky`, `labrador`, `hound` and `pug`
* Each route should fetch data on [`GET /feed`](https://iddog-api.now.sh/feed)
* After first fetch, cached the data so when you go back to the route you don't need to fetch it again
* When you click on a photo, it should open the photo as (https://your-website.com/feed?category=Xid=Y)
* When you refresh the page with a photo opened, it should remain on the photo screen
* Deploy your app or send for us a way to see application live.

**Ps:** You don't need to apply the same styles (CSS and animations) and you can improve it a lot :P 

## 🙋‍ Help

* Use [media](https://github.com/idwall/desafios-iddog/tree/master/frontend/media) as reference ([GIF](https://github.com/idwall/desafios-iddog/tree/master/frontend/media/id-dog.gif) and 01-07 flow)
* Use React and Redux
* Create tests (components, actions, reducers etc)
