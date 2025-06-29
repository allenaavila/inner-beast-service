
# Inner Beast Service Overview

## Find Your Inner Beast

With this REST API, you have the ability to create and manage personality quizzes that determine a quiz-taker's inner beast.

This service enables you to:

* Generate a multiple choice personality quiz. Each answer choice links to a personality trait value in the **beast** resource.
* Fetch animal personality data from the **beast** resource.

## Why use this service?

You can use this service to quickly implement a "personality match" feature in your web or mobile applications.

This service saves you time and effort because you won't have to manually build out the entire data model and content for quiz questions and animal profiles.

## API Resources

The Inner Beast Service uses these two resources: `beasts` and `quizdefinitions`.

* [Beasts](../api/beasts.md)
  * [GET beasts](../api/beasts-get-beasts.md)
  * [GET beasts by ID](../api/beasts-get-beasts-by-id.md)
* [Quiz definitions](../api/quizdefinitions.md)
  * [GET quiz definitions](../api/quizdefinitions-get-quiz-definitions.md)
  * [GET quiz definitions by ID](../api/quizdefinitions-get-quizdefinition-by-id.md)
