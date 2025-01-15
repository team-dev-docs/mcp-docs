

  # Getting Started with MCP Servers

This guide will walk you through installing, configuring, and using the various Model Context Protocol (MCP) servers. MCP servers allow AI assistants to interact with external tools and data sources in a standardized way.

## Installation

To install the MCP servers, follow these steps:

1. Clone the MCP servers repository:
   ```
   git clone https://github.com/anthropic-ai/mcp-servers.git
   cd mcp-servers
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Build the servers:
   ```
   npm run build
   ```

## Configuration

Each MCP server may require specific configuration. Here are the configuration steps for each server type:

### Brave Search Server

1. Set the `BRAVE_API_KEY` environment variable with your Brave Search API key:
   ```
   export BRAVE_API_KEY=your_api_key_here
   ```

### GitHub Server

1. Set the `GITHUB_TOKEN` environment variable with your GitHub personal access token:
   ```
   export GITHUB_TOKEN=your_github_token_here
   ```

### GitLab Server

1. Set the `GITLAB_PERSONAL_ACCESS_TOKEN` environment variable with your GitLab personal access token:
   ```
   export GITLAB_PERSONAL_ACCESS_TOKEN=your_gitlab_token_here
   ```

2. Optionally, set the `GITLAB_API_URL` environment variable if you're using a self-hosted GitLab instance:
   ```
   export GITLAB_API_URL=https://your-gitlab-instance.com/api/v4
   ```

### Postgres Server

No additional configuration is required. The database URL will be provided as a command-line argument when running the server.

### Puppeteer Server

No additional configuration is required.

### SQLite Server

No additional configuration is required. The database path will be provided when initializing the server.

### Time Server

No additional configuration is required.

## Usage

Here's how to start and use each MCP server:

### Brave Search Server

1. Start the server:
   ```
   npm run start:brave-search
   ```

2. Use the following tools:
   - `brave_web_search`: Perform a web search
   - `brave_local_search`: Search for local businesses and places

Example usage:
```javascript
const result = await callTool("brave_web_search", { query: "latest AI news", count: 5 });
console.log(result.content[0].text);
```

### GitHub Server

1. Start the server:
   ```
   npm run start:github
   ```

2. Use the following tools:
   - `create_or_update_file`: Create or update a file in a repository
   - `search_repositories`: Search for GitHub repositories
   - `create_repository`: Create a new repository
   - `get_file_contents`: Get contents of a file
   - `push_files`: Push multiple files to a repository
   - `create_issue`: Create a new issue
   - `create_pull_request`: Create a new pull request
   - `fork_repository`: Fork a repository
   - `create_branch`: Create a new branch
   - `list_commits`: List commits in a branch
   - `search_code`: Search for code across repositories
   - `search_issues`: Search for issues and pull requests
   - `search_users`: Search for GitHub users

Example usage:
```javascript
const result = await callTool("search_repositories", { query: "machine learning", page: 1, perPage: 10 });
console.log(result.content[0].text);
```

### GitLab Server

1. Start the server:
   ```
   npm run start:gitlab
   ```

2. Use the following tools:
   - `puppeteer_navigate`: Navigate to a URL
   - `puppeteer_screenshot`: Take a screenshot
   - `puppeteer_click`: Click an element
   - `puppeteer_fill`: Fill out an input field
   - `puppeteer_select`: Select an option from a dropdown
   - `puppeteer_hover`: Hover over an element
   - `puppeteer_evaluate`: Execute JavaScript in the browser console

Example usage:
```javascript
const result = await callTool("puppeteer_navigate", { url: "https://example.com" });
console.log(result.content[0].text);
```

### Postgres Server

1. Start the server with a database URL:
   ```
   npm run start:postgres postgresql://username:password@host:port/database
   ```

2. Use the following tool:
   - `query`: Run a read-only SQL query

Example usage:
```javascript
const result = await callTool("query", { sql: "SELECT * FROM users LIMIT 5" });
console.log(result.content[0].text);
```

### Puppeteer Server

1. Start the server:
   ```
   npm run start:puppeteer
   ```

2. Use the following tools:
   - `puppeteer_navigate`: Navigate to a URL
   - `puppeteer_screenshot`: Take a screenshot
   - `puppeteer_click`: Click an element
   - `puppeteer_fill`: Fill out an input field
   - `puppeteer_select`: Select an option from a dropdown
   - `puppeteer_hover`: Hover over an element
   - `puppeteer_evaluate`: Execute JavaScript in the browser console

Example usage:
```javascript
const result = await callTool("puppeteer_navigate", { url: "https://example.com" });
console.log(result.content[0].text);
```

### SQLite Server

1. Start the server:
   ```
   python -m mcp_server_sqlite /path/to/your/database.db
   ```

2. Use the following tools:
   - `read_query`: Execute a SELECT query
   - `write_query`: Execute an INSERT, UPDATE, or DELETE query
   - `create_table`: Create a new table
   - `list_tables`: List all tables in the database
   - `describe_table`: Get schema information for a table
   - `append_insight`: Add a business insight to the memo

Example usage:
```python
result = await call_tool("read_query", {"query": "SELECT * FROM users LIMIT 5"})
print(result[0].text)
```

### Time Server

1. Start the server:
   ```
   python -m mcp_server_time
   ```

2. Use the following tools:
   - `get_current_time`: Get current time in a specific timezone
   - `convert_time`: Convert time between timezones

Example usage:
```python
result = await call_tool("get_current_time", {"timezone": "America/New_York"})
print(result[0].text)
```

## Conclusion

This guide has walked you through the installation, configuration, and basic usage of various MCP servers. Each server provides unique capabilities for AI assistants to interact with external systems and data sources. By leveraging these servers, you can enhance the functionality of your AI applications and provide more comprehensive and accurate responses to user queries.

  