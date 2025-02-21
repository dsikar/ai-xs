# ai-xs
AI-Xs formerly AI Tweets

```
+-----------------+
| Start           |
+-----------------+
          |
          v
+-----------------+
| 1. Schedule     | ---> [Daily, e.g., 8 AM EST]
|    Task         |
+-----------------+
          |
          v
+-----------------+             +-----------------+
| 2. Query APIs   | ---------> | a. arXiv API     | ---> [GET new papers, cs.AI]
|    for Papers   |             | (cat:cs.AI)     |
|                 |             +-----------------+
|                 |             | b. Semantic     | ---> [GET trending AI papers]
|                 | ---------> |    Scholar API  |
+-----------------+             +-----------------+
          |
          v
+-----------------+
| 3. Process      | ---> [Extract: Title, URL, Date]
|    Results      | ---> [Filter: New/Relevant, Avoid Dupes]
+-----------------+
          |
          v
+-----------------+
| 4. Generate     | ---> [Format: "New AI paper: {title} [URL] #AI"]
|    Tweets       |
+-----------------+
          |
          v
+-----------------+
| 5. Validate     | ---> [Check: <280 chars, No Errors]
|    Tweets       |
+-----------------+
          |
          v
+-----------------+             +-----------------+
| 6. Post to X    | ---------> | X API Free Tier | ---> [POST up to 500/mo]
|    via API      |             +-----------------+
+-----------------+
          |
          v
+-----------------+
| 7. Log          | ---> [Record: Tweet ID, Date, Status]
|    Activity     |
+-----------------+
          |
          v
+-----------------+
| End             |
+-----------------+
```
