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

## How to Test
You can test these queries using:
1. GraphQL Playground at https://rickandmortyapi.com/graphql

