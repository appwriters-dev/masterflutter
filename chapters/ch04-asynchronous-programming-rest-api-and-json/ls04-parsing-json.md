---
id: ls04-parsing-json
title: Parsing JSON
---

In the previous chapter, we learned how to make a request to a REST API and get a response. In this chapter, we will learn how to parse the response and extract the data we need. We will use the [JSON](https://www.json.org/json-en.html) format to represent the data.

## Projects

### 1. Pokemon

Create a Pokemon class that mimics the JSON response from the [PokeAPI](https://pokeapi.co/) that you used inthe previous chapter. Add a From Map method that takes a `Map<String, dynamic>` and returns a Pokemon object. Update the project from previous chapter to use the Pokemon class.

### 2. Movie

Create a Movie class that mimics the JSON response from the [OMDB API](http://www.omdbapi.com/) that you used in the previous chapter. Add a From Map method that takes a `Map<String, dynamic>` and returns a Movie object. Update the project from previous chapter to use the Movie class.
