---
id: ls01-http
title: HTTP
description: In this lesson, we will learn how to make HTTP requests in Flutter.
---

## What is HTTP?

HTTP (Hypertext Transfer Protocol) is the protocol used to transfer data over the web. It is the foundation of data communication for the World Wide Web.

To make HTTP requests in Flutter, you can use the `http` package.

```yaml
dependencies:
  http: ^0.13.0
```

## Projects

### 1. Simple App with HTTP

Create a simple app that fetches data from a public API and displays it in a list. You can use the [JSONPlaceholder](https://jsonplaceholder.typicode.com/) API for this project.

Here is an example of how you can fetch a list of posts:

```dart
import 'package:flutter/material.dart';
import 'package:http/http.dart' as http;
import 'dart:convert';

class Post {
  final int id;
  final String title;
  final String body;

  Post({required this.id, required this.title, required this.body});

  factory Post.fromJson(Map<String, dynamic> json) {
    return Post(
      id: json['id'],
      title: json['title'],
      body: json['body'],
    );
  }
}

Future<List<Post>> fetchPosts() async {
  final response = await http.get(Uri.parse('https://jsonplaceholder.typicode.com/posts'));

  if (response.statusCode == 200) {
    List jsonResponse = json.decode(response.body);
    return jsonResponse.map((post) => Post.fromJson(post)).toList();
  } else {
    throw Exception('Failed to load posts');
  }
}

// ... more code for the app
```

## Resources

- [HTTP package](https://pub.dev/packages/http)
- [Fetch data from the internet](https://flutter.dev/docs/cookbook/networking/fetch-data)
