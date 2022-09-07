# Phase 3 React-Frontend-App: Construction blog

## Links

This are the links to the live site on GitHub Pages. 

``
frontend link
``
https://four-gables-app.herokuapp.com/

``
backend link
``
https://powerful-gorge-80946.herokuapp.com/houseData

## Introduction

Welcome to my construction blogs app, where all your construction questions are answered! We encourage you to search, read, explore, learn and let us guide you blog. Our layout is extremely user friendly, offering a beautiful interface as the stories we share. 

Join us as we take you through what you expect from us.

## Setup

## Core Deliverables

As a user:

1. When the app starts, I can view all currently uploaded blogs.
2. I can add a new blog to the list of blogs while sending that data back to the backend model.
3. I can delete blogs and add blogs at will.
4. I can update the blogs too at will.

### Endpoints for Core Deliverables

#### GET /blogs

Example Response:

```json
[
  {
      "id": 1,
      "title": "Baraza",
      "rating": 3,
      "authorId": 2,
      "Content": "Get woken up by the cool breeze of the ocean."
    },
    {
      "id": 3,
      "title": "Esther",
      "rating": 4,
      "authorId": 1,
      "content": "Beautiful waterfall scenery."
    },
]
```

#### POST `/blogs`

Required Headers:

```js
{
  "Content-Type": "application/json"
}
```

Request Object:

```json
{
  "title": "Billy",
  "rating": "Omollo",
  "authorId": "billyomollo@gmail.com",
  "content": "When you want a town setting."
},   
```

Example Response:

```json
{
  "title": "Billy",
  "rating": "Omollo",
  "authorId": "billyomollo@gmail.com",
  "content": "When you want a town setting."
},
```
#### DELETE `/blogs/:id`

```
Using a button, function and the filter method, a blog can be deleted and the remaining blogs displayed.

Example Response:

```json
{}
```

#### Advanced Deliverables

```
As a user:

1. I can add a blog to my favorites and see it on a separate list.
2. I can click on a blog and see it on a separate page with more detailed content.

```