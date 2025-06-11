
# `beasts` resource

Base endpoint:

```shell

{server_url}/beasts
```

Contains a collection of animal profiles with personality traits corresponding to the facets in the quiz. The facets and personality traits accomplish the mapping.

## Resource properties

Sample `beast` resource

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

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `beastID` | string | The ID of the beast |
| `name` | string | The name of the beast|
| `type` | string | `Real` or `Mythical`|
| `coreTraits` | string | The description of the beast's personality traits |
| `elaboration` | string| The additional information about the beast personality type.|
| `wordsOfWisdom` | string| The task's unique record ID |
| `imageURL` | string | The URL with an image of the beast|
