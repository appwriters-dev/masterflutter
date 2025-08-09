---
id: ls02-dio
title: Dio
description: In this lesson, we will learn how to use Dio to make HTTP requests in Flutter.
---

## What is Dio?

Dio is a powerful HTTP client for Dart, which supports interceptors, global configuration, FormData, request cancellation, file uploading/downloading, timeout, and more.

To use Dio, you need to add the `dio` package to your `pubspec.yaml` file:

```yaml
dependencies:
  dio: ^4.0.0
```

## Projects

### 1. Simple App with Dio

Re-create the app from the previous lesson, but this time use Dio to make the HTTP requests.

Here is an example of how you can fetch a list of posts:

```dart
import 'package:flutter/material.dart';
import 'package:dio/dio.dart';

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
  try {
    Response response = await Dio().get('https://jsonplaceholder.typicode.com/posts');
    List<Post> posts = (response.data as List).map((post) => Post.fromJson(post)).toList();
    return posts;
  } catch (e) {
    throw Exception('Failed to load posts');
  }
}

// ... more code for the app
```

## Resources

- [Dio package](https://pub.dev/packages/dio)
- [Dio documentation](https://github.com/flutterchina/dio)
