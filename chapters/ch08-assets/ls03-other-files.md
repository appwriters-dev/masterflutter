---
id: ls03-other-files
title: Other Files
---

Other files, such as a JSON file containing our own data, custom files specific to our project, or even a PDF file, can be added to assets. We can place any file in our assets folder.

## Projects

### 1. A Quiz App

Load question data from a JSON file in asset. Create a new file `assets/questions.json` in your Flutter project. Add it to asset.

```json
[
    {
      "question": "What is the capital of Nepal?",
      "answers": ["Kathmandu", "Pokhara", "Biratnagar", "Lalitpur"],
      "correctAnswer": "Kathmandu"
    },
    {
    "question": "What is the capital of India?",
    "answers": ["New Delhi", "Mumbai", "Kolkata", "Chennai"],
    "correctAnswer": "New Delhi"
    },
    {
    "question": "What is the capital of Pakistan?",
    "answers": ["Islamabad", "Karachi", "Lahore", "Peshawar"],
    "correctAnswer": "Islamabad"
    },
    {
    "question": "What is the capital of Bangladesh?",
    "answers": ["Dhaka", "Chittagong", "Khulna", "Rajshahi"],
    "correctAnswer": "Dhaka"
    },
    {
    "question": "What is the capital of Sri Lanka?",
    "answers": ["Colombo", "Kandy", "Galle", "Jaffna"],
    "correctAnswer": "Colombo"
    }
]
```

Display these questions in a quiz app. You can use the `Quiz` app from the previous chapter.

### 2. A Chart

Load the following user data from `assets/data.json` and display it in a chart.

```json
[
    {
      "name": "John",
      "age": 30,
      "height": 6.0,
      "weight": 150
    },
    {
      "name": "Jane",
      "age": 25,
      "height": 5.5,
      "weight": 120
    },
    {
      "name": "Jack",
      "age": 28,
      "height": 5.8,
      "weight": 130
    },
    {
      "name": "Jill",
      "age": 32,
      "height": 5.6,
      "weight": 140
    }
]
```

Plot the height and weight of the users in a line chart.

> Hint: Use the [fl_chart](https://pub.dev/packages/fl_chart) package. Or you may use any other charting package of your choice from [pub.dev](https://pub.dev/).

## Resources

- [Flutter assets and images](https://flutter.dev/docs/development/ui/assets-and-images)
- [JSON and serialization](https://flutter.dev/docs/development/data-and-backend/json)
- [FL Chart](https://pub.dev/packages/fl_chart)
