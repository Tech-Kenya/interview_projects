**Technical Assessment**

# Overview

The core requirement is to build a web application and a backend application that integrates with the [FBI Wanted API](https://www.fbi.gov/wanted/api)

The exercise is intended to evaluate the candidate's technical and problem-solving skills in both frontend and backend development.

## Objective

Build a full-stack application (frontend + backend) that consumes and manages information from the FBI Wanted API

## Tech Stack Choices

1. Frontend: ReactJS or VueJS
2. Backend: Java, Kotlin, Go, PHP or NodeJS

## Expected deliverables

A functional web application with key features implemented, demonstrating your ability to integrate external data, handle it on the server, and present it effectively on the frontend.

# Key areas of focus

## Integration with external API

1. Understanding of RESTful API concepts.
2. Ability to fetch data from the FBI Wanted API endpoints
3. How errors and edge cases are handled (eg. rate-limiting, malformed requests, interuptions)

## Backend development

1. Creating RESTful endpoints or GraphQL resolvers (whichever is preferred) to securely and efficiently handle data from the FBI Wanted API.
2. Data transformations and caching strategies (if applicable)
3. Proper error handling and logging on the server side.

## Frontend development

1. Building a responsive interface using ReactJS or VueJS
2. Proper component structure, state management, and data flow (eg Redux, Vuex, Context APIs or Composition APIs)
3. Good UI/UX principles, including consistent styling and a clear navigation scheme

## Testing

1. Unit testing and/or integration testing of critical functionality both on the frontend and backend.
2. Understanding of testing frameworks and best practices for the chosen languages.

## Documentation and code quality

1. Clear and concise documentation for setup and usage.
2. Code readability, maintainability, and adherence to style guidelines.

# Detailed Requirements

## Fetching data

1. At minimum, fetch a list of wanted persons from the FBI Wanted API and display relevant information (eg. name, description, image)
2. Implement pagination or infinite scrolling when displaying the list

## Search and filter

1. Implement a search feature that allows users to search for wanted persons based on parameters supported by the API (eg name, keywords, subject)
2. Allow users to filter the results (eg by hair color, eye color, race etc) if such data is provided by the API

## Detailed view

1. Enable users to select an item from the list to view more details. (eg personal details, descriptions, alerts, caution, field offices)
2. Include an "additional information" panel that might include external links, if provided in the API response.

## Backend integration

1. Expose a simple backend endpoint (eg /api/wanted ) that the frontend consumes. This backend endpoint should proxy or transform data from the FBI Wanted API.
2. Implement at least one form of caching or data storage mechanism (optional to store the results in memory or a small database) to illustrate how your app handles repeated requests.

## Error handling

1. Display meaningful error messages on the frontend (eg "Unable to fetch data", "Search returned no results")
2. Handle service failures gracefully

# Nice to have features

## Authentication

A simple login flow (session or token-based) to demonstrate secure routes or personalized data

## Advanced filtering

More granular filter options if the API supports additional filtering parameters

## Performance optimizations

Caching strategy or local data store for offline capability or faster UI

## Automated testing

Frontend: Unit testing with Jest, Mocha or equivalent.
Backend: Using JUnit/TestNG, Go testing libraries, PHPUnit, Jest (NodeJS) or another relevant testing framework

## Containerization

Use Docker to containerize the application for easier deployment