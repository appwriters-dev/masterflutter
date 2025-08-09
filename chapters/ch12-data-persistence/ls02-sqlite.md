---
id: ls02-sqlite
title: SQLite
description: In this lesson, we will learn how to use SQLite to store structured data.
---

## What is SQLite?

SQLite is a C-language library that implements a small, fast, self-contained, high-reliability, full-featured, SQL database engine. It is the most used database engine in the world.

To use SQLite in Flutter, you can use the `sqflite` package.

```yaml
dependencies:
  sqflite: ^2.0.0
  path: ^1.8.0
```

## Projects

### 1. Simple To-Do App with SQLite

Create a simple to-do app that saves the tasks to a SQLite database. The app should allow the user to add, update, and delete tasks.

Here is an example of how you can implement this:

```dart
import 'package:flutter/material.dart';
import 'package:sqflite/sqflite.dart';
import 'package:path/path.dart';

class Todo {
  final int id;
  final String title;
  final bool completed;

  Todo({required this.id, required this.title, required this.completed});

  Map<String, dynamic> toMap() {
    return {
      'id': id,
      'title': title,
      'completed': completed ? 1 : 0,
    };
  }
}

class DatabaseHelper {
  static final _databaseName = "MyDatabase.db";
  static final _databaseVersion = 1;

  static final table = 'my_table';

  static final columnId = 'id';
  static final columnTitle = 'title';
  static final columnCompleted = 'completed';

  DatabaseHelper._privateConstructor();
  static final DatabaseHelper instance = DatabaseHelper._privateConstructor();

  static Database? _database;
  Future<Database> get database async {
    if (_database != null) return _database!;
    _database = await _initDatabase();
    return _database!;
  }

  _initDatabase() async {
    String path = join(await getDatabasesPath(), _databaseName);
    return await openDatabase(path,
        version: _databaseVersion,
        onCreate: _onCreate);
  }

  Future _onCreate(Database db, int version) async {
    await db.execute('''
          CREATE TABLE $table (
            $columnId INTEGER PRIMARY KEY,
            $columnTitle TEXT NOT NULL,
            $columnCompleted INTEGER NOT NULL
          )
          ''');
  }
}

// ... more code for the app
```

## Resources

- [SQflite package](https://pub.dev/packages/sqflite)
- [Persist data with SQLite](https://flutter.dev/docs/cookbook/persistence/sqlite)
