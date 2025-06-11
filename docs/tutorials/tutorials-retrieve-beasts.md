

# Retrieve Beasts

## What you'll learn

In this topic, you'll learn how to get all available `beast` profiles. This provides your application with `beasts` data.

## Steps

1. Open GitHub Desktop.

2. Open your fork of the To-Do-service repository in your development system's command line.

3. Start your local service:`json-server -w beast-db.json`

4. Open the Postman desktop app.

5. Select **GET** from the method dropdown.

6. Call the service: `http://localhost:3000/beasts/{beastId}/lion`

## Response

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
