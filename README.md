# Instagram API Spec JSON

This library provides a simple JSON object which provides a machine readable specification of the Instagram API.

##Some examples:

> instagram["GET"]["/users/search"]

> instagram["POST"]["/media/media-id/likes"]

> instagram["DELETE"]["/media/media-id/comments/comment-id"]

##Sample response

    {
       url: "https://api.instagram.com/v1/users/{user-id}/media/recent",
       headers: [],
       body: [],
       body_meaning: [],
       body_optional: "",
       params: ["access_token", "count", "max_stimestamp", "min_timestamp", "min_id", "max_id"],
       params_meaning: ["A valid access token.", "Count of media to return.", "Return media before this UNIX timestamp.", "Return media after this UNIX timestamp.", "Return media later than this min_id.", "Return media earlier than this max_id."],
       params_optional: "NYYYYY",
       misc: ["You can use self instead of the user-id."],
       authNeeded: "true"
    }



##Contributing:

All contributions are welcome. Need other machine readable specifications of other APIs. Request it and we will get it done. Or better yet, contribute it and we will make you a hero.