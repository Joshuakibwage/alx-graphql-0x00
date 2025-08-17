# 🎬 Episode Queries – Rick & Morty API

This project demonstrates how to use **GraphQL** to fetch episode details by ID from the [Rick and Morty API](https://rickandmortyapi.com/graphql).  
The task is part of the **ALX GraphQL 0x00** module.

---

## 📂 Files

- `episode-id-1.graphql` → Query for episode with ID 1  
- `episode-id-1-output.json` → Output of the query  
- `episode-id-2.graphql` → Query for episode with ID 2  
- `episode-id-2-output.json` → Output of the query  
- `episode-id-3.graphql` → Query for episode with ID 3  
- `episode-id-3-output.json` → Output of the query  
- `episode-id-4.graphql` → Query for episode with ID 4  
- `episode-id-4-output.json` → Output of the query  

---

## 🔎 Example Query

```graphql
query {
  episode(id: 1) {
    id
    name
    air_date
    episode
  }
}


---

📤 Example Output

{
  "data": {
    "episode": {
      "id": "1",
      "name": "Pilot",
      "air_date": "December 2, 2013",
      "episode": "S01E01"
    }
  }
}
