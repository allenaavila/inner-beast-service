# GET beasts by ID

Returns all `beasts` specified by the `beastId` parameter, if it exists.

## URL

```shell

{server_url}/beasts?beastId={beastId}
```

## Parameters

| Name | Type | Description |
| ------------- | ----------- | ----------- |
| `beastId` | string | The ID of the beast to return |

## Request headers

None

## Request body

None

## Return body

```js
[
    {
        "beastId": "owl",
        "name": "Owl",
        "type": "Real",
        "coreTraits": {
            "socialInteraction": "Observational & Introverted",
            "problemSolvingApproach": "Strategic & Methodical",
            "responseToAdversity": "Cautious & Perceptive",
            "primaryMotivation": "Wisdom & Understanding",
            "communicationStyle": "Considered & Observational"
        },
        "elaboration": "Often seen as patient and methodical, with a keen eye for detail, preferring to watch, listen, and gather information before acting.",
        "wordsOfWisdom": "While your silent observation gathers all the secrets of the night, remember that sometimes hooting your insights is necessary for the forest to thrive.",
        "imageUrl": "https://example.com/images/beasts/owl.png"
    }
]
```

## Return status

| HTTP status code| Description |
| ------------- | ----------- |
| 200 OK| Returns specified beast successfully. |
| 400 Not Found | Specified beast not found.|

## Related information

* [Beasts](./beasts.md)
* [GET beasts](./beasts-get-beasts.md)
