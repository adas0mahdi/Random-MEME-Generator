# Random-MEME-Generator
Random MEME Generator Using HTML CSS JavaScript
⚠️ Heroku has discontinued support for free Dynos, so the old Domain meme-api.herokuapp.com has stopped working ⚠️

Please update your apps to the new Domain meme-api.com to continue using the API

CodeFactor Codacy Badge DeepSource

JSON API for a random meme scraped from reddit.

API Link : https://meme-api.com/gimme

Example Response:

{
 "postLink": "https://redd.it/jiovfz",
  "subreddit": "dankmemes",
  "title": "*leaves call*",
  "url": "https://i.redd.it/f7ibqp1dmiv51.gif",
  "nsfw": false,
  "spoiler": false,
  "author": "Spartan-Yeet",
  "ups": 3363,

  // preview images of the meme sorted from lowest to highest quality
  "preview": [
    "https://preview.redd.it/f7ibqp1dmiv51.gif?width=108&crop=smart&format=png8&s=02b12609100c14f55c31fe046f413a9415804d62",
    "https://preview.redd.it/f7ibqp1dmiv51.gif?width=216&crop=smart&format=png8&s=8da35457641a045e88e42a25eca64c14a6759f82",
    "https://preview.redd.it/f7ibqp1dmiv51.gif?width=320&crop=smart&format=png8&s=f2250b007b8252c7063b8580c2aa72c5741766ae",
    "https://preview.redd.it/f7ibqp1dmiv51.gif?width=640&crop=smart&format=png8&s=6cd99df5e58c976bc115bd080a1e6afdbd0d71e7"
  ]
}




Custom Endpoints
Specify count (MAX 50)
In order to get multiple memes in a single request specify the count with the following endpoint.

Endpoint: /gimme/{count}

Example: https://meme-api.com/gimme/2

Response:

{
  "count": 2,
  "memes": [
    {
      "postLink": "https://redd.it/jictqq",
      "subreddit": "dankmemes",
      "title": "Say sike",
      "url": "https://i.redd.it/j6wu6o9ncfv51.gif",
      "nsfw": false,
      "spoiler": false,
      "author": "n1GG99",
      "ups": 72823,
      "preview": [
        "https://preview.redd.it/j6wu6o9ncfv51.gif?width=108&crop=smart&format=png8&s=3b110a4d83a383b7bfebaf09ea60d89619cddfb3",
        "https://preview.redd.it/j6wu6o9ncfv51.gif?width=216&crop=smart&format=png8&s=ba5808992b3245a6518dfe759cbe4af24e042f2d",
        "https://preview.redd.it/j6wu6o9ncfv51.gif?width=320&crop=smart&format=png8&s=7567bb64e639223e3603236f774eeca149551313"
      ]
    },
    {
      "postLink": "https://redd.it/jilgdw",
      "subreddit": "dankmemes",
      "title": "I forgot how hard it is to think of a title",
      "url": "https://i.redd.it/jk12rq8nrhv51.jpg",
      "nsfw": false,
      "spoiler": false,
      "author": "TheRealKyJoe01",
      "ups": 659,
      "preview": [
        "https://preview.redd.it/jk12rq8nrhv51.jpg?width=108&crop=smart&auto=webp&s=d5d3fe588ccff889e61fca527c2358e429845b80",
        "https://preview.redd.it/jk12rq8nrhv51.jpg?width=216&crop=smart&auto=webp&s=b560b78301afd8c173f8c702fbd791214c1d7f61",
        "https://preview.redd.it/jk12rq8nrhv51.jpg?width=320&crop=smart&auto=webp&s=3cd427240b2185a3691a818774214fd2a0de124d",
        "https://preview.redd.it/jk12rq8nrhv51.jpg?width=640&crop=smart&auto=webp&s=1142cc19a746b8b5d8335679d1d36127f4a677b9"
      ]
    }
  ]
}
