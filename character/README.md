# 🚀 GraphQL Character Queries – Rick & Morty API

This project demonstrates how to use **GraphQL** to fetch specific character details from the [Rick and Morty API](https://rickandmortyapi.com/graphql).  
The task is part of the **ALX GraphQL 0x00** module.

---

## 📂 Project Structure

```bash
character/
├── README.md
├── character-id-1.graphql
├── character-id-1-output.json
├── character-id-2.graphql
├── character-id-2-output.json
├── character-id-3.graphql
├── character-id-3-output.json
├── character-id-4.graphql
├── character-id-4-output.json

🔎 Queries

Each .graphql file contains a query to fetch character details by ID.
The fields returned are:

    id

    name

    status

    species

    type

    gender

Example (character-id-1.graphql):

query {
  character(id: 1) {
    id
    name
    status
    species
    type
    gender
  }
}

📤 Outputs

Each query’s response is stored in a corresponding .json file.
Example (character-id-1-output.json):

{
  "data": {
    "character": {
      "id": "1",
      "name": "Rick Sanchez",
      "status": "Alive",
      "species": "Human",
      "type": "",
      "gender": "Male"
    }
  }
}

🛠 How to Test

    Open the Rick and Morty GraphQL Playground.

    Copy a query from any character-id-X.graphql file.

    Run it in the playground.

    Compare the response with the corresponding character-id-X-output.json.

✅ Learning Outcomes

    Understanding how to structure a GraphQL query.

    Fetching nested data with a single endpoint.

    Mapping GraphQL query results into .json output.


---

## 📖 Task 2: List of All Characters (Paginated)

This task queries the Rick and Morty API to fetch a list of characters across multiple pages.

### Queries
- `characters-page-1.graphql`
- `characters-page-2.graphql`
- `characters-page-3.graphql`
- `characters-page-4.graphql`

### Fields
- `id`
- `name`
- `status`
- `image`

### Example Query
```graphql
query {
  characters(page: 1) {
    results {
      id
      name
      status
      image
    }
  }
}

Example Output

See characters-page-1-output.json for the full response of page 1.


---

