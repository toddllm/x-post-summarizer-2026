# x-post-summarizer-2026

AI-generated summary of a public figure's 2026 X posts, built with LangGraph, MCP tools, and the X API.

## Project Description
This repository summarizes a public figure's 2026 X posts using AI. The analyzed account handle is @llm_wizard. The project was built using a LangGraph agent combined with GitHub MCP tools for repository operations and the X API v2 for retrieving posts.

## How It Works
- The LangGraph agent orchestrates the workflow.
- GitHub MCP tools manage repository creation, file commits, branching, and pull requests.
- The X API v2 is used to fetch recent posts from the specified X account.

## Replicating the Process
To replicate this project, follow these steps:

### 1. Set Up Your X API Bearer Token
- Obtain your Bearer Token from the X developer portal.
- Set it as an environment variable in your system:
  ```bash
  export X_BEARER_TOKEN="your_bearer_token_here"
  ```

### 2. Install Python Dependencies
- This project requires the `requests` library.
- Install it using pip:
  ```bash
  pip install requests
  ```

### 3. Run the Search Script
- Use the provided `x_search.py` script to fetch recent posts:
  ```bash
  python x_search.py <x_account_handle>
  ```
- Replace `<x_account_handle>` with the desired X username (default is `llM_wizard`).

### 4. Review and Summarize
- The script outputs a `posts.json` file with the fetched posts.
- Use AI or manual methods to analyze and summarize the posts.

---

This setup allows you to automate the retrieval and summarization of public X posts for any account of interest.