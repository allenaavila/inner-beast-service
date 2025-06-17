# GET beasts

Returns all `beasts` contained in the service.

## URL

```shell

{server_url}/beasts
```

## Parameters

None

## Request headers

None

## Request body

None

## Return body

```js
[
    {
        "beastId": "lion",
        "name": "Lion",
        "type": "Real",
        "coreTraits": {
            "socialInteraction": "Assertive Leadership",
            "problemSolvingApproach": "Direct & Courageous",
            "responseToAdversity": "Protective & Strong",
            "primaryMotivation": "Courage & Command",
            "communicationStyle": "Direct & Authoritative"
        },
        "elaboration": "Possesses a dignified and commanding presence, inspiring respect and naturally taking charge.",
        "wordsOfWisdom": "Your roar commands attention, but remember even the king of the jungle needs to listen to the whispers of the savanna to truly lead.",
        "imageUrl": "https://example.com/images/beasts/lion.png"
    },
    {
        "beastId": "dolphin",
        "name": "Dolphin",
        "type": "Real",
        "coreTraits": {
            "socialInteraction": "Highly Social & Playful",
            "problemSolvingApproach": "Intelligent & Collaborative",
            "responseToAdversity": "Adaptable & Agile",
            "primaryMotivation": "Joy & Connection",
            "communicationStyle": "Expressive & Communicative"
        },
        "elaboration": "Known for being highly communicative, intelligent, and adaptable in social situations, approaching life with a joyful and inquisitive spirit.",
        "wordsOfWisdom": "Your joyful leaps make waves, but ensure your playful currents don't inadvertently capsize smaller boats in the shared ocean of collaboration.",
        "imageUrl": "https://example.com/images/beasts/dolphin.png"
    }
    ...
]
```

## Return status

| HTTP status code| Description |
| ------------- | ----------- |
| 200 OK| Returns beasts contained in the service. The server has responded successfully. |
| 400 Not Found | Beasts not found.|

## Related information

* [Beasts](./beasts.md)
* [GET beasts by ID](./beasts-get-beasts-by-id.md)
