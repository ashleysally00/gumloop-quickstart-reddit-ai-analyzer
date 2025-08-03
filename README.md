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

1. On your Gumloop dashboard, click **New Flow** to start a project.  
   <img src="https://raw.githubusercontent.com/ashleysally00/gumloop-quickstart-reddit-ai-analyzer/main/AddFirstNode.png" width="50%"/>
2. Drag the **Reddit Scraper** node onto the canvas.  
   <img src="https://raw.githubusercontent.com/ashleysally00/gumloop-quickstart-reddit-ai-analyzer/main/RedditScraper.png" width="50%"/>
3. Set the subreddit to `artificialintelligence`.  
4. Choose sorting: `top`, `hot`, or `new`. (Use `top` for this guide.)  
   <img src="https://raw.githubusercontent.com/ashleysally00/gumloop-quickstart-reddit-ai-analyzer/main/SearchForReddit.png" width="50%"/>
5. Optional: Set a post limit (e.g., 15).  
6. Turn **Loop Mode ON**.  
7. Use outputs like: `post_titles`, `post_urls`, `post_contents`, `post_dates`.

