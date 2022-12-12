---
id: ls04-parsing-json
title: Parsing JSON
description: Learn how to convert JSON data into Dart objects and use them to make your code more readable and maintainable.
---

In the previous chapter, we learned how to make a REST API request and receive a response. In this chapter, we'll go over how to parse the response and extract the information we need. To represent the data, we will use the [JSON](https://www.json.org/json-en.html) format.

## Projects

### 1. Pokemon

Create a Pokemon class that mimics the JSON response from the [PokeAPI](https://pokeapi.co/) that you used in the previous chapter. Add a From Map method that takes a `Map<String, dynamic>` and returns a Pokemon object. Update the project from previous chapter to use the Pokemon class.

### 2. Movie

Create a Movie class that mimics the JSON response from the [OMDB API](http://www.omdbapi.com/) that you used in the previous chapter. Add a From Map method that takes a `Map<String, dynamic>` and returns a Movie object. Update the project from previous chapter to use the Movie class.
