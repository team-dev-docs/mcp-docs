

  # Brave Search MCP Server Guide

This guide provides detailed information on using the Brave Search MCP (Model Context Protocol) server, including available tools, input schemas, and example usage scenarios.

## Overview

The Brave Search MCP server provides access to Brave's search capabilities through two main tools:
1. Web Search
2. Local Search

These tools allow you to perform general web searches and location-based searches using Brave's search API.

## Prerequisites

Before using the Brave Search MCP server, ensure you have:

1. A valid Brave API key (set as the `BRAVE_API_KEY` environment variable)
2. The MCP SDK installed and configured in your project

## Available Tools

### 1. Web Search Tool

**Name**: `brave_web_search`

**Description**: Performs a web search using the Brave Search API. Ideal for general queries, news, articles, and online content. Use this for broad information gathering, recent events, or when you need diverse web sources.

**Input Schema**:

```json
{
  "type": "object",
  "properties": {
    "query": {
      "type": "string",
      "description": "Search query (max 400 chars, 50 words)"
    },
    "count": {
      "type": "number",
      "description": "Number of results (1-20, default 10)",
      "default": 10
    },
    "offset": {
      "type": "number",
      "description": "Pagination offset (max 9, default 0)",
      "default": 0
    }
  },
  "required": ["query"]
}
```

### 2. Local Search Tool

**Name**: `brave_local_search`

**Description**: Searches for local businesses and places using Brave's Local Search API. Best for queries related to physical locations, businesses, restaurants, services, etc. Returns detailed information including business names, addresses, ratings, review counts, phone numbers, and opening hours.

**Input Schema**:

```json
{
  "type": "object",
  "properties": {
    "query": {
      "type": "string",
      "description": "Local search query (e.g. 'pizza near Central Park')"
    },
    "count": {
      "type": "number",
      "description": "Number of results (1-20, default 5)",
      "default": 5
    }
  },
  "required": ["query"]
}
```

## Usage Examples

### Web Search Example

To perform a web search:

```javascript
const result = await server.callTool("brave_web_search", {
  query: "latest developments in artificial intelligence",
  count: 5
});

console.log(result.content[0].text);
```

This will return 5 web search results related to the latest developments in artificial intelligence.

### Local Search Example

To perform a local search:

```javascript
const result = await server.callTool("brave_local_search", {
  query: "Italian restaurants in New York City",
  count: 3
});

console.log(result.content[0].text);
```

This will return information about 3 Italian restaurants in New York City, including their names, addresses, ratings, and other relevant details.

## Rate Limiting

The Brave Search MCP server implements rate limiting to comply with Brave's API usage policies:

- 1 request per second
- 15,000 requests per month

Exceeding these limits will result in a rate limit error.

## Error Handling

The server returns errors in the following format:

```javascript
{
  content: [
    {
      type: "text",
      text: "Error: [Error message]"
    }
  ],
  isError: true
}
```

Common errors include:
- Invalid arguments
- Rate limit exceeded
- API key not set or invalid
- Unknown tool name

## Best Practices

1. Use `brave_web_search` for general information queries and current events.
2. Use `brave_local_search` for location-based queries or when searching for businesses and services.
3. Handle rate limiting by implementing appropriate delays between requests.
4. Always check the `isError` flag in the response to handle potential errors gracefully.
5. For pagination in web search, use the `offset` parameter to retrieve additional results.

By following this guide, you can effectively utilize the Brave Search MCP server to enhance your applications with powerful web and local search capabilities.

  