# GET quiz definition by quiz ID

Returns all `quizdefinitions` specified by the `quizId` parameter, if it exists.

## URL

```shell

{server_url}/quizdefinitions?quizId={quizId}
```

## Parameters

| Name | Type | Description |
| ------------- | ----------- | ----------- |
| `quizId` | string | The ID of the quiz to return. |

## Authorization

None

## Request headers

None

## Request body

None

## Return body

```js
[ 
    {
      "quizId": "innerBeastDiscovery_v1",
      "title": "Find Your Inner Beast",
      "description": "Answer these questions thoughtfully to unveil the animal spirit that resonates most with your personality.",
      "questions": 
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
    }
]
```

## Return status

| HTTP status code| Description |
| ------------- | ----------- |
| 200 OK| Specified quiz returned successfully. |
| 400 Not Found | Specified quiz definition not found. |

## Related information

* [Quiz definitions](./quizdefinitions.md)
* [GET quiz definitions](./quizdefinitions-get-quiz-definitions.md)
