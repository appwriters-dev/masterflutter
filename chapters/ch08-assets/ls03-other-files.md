---
id: ls03-other-files
title: Other Files
---

In assets we can add other files like a JSON file with our own data, our own custom files specific to our project, or even a PDF file. We can add any file we want to our assets folder.

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

## Resources

- [Flutter assets and images](https://flutter.dev/docs/development/ui/assets-and-images)
- [JSON and serialization](https://flutter.dev/docs/development/data-and-backend/json)