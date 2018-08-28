{
  "info": {
    "name": "Spotify Get Album Tracks",
    "_postman_id": "a648dda9-1164-4b4d-8378-4412444cdbdf",
    "description": "[Get an Album's Tracks](https://developer.spotify.com/web-api/get-albums-tracks/)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "music",
      "item": [
        {
          "id": "ca548aff-3f88-41b6-99f1-34e36b555c88",
          "name": "get-an-albums-trackshttpsdeveloperspotifycomwebapigetalbumstracks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spotify.com",
              "path": [
                "v1",
                "albums/:id/tracks"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "market",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "[Get an Album's Tracks](https://developer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1aea9666-fda4-4424-be55-f0900a116ad6"
            }
          ]
        }
      ]
    }
  ]
}