# Have You Tried Gumloop Yet?

Use this quickstart guide with a Reddit AI trend analyzer to get started with Gumloop — an automation platform that helps you create visual data workflows using drag, drop, connect, go.

## Step 1: Sign Up or Log In

Go to [Gumloop.com](https://gumloop.com), create a free account or sign in.  
Gumloop is free to use as long as the tools you connect to are also free.  
(For example, GPT-3.5 may be free via OpenAI, while GPT-4 or premium APIs may incur charges.)

---

## Step 2: Add the Reddit Scraper Node

If you're building a custom node from scratch, you'll need to click "+ Add Your First Node" on the canvas to get started. This allows you to define your own inputs, logic, and connections.

Gumloop has many premade nodes designed for specific tools. Different nodes can scrape websites, run AI models, work with spreadsheets, and more.

For this project, we will use the Reddit Scraper node. It's already available in Gumloop’s built-in node library. You don’t need to build it from scratch.

Instead, search for "Reddit Scraper" and drop it into your flow after completing Step 1 (sign-in).

Then continue with the setup:

1. On your Gumloop dashboard, click **Create Flow** to start a project.  
   <img src="https://github.com/ashleysally00/gumloop-quickstart-reddit-ai-analyzer/blob/main/CreateFlow.png" width="40%"/>
2. Search for the **Reddit Scraper** node.
  <img src="https://raw.githubusercontent.com/ashleysally00/gumloop-quickstart-reddit-ai-analyzer/main/SearchForReddit.png" width="30%"/>   

4. Drag the **Reddit Scraper** node onto the canvas.     
   <img src="https://raw.githubusercontent.com/ashleysally00/gumloop-quickstart-reddit-ai-analyzer/main/RedditScraper.png" width="50%"/>

5. Set the subreddit to `artificialintelligence`.  
6. Choose sorting: `top`, `hot`, or `new`. (Use `top` for this guide.)
7. Optional: Set a post limit (e.g., 15).  
8. Turn **Loop Mode ON**.
   ➡️ [Click here to learn how Loop Mode works and when to use it.][What Does Loop Mode Do?](#-what-does-loop-mode-do)
10. Use outputs like: `post_titles`, `post_urls`, `post_contents`, `post_dates`.

---

### What Does Loop Mode Do?

Let's say the Reddit Scraper finds 15 posts.

If you **turn ON Loop Mode**, Gumloop will do the next step (like analyze with AI or send to a spreadsheet) **one post at a time**:

```
Post 1 → analyze
Post 2 → analyze
Post 3 → analyze
... and so on
```

**Use Loop Mode when:**
- You want AI to give feedback on **each post**
- You want to **filter** or **sort** individual posts
- You want to **send each post** to its own row in a spreadsheet

If you **leave Loop Mode OFF**, Gumloop sends all posts together to the next step:

```
All posts → analyze as one big chunk
```

**Use this when:**
- You want a **summary** or overview
- You want **group stats** like keyword frequency across all posts

**In short:**

| Loop Mode     | What happens                  | When to use it                             |
|---------------|-------------------------------|---------------------------------------------|
| ✅ ON          | Each item handled one-by-one  | You want to work with **each post**         |
| ❌ OFF         | All items sent together       | You want to work with the **whole list**    |

---

