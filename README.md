# Exercise: API Endpoints

In this exercise, you will be determining RESTful endpoints for an API server
based on the given scenarios.

## Set up

Clone the exercise from the [starter].

## Conventions for RESTful Endpoints for an API Server

The following tables show the conventions for RESTful Endpoints of an API
server.

| Path Pattern             | HTTP Verb | Meaning                                          |
| ------------------------ | --------- | ------------------------------------------------ |
| /resource-name           | GET       | Index: Get all of the records for the resource   |
| /resource-name           | POST      | Create: Create a new record for the resource     |
| /resource-name/record-id | GET       | Details: Get the details of the specified record |
| /resource-name/record-id | PUT/PATCH | Update: Update the specified record              |
| /resource-name/record-id | DELETE    | Delete: Delete the specified record              |

For Nested Resources:

| Path Pattern                             | HTTP Verb | Meaning                                                                                |
| ---------------------------------------- | --------- | -------------------------------------------------------------------------------------- |
| /resource-name/record-id/nested-resource | GET       | Index: Get all of the records for the nested resources related to the specified record |
| /resource-name/record-id/nested-resource | POST      | Create: Create a new record for the nested resource related to the specified record    
| /nested-resource/nested-record-id        | GET       | Details: Get the details of the specified nested resource's record                     |
| /nested-resource/nested-record-id        | PUT/PATCH | Update: Update the specified nested resource's record                                  |
| /nested-resource/nested-record-id        | DELETE    | Delete: Delete the specified nested resource's record                                  |

## Instructions

Determine an endpoint for each of the following use cases. Don't worry about
getting it perfect as this is just practice!

API endpoints use similar routes to a traditional web server's RESTful routes.
The major difference between API endpoints those of a traditional web server is
that API endpoints can use all HTTP verbs (`GET`, `POST`, `PUT`, `PATCH`,
`DELETE`).

For example, to edit a specific post, the API endpoint could be
`PATCH /posts/:postId` 

- Get all the posts / get
- Create a new post / put/ patch
- Edit a post /put / patch
- Create a new user / get
- Get the comments for a post / get
- Create a comment for a post / get / patch
- Edit a comment for a post / update
- Delete a comment for a post/ delete
- Add a like for a post /  put / patch
- Remove a like for a post / delete
- Get all the posts of a user /  get
- Submit a search on posts / put / patch

[starter]: https://github.com/appacademy/practice-for-week-08-creating-api-docs
