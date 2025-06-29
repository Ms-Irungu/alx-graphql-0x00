## Assignment 3: Get a Specific Episode by ID

### Objective
Write GraphQL queries to retrieve specific episode information using their ID.

### Directory
`episode/` - Contains all episode-related queries and outputs

### Files Description
- `episode-id-1.graphql` - GraphQL query for episode with ID 1
- `episode-id-1-output.json` - Expected output for episode ID 1
- `episode-id-2.graphql` - GraphQL query for episode with ID 2
- `episode-id-2-output.json` - Expected output for episode ID 2
- `episode-id-3.graphql` - GraphQL query for episode with ID 3
- `episode-id-3-output.json` - Expected output for episode ID 3
- `episode-id-4.graphql` - GraphQL query for episode with ID 4
- `episode-id-4-output.json` - Expected output for episode ID 4

### Query Structure
Each query uses the `episode(id: ID!)` field and includes the following fields:
- id
- name
- air_date
- episode

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
