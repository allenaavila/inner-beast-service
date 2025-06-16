
# `beasts` resource

Base endpoint:

```shell

{server_url}/beasts
```

Contains a collection of animal profiles with personality traits corresponding to the facets in the quiz.

## Resource properties

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `beastID` | string | The beast's ID |
| `name` | string | The beast's name|
| `type` | string | The beast's category |
| `coreTraits` | string | The description of the beast's personality traits |
| `socialInteraction` | string | The beast's preference for social interactions |
| `problemSolvingApproach` | string | The beast's approach to solving problems |
| `responsetoAdversity` | string | The beast's response to hardship |
| `primaryMotivation` | string | The beast's main motive |
| `communicationStyle` | string | The beast's preference for communicating |
| `elaboration` | string| Context about the beast's personality type |
| `wordsOfWisdom` | string| Advice for those who receive this beast in the quiz |
| `imageURL` | string | The URL with an image of the beast |

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

## Get operations

* [GET beasts](./beasts-get-beasts.md)
* [GET beasts by id](./beasts-get-beasts-by-id.md)

## Related Information

* [Quiz definitions resource](./quizdefinitions.md)
