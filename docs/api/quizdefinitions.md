# `quizdefinitions` resource

Base endpoint:

```shell

{server_url}/quizdefinitions
```

Defines the structure of the personality quiz, including questions and answer options that map to specific personality traits.

## Resource properties

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `quizId` | string | The quiz's ID |
| `title` | string | The quiz's title |
| `description` | string | The quiz's details |
| `questions` | string | The questions in the quiz |
| `text` | string | The quiz's description for the question or the answer |
| `facetTargeted` | string | The personality facet that the question focuses on |
| `answers` | string | The answers to the quiz question |
| `answerId` | string | The answer's ID |
| `mapstoTraitValue` | string | The beast's personality trait that the answer maps to |

## Example

This is a sample `quizdefinitions` resource:

```js
 {
      "quizId": "innerBeastDiscovery_v1",
      "title": "Find Your Inner Beast",
      "description": "Answer these questions thoughtfully to unveil the animal spirit that resonates most with your personality.",
      "questions": [
        {
          "questionId": "q1",
          "text": "When you're at a party or social gathering, where are you most likely to be found?",
          "facetTargeted": "Social Interaction",
          "answers": [
            {
              "answerId": "q1a1",
              "text": "In the middle of a lively group, energizing the conversation.",
              "mapsToTraitValue": "Highly Social & Playful" 
            },
            {
              "answerId": "q1a2",
              "text": "Having a deep, meaningful conversation with one or two people.",
              "mapsToTraitValue": "Loyal to a Small Group"
            },
            {
              "answerId": "q1a3",
              "text": "Observing from the sidelines, taking it all in before engaging.",
              "mapsToTraitValue": "Observational & Introverted"
            },
            {
              "answerId": "q1a4",
              "text": "Enjoying my own company, perhaps near the snacks, perfectly content.",
              "mapsToTraitValue": "Values Solitude"
            }
          ]
        }
```

## Get operations

* [GET quiz definitions](./quizdefinitions-get-quiz-definitions.md)
* [GET quiz definitions by ID](./quizdefinitions-get-quiz-definitions-by-id)

## Related Information

* [Beast resource](./beasts.md)
