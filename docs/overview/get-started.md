# Get Started

## Prerequisites

On your computer, you must have:

* [A GitHub account](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://github.com/signup&ved=2ahUKEwi6uOqCnviNAxW2LTQIHSTyNFAQFnoECBcQAQ&usg=AOvVaw0a6qEmIZVdziwPUb-hFApr)
* [Git](https://git-scm.com/downloads)
* [GitHub desktop app](https://github.com/apps/desktop)
* [Postman desktop app](https://www.postman.com/downloads)
* [Node.js](https://nodejs.org/en/download)
* [Json-server](https://www.npmjs.com/package/json-server)

## Context

To simulate using this fictional API service, you must complete this topic before you follow any [tutorials](../tutorials/tutorials.md) or use the Inner Beast REST API.

## Steps

1. Access the [Inner Beast Service repository](https://github.com/allenaavila/inner-beast-service).
2. [Fork the Inner Beast Service repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo?tool=webui#forking-a-repository).
3. [Clone your fork of the Inner Beast repository to your GitHub desktop app](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo?tool=webui#forking-a-repository).

## Results

You now have a copy of the Inner Beast Service repository on your local computer that you can use.

## Next steps

Test your development system is correctly configured.

1. Access your clone of the Inner Beast repository on your computer's command-line interface.

   ```shell
    cd api
    json-server -w beast-db.json
    ```

2. Verify you receive the following response to confirm that the service started successfully:

   ```shell
    \{^_^}/ hi!

    Loading beast-db.json
    Done

    Resources
    http://localhost:3000/beasts
    http://localhost:3000/quizdefinitions

    Home
    http://localhost:3000
    ```

3. Leave the first window open with the service running. Open a new window of your command-line interface to test calling the service.

   Example:

```shell
   curl http://localhost:3000/beasts
   ```

4. Verify that the service returns the expected response.

   Example:

```json
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
