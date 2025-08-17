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

