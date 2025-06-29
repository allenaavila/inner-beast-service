# Get beast by ID

## Context

In this tutorial, you'll learn how to retrieve a specific `beast` profile using its `beastId`.

This action enables you to efficiently access and view data on a `beast` profile for your personality quizzes.

## Prerequisites

Complete the [Get Started](../overview/get-started.md) topic to set up your computer for the Inner Beast Service.

## Steps

1. Open GitHub Desktop.

   Open your fork of the Inner Beast Service repository in your development system's command line.

2. From your command line, start your local service:

```shell
    cd <your-github-workspace>/inner-beast-service/api
 json-server -w beast-db.json
```

3. Open the Postman desktop app.  

   Select the **GET** method.
  
   Enter this URL:  

    ```shell
    http://localhost:3000/beasts?beastId={beastId}
    ```

    Click **Send**.

## Result

The service returns the `beast` that you requested using the `beastId`.

## Example

### Request

```shell
http://localhost:3000/beasts?beastId=lion
```

### Response

```js
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
}
```
