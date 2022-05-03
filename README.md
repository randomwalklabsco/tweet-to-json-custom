# tweet-json-to-html-custom

Forked from **[tweet-json-to-html](https://www.npmjs.com/package/tweet-json-to-html)** [converts Twitter API v2 tweet json object into html format with] with styling changes

## Install

```
npm i tweet-json-to-html-custom
```

## Usage

Simply import the package and use it as a function:

```javascript
const tweetJsonToHtml = require('tweet-json-to-html-custom')
const html = await tweetJsonToHtml(tweetJson, 'dim')
```
Here `tweetJson` should contain all possible information. Below is a sample Tweet lookup API URL requested to contain all possible information.

```url
https://api.twitter.com/2/tweets/1295916604127981568?expansions=attachments.poll_ids,attachments.media_keys,author_id,entities.mentions.username,geo.place_id,in_reply_to_user_id,referenced_tweets.id,referenced_tweets.id.author_id&poll.fields=duration_minutes,end_datetime,id,options,voting_status&media.fields=duration_ms,height,media_key,preview_image_url,type,url,width,public_metrics&place.fields=contained_within,country,country_code,full_name,geo,id,name,place_type&tweet.fields=attachments,author_id,context_annotations,conversation_id,created_at,entities,geo,id,in_reply_to_user_id,lang,public_metrics,possibly_sensitive,referenced_tweets,source,text,withheld&user.fields=created_at,description,entities,id,location,name,pinned_tweet_id,profile_image_url,protected,public_metrics,url,username,verified,withheld
```

### tweetJsonToHtml(tweetJson, [background])

Avaliable properties for `background`:

- **default** (Default)
- **dim**
- **lights-out**

## License

MIT License