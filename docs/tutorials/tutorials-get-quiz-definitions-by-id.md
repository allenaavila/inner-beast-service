# Get quiz definitions by ID

## Context

In this tutorial, you'll learn how to retrieve a specific `quizdefinition` using its `quizId`.

This action enables you to efficiently access and view the questions and answers that define a specific quiz.

## Prerequisites

Complete the [Get Started](../overview/get-started.md) topic to set up your computer for the Inner Beast Service.

## Steps

1. Open GitHub Desktop.

    Access your clone of the Inner Beast repository on your computer's command-line interface.

2. From your command line, start your local service:

   ```shell
    cd api
    json-server -w beast-db.json
   ```

3. Open the Postman desktop app.  

   Select the **GET** method.
  
   Enter this URL:  

    ```shell
    http://localhost:3000/quizdefinitions?quizId={quizId}
    ```

    Click **Send**.

## Result

The service returns the `quizdefinition` that you requested using the `quizId`.

## Example

### Request

```shell
http://localhost:3000/quizdefinitions?quizId=innerBeastDiscovery_v1
```

### Response

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
      ]
     }
```
