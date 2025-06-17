# Get quiz definitions by ID

## Prerequisites

Complete the [Get Started](../overview/get-started.md) topic to set up your computer for the Inner Beast REST API.

## Context

In this tutorial, you'll learn how to retrieve a specific `quizdefinition` using its `quizId`.

This action enables you to efficiently access and view the questions and answers that define a specific quiz.

## Steps

1. Open GitHub Desktop.

   Open your fork of the Inner Beast Service repository in your development system's command line.

2. From your command line, start your local service:

```shell
{
     cd <your-github-workspace>/inner-beast-service/api
 json-server -w beast-db.json
}
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
[
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
            },
            {
                "questionId": "q2",
                "text": "There's a complex problem at work/school. Your first instinct is to:",
                "facetTargeted": "Problem-Solving Approach",
                "answers": [
                    {
                        "answerId": "q2a1",
                        "text": "Gather all data, analyze options, and devise a step-by-step plan.",
                        "mapsToTraitValue": "Strategic & Methodical"
                    },
                    {
                        "answerId": "q2a2",
                        "text": "Find a clever, unconventional angle that others might have missed.",
                        "mapsToTraitValue": "Resourceful & Clever"
                    },
                    {
                        "answerId": "q2a3",
                        "text": "Tackle it head-on with courage and decisive action.",
                        "mapsToTraitValue": "Direct & Courageous"
                    },
                    {
                        "answerId": "q2a4",
                        "text": "Rally the team and work collaboratively to find a solution.",
                        "mapsToTraitValue": "Collaborative & Instinctive"
                    }
                ]
            },
            {
                "questionId": "q3",
                "text": "When you face a significant setback or failure, how do you typically react?",
                "facetTargeted": "Response to Adversity",
                "answers": [
                    {
                        "answerId": "q3a1",
                        "text": "See it as a chance to learn, rebuild, and come back stronger.",
                        "mapsToTraitValue": "Resilient & Transformative"
                    },
                    {
                        "answerId": "q3a2",
                        "text": "Focus on protecting what's important and defending your position.",
                        "mapsToTraitValue": "Protective & Strong"
                    },
                    {
                        "answerId": "q3a3",
                        "text": "Quickly adapt to the new situation and find an alternative path.",
                        "mapsToTraitValue": "Adaptable & Quick-thinking"
                    },
                    {
                        "answerId": "q3a4",
                        "text": "Withdraw to process, understanding that some things take time to heal/resolve.",
                        "mapsToTraitValue": "Cautious & Patient"
                    }
                ]
            },
            {
                "questionId": "q4",
                "text": "What drives you most in life?",
                "facetTargeted": "Primary Motivation",
                "answers": [
                    {
                        "answerId": "q4a1",
                        "text": "Achieving great things and making a powerful impact.",
                        "mapsToTraitValue": "Ambition & Power"
                    },
                    {
                        "answerId": "q4a2",
                        "text": "Seeking truth, understanding, and profound knowledge.",
                        "mapsToTraitValue": "Wisdom & Knowledge"
                    },
                    {
                        "answerId": "q4a3",
                        "text": "Ensuring fairness, protecting the vulnerable, and upholding ideals.",
                        "mapsToTraitValue": "Justice & Guardianship"
                    },
                    {
                        "answerId": "q4a4",
                        "text": "Spreading kindness, fostering harmony, and connecting with others.",
                        "mapsToTraitValue": "Purity & Empathy"
                    }
                ]
            },
            {
                "questionId": "q5",
                "text": "When you need to communicate an important idea, you usually:",
                "facetTargeted": "Communication Style",
                "answers": [
                    {
                        "answerId": "q5a1",
                        "text": "State it clearly, confidently, and directly to get your point across.",
                        "mapsToTraitValue": "Direct & Assertive"
                    },
                    {
                        "answerId": "q5a2",
                        "text": "Listen carefully to others first, then offer a thoughtful, well-considered response.",
                        "mapsToTraitValue": "Considered & Observational"
                    },
                    {
                        "answerId": "q5a3",
                        "text": "Use humor and playful language to make your message engaging.",
                        "mapsToTraitValue": "Playful & Engaging"
                    },
                    {
                        "answerId": "q5a4",
                        "text": "Speak with compassion, aiming to connect emotionally and ensure understanding.",
                        "mapsToTraitValue": "Empathetic & Gentle"
                    }
                ]
            }
        ]
    }
]
```
