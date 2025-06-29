# GraphQL Character Queries

This directory contains GraphQL queries to fetch specific character information by ID from the Rick and Morty API.

## Objective
Write GraphQL queries to retrieve specific character information using their ID.

## Endpoint
The GraphQL endpoint used is: `https://rickandmortyapi.com/graphql`

## Files Description

- `character-id-1.graphql` - GraphQL query for character with ID 1
- `character-id-1-output.json` - Expected output for character ID 1
- `character-id-2.graphql` - GraphQL query for character with ID 2
- `character-id-2-output.json` - Expected output for character ID 2
- `character-id-3.graphql` - GraphQL query for character with ID 3
- `character-id-3-output.json` - Expected output for character ID 3
- `character-id-4.graphql` - GraphQL query for character with ID 4
- `character-id-4-output.json` - Expected output for character ID 4

## Query Structure
Each query uses the `character(id: ID!)` field and includes the following fields:
- id
- name
- status
- species
- type
- gender

## Assignment 2: Get a List of All Characters (Paginated)

### Objective
Create GraphQL queries to retrieve a paginated list of all characters.

### Files Description
- `characters-page-1.graphql` - GraphQL query for characters page 1
- `characters-page-1-output.json` - Expected output for page 1
- `characters-page-2.graphql` - GraphQL query for characters page 2
- `characters-page-2-output.json` - Expected output for page 2
- `characters-page-3.graphql` - GraphQL query for characters page 3
- `characters-page-3-output.json` - Expected output for page 3
- `characters-page-4.graphql` - GraphQL query for characters page 4
- `characters-page-4-output.json` - Expected output for page 4

### Query Structure
Each query uses the `characters(page: Int)` field and includes the following subfields:
- id
- name
- status
- image

The response is nested under the `results` array within the `characters` field.

## How to Test
You can test these queries using:
1. GraphQL Playground at https://rickandmortyapi.com/graphql
2. Copy and paste the query content from any `.graphql` file
3. Click the play button to execute
4. Compare the result with the corresponding output JSON file

## Query Examples

### Single Character Query:
```graphql
query GetCharacterById {
  character(id: 1) {
    id
    name
    status
    species
    type
    gender
  }
}
```

### Paginated Characters Query:
```graphql
query GetCharactersList {
  characters(page: 1) {
    results {
      id
      name
      status
      image
    }
  }
}
```

