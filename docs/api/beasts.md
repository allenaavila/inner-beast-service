
# `beasts` resource

Base endpoint:

```shell

{server_url}/beasts
```

Contains a profile of an animal that represents a specific personality type, including trait descriptions used to match quiz-takers to the beast that represents them.

## Resource properties

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `beastID` | string | The unique ID of the beast.|
| `name` | string | The name of the beast.|
| `type` | string | The category of the beast, such as `Real` or `Mythical`. |
| `coreTraits` | object | An object containing the beast's core personality traits.|
| `coreTraits.socialInteraction` | string | The beast's preference for social interactions. |
| `coreTraits.problemSolvingApproach` | string | The beast's typical approach to solving problems. |
| `coreTraits.responsetoAdversity` | string | The beast's typical response to hardship or obstacles.|
| `coreTraits.primaryMotivation` | string | The beast's main source of motivation. |
| `coreTraits.communicationStyle` | string | The beast's preferred communication style. |
| `elaboration` | string| A brief description elaborating on the beast's personality type. |
| `wordsOfWisdom` | string| Advice or insight associated with the beast.|
| `imageURL` | string | A URL linking to an image representing the beast.|

## Example

This is a sample `beast` resource:

```js
{
    "beastId": "wolf",
      "name": "Wolf",
      "type": "Real",
      "coreTraits": {
        "socialInteraction": "Loyal to a Small Group",
        "problemSolvingApproach": "Collaborative & Instinctive",
        "responseToAdversity": "Resilient & United",
        "primaryMotivation": "Pack & Loyalty",
        "communicationStyle": "Coordinated & Instinctual"
      },
      "elaboration": "Resilient and resourceful, especially when working with trusted allies, forming strong bonds and fiercely devoted to their 'pack.'",
      "wordsOfWisdom": "Your loyalty to the pack is your strength, but be wary that the lone wolf's howl for independence isn't misinterpreted as a challenge to the hunt.",
      "imageUrl": "https://example.com/images/beasts/wolf.png"
}
```

## GET operations

* [GET beasts](./beasts-get-beasts.md)
* [GET beasts by id](./beasts-get-beasts-by-id.md)

## Related Information

* [Quiz definitions resource](./quizdefinitions.md)
